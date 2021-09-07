<template>
 <div class="">


     <template class="banner  hidden-sm-and-down mb-10">
      <v-carousel hide-delimiters>
        <v-carousel-item
          v-for="(banner,i) in banners"
          :key="i"
          :src="banner.src"

        >
        <v-container>
          <h3 v-if="banner.heading" class="display-1 pa-10 mt-7"><b>{{banner.heading}}</b>
            <br>
            <v-btn text :to="banner.link" class="yellow">
              ShopNow
            </v-btn>
          </h3>
        </v-container>
        </v-carousel-item>
      </v-carousel>
    </template>


   <div class="pa-lg-3 mt-5 hidden-md-and-up mb-10">

         <template >
           <v-sheet
             class="mx-auto"
           >
             <v-slide-group
               multiple
               show-arrows
             >
               <v-slide-item
                 v-for="c in 10 "
                 :key="c"
                 v-slot="{ active, toggle }"

               >
                <v-avatar
                 class="mx-2"
                 size="70"
                >
                 <img src="https://4.imimg.com/data4/AA/HC/MY-26596027/men-s-fancy-t-shirt-500x500.jpg" alt="">
                </v-avatar>
                 <v-btn

               </v-slide-item>
             </v-slide-group>
           </v-sheet>
         </template>
         <br>
         <hr>
         </div>

<!-- Slides -->
<Slide />
<!-- Brand logo -->
<Brands />
<!-- Looks -->

 <!-- Product listing -->
         <div class="" id="product">
           <h4 class="display-1 pa-5"><b>Latest Arrivals</b> </h4>
           <v-row>

             <v-col cols="6" md="3" lg="2" sm="6" >
               <v-card class="pa-3 card">
                 <img src="https://webmerx.sgp1.cdn.digitaloceanspaces.com/khankudi/product_images/1625489525.TEEM0042.jpeg" alt="">
                 <template >
                   <v-bottom-navigation
                      color="yellow"
                      horizontal
                      elevation="0"
                    >
                      <v-btn>
                          <v-icon>mdi-heart</v-icon>
                      </v-btn>

                      <v-btn>
                        <v-icon>mdi-shopping</v-icon>
                      </v-btn>
                    </v-bottom-navigation>
                 </template>
               </v-card>
             </v-col>
             <v-col cols="6" md="3" lg="2" sm="6" >
               <v-card class="pa-3 card">
                 <img src="https://webmerx.sgp1.cdn.digitaloceanspaces.com/khankudi/product_images/1625489525.TEEM0042.jpeg" alt="">
                 <template >
                   <v-bottom-navigation
                      color="yellow"
                      horizontal
                      elevation="0"
                    >
                      <v-btn>
                          <v-icon>mdi-heart</v-icon>
                      </v-btn>

                      <v-btn>
                        <v-icon>mdi-shopping</v-icon>
                      </v-btn>
                    </v-bottom-navigation>
                 </template>
               </v-card>
             </v-col>
             <v-col cols="6" md="3" lg="2" sm="6" >
               <v-card class="pa-3 card">
                 <img src="https://webmerx.sgp1.cdn.digitaloceanspaces.com/khankudi/product_images/1625489525.TEEM0042.jpeg" alt="">
                 <template >
                   <v-bottom-navigation
                      color="yellow"
                      horizontal
                      elevation="0"
                    >
                      <v-btn>
                          <v-icon>mdi-heart</v-icon>
                      </v-btn>

                      <v-btn>
                        <v-icon>mdi-shopping</v-icon>
                      </v-btn>
                    </v-bottom-navigation>
                 </template>
               </v-card>
             </v-col>
             <v-col cols="6" md="3" lg="2" sm="6" >
               <v-card class="pa-3 card">
                 <img src="https://webmerx.sgp1.cdn.digitaloceanspaces.com/khankudi/product_images/1625489525.TEEM0042.jpeg" alt="">
                 <template >
                   <v-bottom-navigation
                      color="yellow"
                      horizontal
                      elevation="0"
                    >
                      <v-btn>
                          <v-icon>mdi-heart</v-icon>
                      </v-btn>

                      <v-btn>
                        <v-icon>mdi-shopping</v-icon>
                      </v-btn>
                    </v-bottom-navigation>
                 </template>
               </v-card>
             </v-col>
             <v-col cols="6" md="3" lg="2" sm="6" >
               <v-card class="pa-3 card">
                 <img src="https://webmerx.sgp1.cdn.digitaloceanspaces.com/khankudi/product_images/1625489525.TEEM0042.jpeg" alt="">
                 <template >
                   <v-bottom-navigation
                      color="yellow"
                      horizontal
                      elevation="0"
                    >
                      <v-btn>
                          <v-icon>mdi-heart</v-icon>
                      </v-btn>

                      <v-btn>
                        <v-icon>mdi-shopping</v-icon>
                      </v-btn>
                    </v-bottom-navigation>
                 </template>
               </v-card>
             </v-col>
             <v-col cols="6" md="3" lg="2" sm="6" >
               <v-card class="pa-3 card">
                 <img src="https://webmerx.sgp1.cdn.digitaloceanspaces.com/khankudi/product_images/1625489525.TEEM0042.jpeg" alt="">
                 <template >
                   <v-bottom-navigation
                      color="yellow"
                      horizontal
                      elevation="0"
                    >
                      <v-btn>
                          <v-icon>mdi-heart</v-icon>
                      </v-btn>

                      <v-btn>
                        <v-icon>mdi-shopping</v-icon>
                      </v-btn>
                    </v-bottom-navigation>
                 </template>
               </v-card>
             </v-col>
             <v-col cols="6" md="3" lg="2" sm="6" >
               <v-card class="pa-3 card">
                 <img src="https://webmerx.sgp1.cdn.digitaloceanspaces.com/khankudi/product_images/1625489525.TEEM0042.jpeg" alt="">
                 <template >
                   <v-bottom-navigation
                      color="yellow"
                      horizontal
                      elevation="0"
                    >
                      <v-btn>
                          <v-icon>mdi-heart</v-icon>
                      </v-btn>

                      <v-btn>
                        <v-icon>mdi-shopping</v-icon>
                      </v-btn>
                    </v-bottom-navigation>
                 </template>
               </v-card>
             </v-col>
             <v-col cols="6" md="3" lg="2" sm="6" >
               <v-card class="pa-3 card">
                 <img src="https://webmerx.sgp1.cdn.digitaloceanspaces.com/khankudi/product_images/1625489525.TEEM0042.jpeg" alt="">
                 <template >
                   <v-bottom-navigation
                      color="yellow"
                      horizontal
                      elevation="0"
                    >
                      <v-btn>
                          <v-icon>mdi-heart</v-icon>
                      </v-btn>

                      <v-btn>
                        <v-icon>mdi-shopping</v-icon>
                      </v-btn>
                    </v-bottom-navigation>
                 </template>
               </v-card>
             </v-col>

           </v-row>
         </div>
 </div>
</template>
<script>
import Brands from '@/components/Brand'
import Slide from '@/components/slide'


  export default {
    data: () => ({
      model: null,
      banners: [
          {
            src: './banner/banner1.png',
            heading:"Women Monson Sale",
            link:"/collection/women"
          },
          {
            src: './banner/men-banner.png',
              heading:"Men Monson Sale",
          },
          {
            src: './banner/banner1.png',
              heading:"Kids Monson Sale",
          },
          {
            src: './banner/men-banner.png',
              heading:"Women Monson Sale",
          },
        ],
    }),
    components:{
      Brands,
      Slide,
    }
  }
</script>

<style media="screen">
  #product img{
    width: 100%;
    height: 70%;
  }
  .card{
    width: 250px
  }
  .banner{
    width: 100%;
    height:40vh;
    background-color: orange;
  }
</style>
