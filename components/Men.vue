<template>

  <div class="my-8  pa-5 px-10">

      <h5 class="display-1 my-5">TRENDING IN MEN</h5>
      <v-row class="my-8">
        <v-col md="3" lg="2" sm="4" cols="6" v-for="(look,i) in looks"  :key="i">
          <v-card class="pa-10">
            {{i}}
          </v-card>
        </v-col>
      </v-row>

  </div>

</template>

<script>
 export default{
   name:"Men",
  
   data(){
     return{
       looks:[
         {
           link:"https://yellowbacks.com/men/look/384a3bb0-0706-11ec-b780-5fb0606b520b",
           image:"https://yellowbacks-v1.sfo3.digitaloceanspaces.com/LOOKS/MEN/384a3bb0-0706-11ec-b780-5fb0606b520b.jpg"
         },
         { link:"https://yellowbacks.com/men/look/0dbe14a0-0703-11ec-b780-5fb0606b520b",
           image:"https://yellowbacks-v1.sfo3.digitaloceanspaces.com/LOOKS/MEN/0dbe14a0-0703-11ec-b780-5fb0606b520b.jpg"
         },
         {
           link:"https://yellowbacks.com/men/look/384a3bb0-0706-11ec-b780-5fb0606b520b",
           image:"https://yellowbacks-v1.sfo3.digitaloceanspaces.com/LOOKS/MEN/384a3bb0-0706-11ec-b780-5fb0606b520b.jpg"
         },
         { link:"https://yellowbacks.com/men/look/0dbe14a0-0703-11ec-b780-5fb0606b520b",
           image:"https://yellowbacks-v1.sfo3.digitaloceanspaces.com/LOOKS/MEN/0dbe14a0-0703-11ec-b780-5fb0606b520b.jpg"
         },
         {
           link:"https://yellowbacks.com/men/look/384a3bb0-0706-11ec-b780-5fb0606b520b",
           image:"https://yellowbacks-v1.sfo3.digitaloceanspaces.com/LOOKS/MEN/384a3bb0-0706-11ec-b780-5fb0606b520b.jpg"
         },
         { link:"https://yellowbacks.com/men/look/0dbe14a0-0703-11ec-b780-5fb0606b520b",
           image:"https://yellowbacks-v1.sfo3.digitaloceanspaces.com/LOOKS/MEN/0dbe14a0-0703-11ec-b780-5fb0606b520b.jpg"
         },
         {
           link:"https://yellowbacks.com/men/look/384a3bb0-0706-11ec-b780-5fb0606b520b",
           image:"https://yellowbacks-v1.sfo3.digitaloceanspaces.com/LOOKS/MEN/384a3bb0-0706-11ec-b780-5fb0606b520b.jpg"
         }

       ]
     }
   }
 }

</script>

<style media="screen">
  .looks{
    background-color: white;
  }


</style>
