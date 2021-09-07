<template id="men">
  <div class="">

    <div class="men-banner mb-0 pt-5 pb-0 px-lg-15">
       <h1 class="text-center pa-5">Men's Collection</h1>
    </div>
  <!--back up
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

-->
    <!-- Product listing -->
            <div class="" id="product">
              <p class="pa-2 mt-4"><b>Latest Arrivals</b> </p>
              <v-row class="pa-4">
                <v-col cols="6" md="3" lg="2" sm="6" v-for="(product,i) in products" :key="i">
                  <v-card class="pa-3 card">
                    <a href="/men/product">
                      <img id="product-img" :src="product.image1" alt="">
                    </a>
                    <p>{{product.title}}</p>
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
import axios from "axios"
export default {
  name:"men",
  components:{

  },
  data(){
    return{
      model:null,
      products:[],
    }
  },

/***** API CALL ***/
  mounted(){
   axios
   .get('http://localhost:8000/api/products')
   .then(result => {
     this.products=result.data
   })
  }



}


</script>

<style media="screen">
  .men-banner{
    background-color: #FFDE59;
    height: 20vh;
  }
  #product-img{
    width: 100%;
  }
</style>
