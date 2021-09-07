<template>

  <div class="my-8">
    <v-container class="">
      <h5 class="display-1 mb-5">EXPLORE TOP BRANDS</h5>
      <v-row class="my-8">
        <v-col md="2" lg="2" v-for="(brand,i) in brands"  :key="i">
          <v-card flat class="text-center">
          <v-avatar size="100" class="center">
            <img :src="brand.logo" alt="" class="text-center">
          </v-avatar>
           <h4 class="text-center mt-2 pa-1">{{brand.name}}</h4>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>

</template>

<script>
 export default{
   name:"Brands",
   data(){
     return{
       brands:[
         {
           name:"ZARA",
           logo:"https://img.mensxp.com/media/content/2019/Feb/the-new-zara-logo-has-made-people-upset1400-1549374083.jpg?w=820&h=540&cc=1"
         },
         {
           name:"LEVI'S",
           logo:"https://thumbs.dreamstime.com/b/levi-strauss-co-privately-held-american-clothing-company-levis-logo-above-entrance-to-store-krasnoyarsk-russia-may-220694800.jpg"
         },
         {
           name:"GUCCI",
           logo:"https://blog.logomyway.com/wp-content/uploads/2016/12/gucci-logo-gold.jpg"
         },
         {
           name:"ROADSTER",
           logo:"https://etimg.etb2bimg.com/thumb/msid-53739843,width-700,resizemode-4/.jpg"
         },
         {
           name:"HRX",
            logo:"https://upload.wikimedia.org/wikipedia/commons/b/bf/Hrx_logo.jpg"

         },
         {
           name:"JACK & JONES",
            logo:"https://pbs.twimg.com/profile_images/1035441567069175809/DndJA0CN_400x400.jpg"

         }
       ]
     }
   }
 }

</script>
