<template>
  <div>
    <!-- GANTI BAHASA -->
    <v-container class="mt-4"
      style="max-width: 1140px; display: flex; justify-content: space-between; align-items: center;">
      <v-spacer></v-spacer>
      <MultiLanguage style="margin-left: 30px; margin-top: -25px" @choosed="changeLang($event)"></MultiLanguage>
    </v-container>

    <!-- PARTICLE BACKGROUND -->
    <div id="particles-js"></div>
    <script src="/particles.js"></script>
    <script src="/app.js"></script>

    <!-- TEXT BESAR #about_us -->
    <div class="section" id="about_us">
      <div class="container" style="max-width: 1140px;">
        <v-row class="text-center">
          <v-spacer></v-spacer>
          <v-col cols="12" md="10" sm="12">

            <h1 style="font-size: 120px; font-weight: 800;">
              {{ showText }}
            </h1>

            <h3 class="mt-12" style="color: darkslategrey;">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Corporis, quo quas deserunt numquam ducimus
              repudiandae similique. Dolore doloribus fugit vitae suscipit quasi cumque ex debitis soluta expedita
              eveniet, accusamus nulla?
            </h3>
          </v-col>
          <v-spacer></v-spacer>
        </v-row>
      </div>
    </div>

    <!-- #campaign -->
    <div class="section" id="campaign" style="margin-top: 40px;">
      <div class="container" style="max-width: 1140px;">
        <v-row>
          <v-col cols="4" md="4" sm="4" style="text-align: center;">
            <div>
              <img src="https://growinc.id/assetfront/img/growinc/corona.png" alt="" style="width: 70%;">
            </div>
          </v-col>
          <v-col cols="8" md="8" sm="8">
            <h2 style="font-size: 40px;">
              Startegi bisnis menghadapi <span class="green--text">Krisis</span>
            </h2>
            <h4 class="mt-4" style="color: darkslategrey;">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Corporis, quo quas deserunt numquam ducimus
              repudiandae similique. Dolore doloribus fugit vitae suscipit quasi cumque ex debitis soluta expedita
              eveniet, accusamus nulla?
            </h4>
            <v-btn class="mt-4" color="green" dark href="" style="text-transform: none">
              Next
              <v-icon right>
                mdi-chevron-double-right
              </v-icon>
            </v-btn>
          </v-col>
          <v-spacer></v-spacer>
        </v-row>
      </div>
    </div>

    <!-- #other -->
    <div class="section" id="about" style="margin-top: 40px;">
      <div class="container" style="max-width: 1140px;">
        <v-row>
          <v-col cols="12" md="8" sm="12">
            <h2 style="font-size: 40px;">
              We <span class="green--text">understand</span> that staying <span class="green--text">significant</span> can
              be real <span class="green--text">challenge</span>.
            </h2>
            <h4 class="mt-4" style="color: darkslategrey;">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci sint alias non illum totam at, temporibus
              voluptas ducimus sapiente officiis est cum odio voluptate quae aliquam quidem ipsam voluptatum laboriosam.
            </h4>
          </v-col>
          <v-col cols="12" md="4" sm="12" style="text-align: center;">
            <div>
              <img src="https://growinc.id/assetfront/img/growinc/growinc-background.png" width="380px" alt="">
            </div>
          </v-col>
          <v-spacer></v-spacer>
        </v-row>
      </div>
    </div>

    <!-- we are ... -->
    <div class="section" id="about2" style="margin-top: 40px;">
      <div class="container text-center" style="max-width: 1140px;">
        <v-row>
          <v-spacer></v-spacer>
          <v-col cols="12" md="8" sm="12">
            <h2 style="font-size: 40px;">
              We are <span class="green--text">DTA PROMOTION.</span>
            </h2>
            <h4 class="mt-4" style="color: darkslategrey;">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci sint alias non illum totam at, temporibus
              voluptas ducimus sapiente officiis est cum odio voluptate quae aliquam quidem ipsam voluptatum laboriosam.
            </h4>
          </v-col>
          <v-spacer></v-spacer>
        </v-row>
      </div>
      <div>
        <img src="https://growinc.id/assetfront/img/sebelum_we_are_growinc.png" alt="" style="width:100%;height: 450px">
      </div>
    </div>

    <!-- #whatwedo ... -->
    <div class="section" style="margin-top: 20px;">
      <div class="container text-center" style="max-width: 1140px;">
        <v-row id="whatwedo">
          <v-spacer></v-spacer>
          <v-col cols="12" md="8" sm="12">
            <h2 style="font-size: 40px;">
              We <span class="green--text">craft</span> details to bring solutions to your business.
            </h2>
          </v-col>
          <v-spacer></v-spacer>
        </v-row>

        <v-row class="mt-8" align="center">
          <v-col cols="12" md="4" sm="12">
            <div>
              <img src="https://growinc.id/assets/img/insight-and-evaluation.png" alt="" width="155px">
            </div>
            <h3 class="mb-2">
              INSIGHT & EVALUATION
            </h3>
            <div>
              <p class="mb-1">Market insight</p>
              <p class="mb-1">Data insight</p>
              <p class="mb-1">Competitive analysis</p>
              <p class="mb-1">Asset measurement and optimization</p>
            </div>
          </v-col>
          <v-col cols="12" md="4" sm="12">
            <div>
              <img src="https://growinc.id/assets/img/insight-and-evaluation.png" alt="" width="155px">
            </div>
            <h3 class="mb-2">
              INSIGHT & EVALUATION
            </h3>
            <div>
              <p class="mb-1">Market insight</p>
              <p class="mb-1">Data insight</p>
              <p class="mb-1">Competitive analysis</p>
              <p class="mb-1">Asset measurement and optimization</p>
            </div>
          </v-col>
          <v-col cols="12" md="4" sm="12">
            <div>
              <img src="https://growinc.id/assets/img/insight-and-evaluation.png" alt="" width="155px">
            </div>
            <h3 class="mb-2">
              INSIGHT & EVALUATION
            </h3>
            <div>
              <p class="mb-1">Market insight</p>
              <p class="mb-1">Data insight</p>
              <p class="mb-1">Competitive analysis</p>
              <p class="mb-1">Asset measurement and optimization</p>
            </div>
          </v-col>
        </v-row>

        <v-row class="mt-2" align="center">
          <v-spacer></v-spacer>
          <v-col cols="12" md="4" sm="12">
            <div>
              <img src="https://growinc.id/assets/img/insight-and-evaluation.png" alt="" width="155px">
            </div>
            <h3 class="mb-2">
              INSIGHT & EVALUATION
            </h3>
            <div>
              <p class="mb-1">Market insight</p>
              <p class="mb-1">Data insight</p>
              <p class="mb-1">Competitive analysis</p>
              <p class="mb-1">Asset measurement and optimization</p>
            </div>
          </v-col>
          <v-col cols="12" md="4" sm="12">
            <div>
              <img src="https://growinc.id/assets/img/insight-and-evaluation.png" alt="" width="155px">
            </div>
            <h3 class="mb-4">
              INSIGHT & EVALUATION
            </h3>
            <div>
              <p class="mb-1">Market insight</p>
              <p class="mb-1">Data insight</p>
              <p class="mb-1">Competitive analysis</p>
              <p class="mb-1">Asset measurement and optimization</p>
            </div>
          </v-col>
          <v-spacer></v-spacer>
        </v-row>
      </div>
    </div>

    <!-- OUR WORKS / #portiofolio ... -->
    <div class="section" style="margin-top: 40px;">
      <div class="container text-center" style="max-width: 1140px;">
        <v-row id="portofolio">
          <v-spacer></v-spacer>
          <v-col cols="12" md="8" sm="12">
            <h2 style="font-size: 40px;">
              The <span class="green--text">Portofolio</span>
            </h2>
            <h4 class="mt-4" style="color: darkslategrey; margin-bottom: 20px">
              Products and Services that we provide for advertising and promotion are divided into two parts in general,
              which is outdoor advertising & branding (Banner, Car Branding, Neon Box, and Light Box), and also indoor
              advertising & branding (sticker, showcase, cutting sticker, poster, and many more).
            </h4>
          </v-col>
          <v-spacer></v-spacer>
        </v-row>
        <v-divider class="my-4"></v-divider>

        <!--BANNER-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Banner</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for LotteMart, FamilyMart and Tiptop.
                We use the material such as flexy banner material from flexy banner china 280 to german 440.
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in banner_images" :key="imgkey" class="d-flex child-flex" cols="12" md="4"
              sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Neon Box & Light Box-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Neon Box & Light Box</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for FamilyMart, and Alleira Batik.
                We use the material such as cutting sticker Oracal or Duratran.
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in lightbox_images" :key="imgkey" class="d-flex child-flex" cols="12" md="4"
              sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Car Wrap / Branding-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Car Wrap / Branding</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for Courts, FamilyMart, and GoldFrance.
                We use the material such as Ritrama Vinyl Sticker with matte or glossy finish.
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in car_images" :key="imgkey" class="d-flex child-flex" cols="12" md="4"
              sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Sticker-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Sticker</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for Delami Brands, Courts and Antony Morato.
                Media placement: Wall, Lift Door, and Glass Wall.
                We use the material such as Ritrama Vinyl Sticker with matte or glossy finish, or clear sticker.
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in sticker_images" :key="imgkey" class="d-flex child-flex" cols="12" md="4"
              sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Showcase-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Showcase</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for FamilyMart.
                We use the material such as PVC board, Acrylic, or Impraboard, and then covered with Ritrama Vinyl Sticker
                with matte or glossy finish.
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in showcase_images" :key="imgkey" class="d-flex child-flex" cols="12" md="6"
              sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Cutting Sticker-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Cutting Sticker</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for FamilyMart and Axis
                We use the material such as Oracal cutting sticker, sunblast, and Scotlite.
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in cuttingsticker_images" :key="imgkey" class="d-flex child-flex" cols="12"
              md="4" sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Posters-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Posters</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for FamilyMart, and Lottemart.
                We use the material such as Albatros, Photopaper, and Duratran.
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in posters_images" :key="imgkey" class="d-flex child-flex" cols="12" md="4"
              sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Standing Banner-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Standing Banner</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for FamilyMart.
                We use the material such as Easy Banner, Albatros, and Photopaper
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in standing_banner_images" :key="imgkey" class="d-flex child-flex" cols="12"
              md="4" sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Hanging-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Hanging</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for Courts, FamilyMart, and Lottemart.
                We use the material such as PVC Banner, Albatros, or Ritrama Vinyl Sticker with matte or glossy finish, to
                be placed on PVC Board
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in hanging_images" :key="imgkey" class="d-flex child-flex" cols="12" md="4"
              sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Booth-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Booth</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for Family Mart and PGC Cililitan.
                We use the material as PVC board, impraboard, and wooden based board, and covered with Ritrama Vinyl
                Sticker with matte or glossy finish.
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in booth_images" :key="imgkey" class="d-flex child-flex" cols="12" md="4"
              sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Gondola-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Gondola</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for FamilyMart.
                We use the material such as PVC Board or Impraboard, and coated with Ritrama Vinyl Sticker with matte or
                glossy finish, as desired form and layout design.
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in gondola_images" :key="imgkey" class="d-flex child-flex" cols="12" md="4"
              sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Backdrop-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Backdrop</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our projects for FamilyMart, NS Battery, and Lottemart.
                We use the material such as Ritrama Vinyl Sticker with matte or glossy finish, and also with flexy banner
                material from flexy banner china 280 to german 440.
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in backdrop_images" :key="imgkey" class="d-flex child-flex" cols="12" md="4"
              sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

        <!--Merchandise-->
        <div style="margin-top: 40px">
          <v-row>
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 30px;">
                <span class="green--text">Merchandise</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                Here are some example of our offset print projects for PT. PLN, JNE, and Anna Hospital.
                We also provide any other kind of merchandises / company gifts, such as lanyards, tumbler, notebook,
                umbrella, calender, and many more
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
          <v-row>
            <v-col v-for="(porto_img, imgkey) in merchandise_images" :key="imgkey" class="d-flex child-flex" cols="12"
              md="4" sm="12">
              <v-hover v-slot="{ hover }">
                <v-img :src="porto_img.src" height="285px" style="cursor: pointer" aspect-ratio="1"
                  @click="viewimage(porto_img)">
                  <v-fade-transition>
                    <v-overlay v-if="hover" absolute color="black" opacity="0.5">
                      <v-icon x-large>
                        mdi-magnify-plus-outline
                      </v-icon>
                    </v-overlay>
                  </v-fade-transition>
                </v-img>
              </v-hover>
            </v-col>
          </v-row>
        </div>

      </div>

      <!-- services -->
      <div class="section" id="about" style="margin-top: 40px;">
        <div class="container" style="max-width: 1140px;">
          <v-row>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 40px;">
                <span class="green--text">Services</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey;">
                We also provide consultancy & other services for your campaign needs. We will provide you some case
                studies that related to your campaign, based on your preferences
              </h4>
            </v-col>
            <v-col cols="12" md="4" sm="12" style="text-align: center;">
              <div>
                <img :src="require('@/assets/brand.jpg')" alt="" width="380px">
              </div>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
        </div>
      </div>

      <!-- clients -->
      <div class="section" id="clients" style="margin-top: 40px;">
        <div class="container" style="max-width: 1140px;">
          <v-row>
            <v-col cols="12" md="6" sm="12">
              <h2 style="font-size: 40px;">
                We help local and international businesses in Indonesia to grow.
              </h2>
              <hr style="border-bottom: 4px solid green; width: 25%;">
              <h4 class="mt-8" style="color: darkslategrey; text-align: justify;">
                Growinc is a full-service marketing & advertising agency, leading its agencies: Growmint, Nesvara and Nata
                Software House to give actionable business solutions and drive better business impact for clients and
                partners, using measurable performance-base initiatives, in order to achieve higher impact.
              </h4>
            </v-col>
            <v-col cols="12" md="6" sm="12" align="right">
              <div>
                <img :src="require('@/assets/client.png')" alt="" width="450px">
              </div>
            </v-col>
          </v-row>
        </div>
      </div>

      <!-- OUR COMPANY  -->
      <div class="section" style="margin-top: 40px;">
        <div class="container text-center" style="max-width: 1140px;">
          <v-row id="company">
            <v-spacer></v-spacer>
            <v-col cols="12" md="8" sm="12">
              <h2 style="font-size: 40px;">
                Our <span class="green--text">Companies</span>
              </h2>
              <h4 class="mt-4" style="color: darkslategrey; margin-bottom: 20px">
                How our capabilities can be linked seamlessly to ensure continous bussiness growth.
              </h4>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>

          <v-row>
            <v-col v-for="(comp, imgkey) in companies" :key="imgkey" cols="12" md="3" sm="12">
              <div style="height: 120px; display: flex; justify-content: center; align-items: center;">
                <v-hover v-slot="{ hover }">
                  <v-img :src="comp.src" width="255px" max-height="120px" style="cursor: pointer">
                    <v-fade-transition>
                      <v-overlay v-if="hover" absolute color="black" opacity="0.8">
                        <h4>{{ comp.name }}</h4>
                      </v-overlay>
                    </v-fade-transition>
                  </v-img>
                </v-hover>
              </div>
              <div class="mt-8">{{ comp.desc }}</div>
            </v-col>
          </v-row>

        </div>
      </div>

      <!-- team -->
      <div class="section" id="team" style="margin-top: 40px;">
        <div class="container" style="max-width: 1140px;">
          <v-row>
            <v-col cols="12" md="7" sm="12">
              <div>
                <img src="https://growinc.id/assetfront/img/growinc/growinc_team.png" alt="" width="635px">
              </div>
            </v-col>
            <v-col cols="12" md="5" sm="12">
              <h2 style="font-size: 40px;">
                Meet the team who grow.
              </h2>
              <hr style="border-bottom: 4px solid green; width: 25%;">
              <h4 class="mt-8" style="color: darkslategrey; text-align: justify;">
                Get to know better about who are responsible for our clients growth
              </h4>
              <v-btn class="mt-4" color="green" dark href="" style="text-transform: none">
                See our leaders
              </v-btn>
            </v-col>
          </v-row>
        </div>
      </div>

      <!-- contact -->
      <div class="section" id="contact" style="margin-top: 40px;">
        <div class="container" style="max-width: 1140px;">
          <v-row class="text-center">
            <v-spacer></v-spacer>
            <v-col cols="12" md="6" sm="12">
              <div>
                <img src="https://growinc.id/assetfront/img/growmint/letsTalk.png" alt="" width="200px">
              </div>
              <h2 style="font-size: 40px;">
                What we can do for you?
              </h2>
              <h4 class="mt-8" style="color: darkslategrey; text-align: justify;">
                If you have any ideas, we're here to listen and help your achieve your
              </h4>
              <v-btn class="mt-4" color="green" dark href="" style="text-transform: none">
                Let's talk
              </v-btn>
            </v-col>
            <v-spacer></v-spacer>
          </v-row>
        </div>
      </div>

      <div class="section" id="contact2" style="margin-top: 40px;">
        <div style="background-color: darkslategray">
          <div class="container" style="max-width: 1140px;">
            <v-row class="mt-2">
              <v-col cols="12" md="4" sm="12">
                <v-img style="max-width: 100px; cursor: pointer" :src="logo" alt="" />
                <p class="mt-4" style="color: white">
                  Pt. Deta Graha Mulya
                </p>
              </v-col>
              <v-col cols="12" md="4" sm="12">
                <p class="mb-2" style="color:white">
                  Komplek Golden Fatmawati
                  <br>
                  Jl. RS. Fatmawati No.15, RT 03 RW 06 
                  <br>
                  Kel. Gandaria Selatan, Kec. Cilandak
                  <br>
                  Jakarta Selatan 12420
                </p>
                <div>
                  <v-btn icon href="https://www.facebook.com/" dark>
                    <v-icon>
                      mdi-facebook
                    </v-icon>
                  </v-btn>
                  <v-btn icon href="https://www.linkedin.com/" dark>
                    <v-icon>
                      mdi-linkedin
                    </v-icon>
                  </v-btn>
                  <v-btn icon href="https://www.instagram.com/" dark>
                    <v-icon>
                      mdi-instagram
                    </v-icon>
                  </v-btn>
                </div>
              </v-col>
              <v-col cols="12" md="4" sm="12">
                <div v-for="(menu, key) in menuList" :key="key">
                  <div class="mb-1">
                    <a :style="{
                      'text-transform': 'uppercase',
                      'text-decoration': 'none',
                      'border-bottom': menu.hover ? '2px solid green' : 'none',
                      'color': menu.hover ? 'green' : 'white',
                      'transition': 'border-color 0.3s, color 0.3s'
                    }" @mouseover="menu.hover = !menu.hover" @mouseleave="menu.hover = !menu.hover">
                      {{ $t(`${menu.name}`) }}
                    </a>
                  </div>
                </div>
              </v-col>
            </v-row>
          </div>
        </div>
        
      </div>

    </div>

    <v-dialog v-model="imageModal" max-width="600px">
      <v-card>
        <v-card-title class="mb-2">
          {{ image_detail_name }}
          <v-spacer></v-spacer>
          <v-icon @click="imageModal = false" small class="grey-icon">
            mdi-close
          </v-icon>
        </v-card-title>
        <v-card-text>
          <v-img :src="image_detail_src"></v-img>
        </v-card-text>
      </v-card>
    </v-dialog>


  </div>
</template>

<script>

import MultiLanguage from "~/components/MultiLanguage";
export default {
  components: {
    MultiLanguage
  },
  data() {
    return {
      lang: "",
      logo: require('@/assets/dta_logo.png'),

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

      mainText: [
        { text: 'We Solve Problems' },
        { text: 'We Drive Progress' },
        { text: 'We Leverage Growth' }
      ],
      showText: 'We Solve Problems',
      
      textCounter: 0,
      interval: null,

      imageModal: false,
      image_detail_name: '',
      image_detail_src: '',

      banner_images: [
        {
          name: 'Banner',
          src: require('@/assets/banner1.png'),
        },
        {
          name: 'Banner',
          src: require('@/assets/banner2.png')
        },
        {
          name: 'Banner',
          src: require('@/assets/banner3.png')
        },
      ],

      lightbox_images: [
        {
          name: 'Neon Box & Light Box',
          src: require('@/assets/box1.png'),
        },
        {
          name: 'Neon Box & Light Box',
          src: require('@/assets/box2.png')
        },
        {
          name: 'Neon Box & Light Box',
          src: require('@/assets/box3.png')
        },
      ],

      car_images: [
        {
          name: 'Car Wrap / Branding',
          src: require('@/assets/car1.png'),
        },
        {
          name: 'Car Wrap / Branding',
          src: require('@/assets/car2.png')
        },
        {
          name: 'Car Wrap / Branding',
          src: require('@/assets/car3.png')
        },
      ],

      sticker_images: [
        {
          name: 'Stickers',
          src: require('@/assets/sticker1.png'),
        },
        {
          name: 'Stickers',
          src: require('@/assets/sticker2.png')
        },
        {
          name: 'Stickers',
          src: require('@/assets/sticker3.png')
        },
      ],

      showcase_images: [
        {
          name: 'Showcase',
          src: require('@/assets/showcase1.png'),
        },
        {
          name: 'Showcase',
          src: require('@/assets/showcase2.png')
        },
      ],

      cuttingsticker_images: [
        {
          name: 'Cutting Stickers',
          src: require('@/assets/cutting_sticker1.png'),
        },
        {
          name: 'Cutting Stickers',
          src: require('@/assets/cutting_sticker2.png')
        },
        {
          name: 'Cutting Stickers',
          src: require('@/assets/cutting_sticker3.png')
        },
      ],

      posters_images: [
        {
          name: 'Posters',
          src: require('@/assets/posters1.png'),
        },
        {
          name: 'Posters',
          src: require('@/assets/posters2.png')
        },
        {
          name: 'Posters',
          src: require('@/assets/posters3.png')
        },
      ],

      standing_banner_images: [
        {
          name: 'Standing Banner',
          src: require('@/assets/standing_banner1.png'),
        },
        {
          name: 'Standing Banner',
          src: require('@/assets/standing_banner2.png')
        },
        {
          name: 'Standing Banner',
          src: require('@/assets/standing_banner3.png')
        },
      ],

      hanging_images: [
        {
          name: 'Hanging',
          src: require('@/assets/hanging1.png'),
        },
        {
          name: 'Hanging',
          src: require('@/assets/hanging2.png')
        },
        {
          name: 'Hanging',
          src: require('@/assets/hanging3.png')
        },
      ],

      booth_images: [
        {
          name: 'Booth',
          src: require('@/assets/booth1.png'),
        },
        {
          name: 'Booth',
          src: require('@/assets/booth2.png')
        },
        {
          name: 'Booth',
          src: require('@/assets/booth3.png')
        },
      ],

      gondola_images: [
        {
          name: 'Gondola Branding',
          src: require('@/assets/gondola1.png'),
        },
        {
          name: 'Gondola Branding',
          src: require('@/assets/gondola2.png')
        },
        {
          name: 'Gondola Branding',
          src: require('@/assets/gondola3.png')
        },
      ],

      backdrop_images: [
        {
          name: 'Backdrop',
          src: require('@/assets/backdrop1.png'),
        },
        {
          name: 'Backdrop',
          src: require('@/assets/backdrop2.png')
        },
        {
          name: 'Backdrop',
          src: require('@/assets/backdrop3.png')
        },
      ],

      merchandise_images: [
        {
          name: 'Merchandise',
          src: require('@/assets/merchandise1.png'),
        },
        {
          name: 'Merchandise',
          src: require('@/assets/merchandise2.png')
        },
        {
          name: 'Merchandise',
          src: require('@/assets/merchandise3.png')
        },
      ],

      companies: [
        {
          name: 'Growmint',
          desc: 'A digital company focusing on delivering impacts that matter for clients business.',
          link: 'https://growinc.id/Home/growmint',
          src: 'https://growinc.id/assetfront/img/growmint/growmint.svg'
        },
        {
          name: 'Nesvara',
          desc: 'A brand experience company that delivers brand stories through strategic integrated actions.',
          link: 'https://growinc.id/Home/nesvara',
          src: 'https://growinc.id/assets/img/product/NESVARA-LOGO.png'
        },
        {
          name: 'Kira Kreasi',
          desc: 'An IP Builder company, we are the architects of innovation, specializing in transforming imaginative concepts into thriving business.',
          link: 'https://www.linkedin.com/company/kira-kreasi/about/?viewAsMember=true',
          src: 'https://growinc.id/assets/img/product/Kira-Kreasi.png',
        },
        {
          name: 'Buatan Tangan Studio',
          desc: 'A Manufacture handmade shoes and fashion accessories over 15 years of experience.',
          link: 'https://www.buatantanganstudio.com/',
          src: 'https://growinc.id/assets/img/product/Buatan-Tangan-Studio-3.png',
        },
      ],
    }
  },

  mounted() {
    this.interval = setInterval(this.swapText, 3000);
  },

  beforeDestroy() {
    clearInterval(this.interval)
  },

  created() {

  },

  methods: {

    changeLang(lang) {
      this.lang = lang;
    },

    swapText() {
      this.textCounter = (this.textCounter + 1) % this.mainText.length;
      this.showText = this.mainText[this.textCounter].text;
    },

    viewimage(porto_img) {
      this.image_detail_name = porto_img.name
      this.image_detail_src = porto_img.src
      this.imageModal = true
    }

  }
}
</script>

<style>
#about_us {
  overflow: hidden;
}

#particles-js {
  position: absolute;
  width: 100%;
  height: 800px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: 50% 50%;
  opacity: 0.48;
}

.section {
  padding-top: 60px;
}

</style>