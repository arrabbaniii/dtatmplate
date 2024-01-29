<template>
  <v-app dark>
    <v-navigation-drawer v-model="drawer" app temporary style="background-color:white ;">

      <div v-for="(menu, key) in menuList" :key="key">
        <a class="menulink" @click="active(menu)" :style="{
          'text-transform': 'uppercase',
          'text-decoration': 'none',
          'border-bottom': menu.active || menu.hover ? '2px solid green' : 'none',
          'color': menu.active || menu.hover ? 'green' : 'black',
          'transition': 'border-color 0.3s, color 0.3s'
        }" @mouseover="menu.hover = !menu.hover" @mouseleave="menu.hover = !menu.hover">
          {{ $t(`${menu.name}`) }}
        </a>
      </div>
    </v-navigation-drawer>

    <!-- NAVBAR -->
    <v-app-bar :clipped-left="clipped" fixed app elevation="1" color="white">
      <v-container style="max-width: 1140px; display: flex; justify-content: space-between; align-items: center;">
        <!-- LOGO -->
        <div class="menu-logo">
          <v-img style="max-width: 60px; cursor: pointer" :src="logo" alt="" />
        </div>


        <!-- MENU -->

        <v-app-bar-nav-icon @click.stop="drawer = !drawer" class="mr-4" v-if="isXs" />

        <div style="display: flex;" v-else>
          <div v-for="(menu, key) in menuList" :key="key">
            <a class="menulink" @click="active(menu)" :style="{
              'text-transform': 'uppercase',
              'text-decoration': 'none',
              'border-bottom': menu.active || menu.hover ? '2px solid green' : 'none',
              'color': menu.active || menu.hover ? 'green' : 'black',
              'transition': 'border-color 0.3s, color 0.3s'
            }" @mouseover="menu.hover = !menu.hover" @mouseleave="menu.hover = !menu.hover">
              {{ $t(`${menu.name}`) }}
            </a>
          </div>
        </div>

      </v-container>
    </v-app-bar>

    <!-- APP -->
    <v-main>
      <Nuxt />
    </v-main>

    <v-scale-transition>
      <v-btn fab v-show="fab" v-scroll="onScroll" fixed bottom right color="green" @click="toTop">
        <v-icon style="color: white;">mdi-arrow-up</v-icon>
      </v-btn>
    </v-scale-transition>

    <!-- FOOTER -->
    <v-footer :absolute="!fixed" app>
      <div class="text-center" style="width: 100%;">
        All right reserved © PT. Deta Graha Mulya
      </div>
    </v-footer>
  </v-app>
</template>

<script>

export default {
  name: 'DefaultLayout',
  data() {
    return {
      clipped: false,
      fixed: false,
      drawer: null,
      isXs: false,

      lang: "",

      //LOGO
      logo: require('@/assets/dta_logo.png'),

      //MENU
      menuList: [
        {
          name: `${this.$i18n.t('About Us')}`,
          id: '#about_us',
          active: false,
          hover: false,
        },
        {
          name: `${this.$i18n.t('What We Do')}`,
          id: '#whatwedo',
          active: false,
          hover: false,
        },
        {
          name: `${this.$i18n.t('Portofolio')}`,
          id: '#portofolio',
          active: false,
          hover: false,
        },
        {
          name: `${this.$i18n.t('Clients')}`,
          id: '#clients',
          active: false,
          hover: false,
        },
        {
          name: `${this.$i18n.t('Contact')}`,
          id: '#contact',
          active: false,
          hover: false,
        },
      ],

      fab: null,
      color: "",
      flat: null,
    }
  },

  created() {
    const top = window.pageYOffset || 0;
    if (top <= 60) {
      this.color = "transparent";
      this.flat = true;
    }
  },

  mounted() {
    this.onResize();
    window.addEventListener("resize", this.onResize, { passive: true });
  },

  watch: {
    fab(value) {
      if (value) {
        this.color = "green";
        this.flat = false;
      } else {
        this.color = "transparent";
        this.flat = true;
      }
    },

    isXs(value) {
      if (!value) {
        if (this.drawer) {
          this.drawer = false;
        }
      }
    },

  },

  methods: {

    active(menu) {
      this.menuList.forEach(i => {
        if (i === menu) {
          i.active = true;
          this.$vuetify.goTo(menu.id)
        } else {
          i.active = false;
        }
      });
    },

    onResize() {
      this.isXs = window.innerWidth < 850;
    },

    changeLang(lang) {
      this.lang = lang;
    },

    onScroll(e) {
      if (typeof window === "undefined") return;
      const top = window.pageYOffset || e.target.scrollTop || 0;
      this.fab = top > 60;
    },
    toTop() {
      this.$vuetify.goTo(0);
    },

  },

}
</script>

<style>
.menu-logo {
  display: inline-block;
  padding-top: 0.3125rem;
  padding-bottom: 0.3125rem;
  margin-right: 1rem;
  font-size: 1.25rem;
  line-height: inherit;
  white-space: nowrap;
}

.menulink {
  font-size: 14px;
  padding-top: 5px;
  padding-bottom: 2px;
  margin-left: 30px;
  position: relative;
}
</style>