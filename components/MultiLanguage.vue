<template>
  <router-link :to="switchLocalePath(`${langswitcher.toString()}`)"
    @click.native="changeLang(`/${langswitcher.toString()}`)" exact>
      <input v-model="langtoggs" type="checkbox" id="lang-toggle"/>
        <label for="lang-toggle">
      </label>
  
  </router-link>
</template>

<script>
export default {
  data() {
    return {
      isPublic: true,
      lang: "",
      langtoggs: this.$i18n.locale == 'id' ? false : true,
      langswitcher: this.$i18n.locale == 'id' ? 'en' : 'id',
    };
  },
  methods: {
    changeLang(lang) {
      this.lang = lang;
      this.$emit("choosed", this.lang)
    },
  },

  async created() {
    
  },

  watch: {

  }
};
</script>

<style scoped>
.v-list-item--link:before {
  background-color: transparent;
}

.addhover:hover {
  background-color: transparent;
}

label {
	width:50px;
	height:26px;
	position: relative;
	display: block;
	background: #EDEDED;
	border-radius: 50px;
	
	cursor: pointer;
	transition: 0.3s;
}
label:after {
	content: "";
	width:19px;
	height: 19px;
	position: absolute;
	top:3px;
	left:3px;
	background-image: url("https://cdn-icons-png.flaticon.com/32/6157/6157721.png");
    background-position: center; 
	border-radius: 20px;
	transition: 0.3s;
}
input {
	width: 0;
	height: 0;
	visibility: hidden;
}
input:checked + label {
	background: #EDEDED;
}
input:checked + label:after {
	left:47px;
	transform: translateX(-100%);
	background-image: url("https://cdn-icons-png.flaticon.com/32/299/299985.png");
    background-position: center; 
}
label:active:after{
	width: 30x;
}
</style>