<template >
  <div class="container">
   <div class="images">

   </div>
  </div>
</template>

<script>
  import axios from 'axios'
  export default{

    data(){
      return{
        product:{}
      }
    },

/*
    async  created(){

      const config = {
        headers:{
          'Accept':'application/JSON'
        }
      }
      try {
        const res = await axios.get(`https://icanhazdadjoke.com/j/${this.$route.params.id}`,config)
        this.product = res.data
      } catch (e) {
        console.log(e)
      }

    },
    */
  };
</script>

<style media="screen">
  .images{
    width: 200px;
    height: 230px;
  }
</style>
