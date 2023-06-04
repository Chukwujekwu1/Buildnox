<script>

import navbar from '../components/navbar.vue';
export default{
  components:{
    navbar
  }
}
</script>

<template>
  <main>
    <header>
    <navbar/>
    <img src="../assets/image-2.png" alt="" class="house">
    <img src="../assets/image-1.png" alt="" class="man">
    <div class="text">
      <h2>VISION IN </h2>
    <h1>BUIL<span>DING</span> </h1>

    </div>
    
  </header>
  </main>
</template>
<style lang="scss" scoped>
header{
    background-image: url('../assets/banner-1.jpg');
    background-size: cover;
    height: 100vh;
    font-family: Roboto, sans-serif;
    color:white;

    
.house{
  
  margin-left:51.5rem;
  margin-top: 10.2rem;
}
.man{
  margin-left: 40rem;
  margin-top: -59rem;
  height: 40rem;
}
.text{
  margin-top: -28rem;
  margin-left: 10rem;
  h2{
    font-size: 4rem;
  }
  h1{
    font-size:10rem;
    span{
    -webkit-text-stroke-width: 2px;
    -webkit-text-stroke-color: rgb(255 255 255 / 60%);
    color: transparent
    }
  }
}
}

</style>
