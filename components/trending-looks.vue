<template>

  <div class="my-8 looks pa-5 px-10">

      <h5 class="display-1 my-5">TRENDING LOOKS</h5>
      <v-row class="my-8">
        <v-col md="3" lg="2" sm="4" cols="6" v-for="(look,i) in looks"  :key="i">
         <v-card>
           <v-card>
             <img :src="look.image" alt="">
           </v-card>
         </v-card>
        </v-col>
      </v-row>

  </div>

</template>

<script>
 export default{
   name:"Looks",

   data(){
     return{
       looks:[
         {
           image:"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSSBvzPEatx8H8Y_INMBQxuagYod9pXkrtIPg&usqp=CAU"
         },
         {
           image:"https://res.cloudinary.com/trunk-club/image/upload/f_auto,q_auto/Blog/20014_SpringTrends_Blog_StreetFashion_SeaSideBlues_00.jpg"
         },
         {
           link:"https://yellowbacks.com/women/look/e004fe00-0114-11ec-b780-5fb0606b520b",
           image:"https://yellowbacks-v1.sfo3.digitaloceanspaces.com/LOOKS/WOMEN/e004fe00-0114-11ec-b780-5fb0606b520b.jpg"
         },
         {
           image:"https://shaye.co.in/media/catalog/product/cache/9d0df6da185847a889b25b0d66162244/a/n/angle_09.jpg"
         },
         {
            link:"https://yellowbacks.com/women/look/8077ffe0-fc60-11eb-bbc6-073170ee8616",
            image:"https://yellowbacks-v1.sfo3.digitaloceanspaces.com/LOOKS/WOMEN/8077ffe0-fc60-11eb-bbc6-073170ee8616.jpg"

         },
         {
            image:"https://yellowbacks-v1.sfo3.digitaloceanspaces.com/LOOKS/WOMEN/8ed0bab0-fa25-11eb-bbc6-073170ee8616.jpg",
            link:"https://yellowbacks.com/women/look/8ed0bab0-fa25-11eb-bbc6-073170ee8616"

         }
       ]
     }
   }
 }

</script>
