<script>

import navbar from '../components/navbar.vue';
import homeSection2 from '../components/homeSection2.vue';
import homeSection3 from '../components/homeSection3.vue';
import homeSection4 from '../components/homeSection4.vue'
import house from '../assets/image-2.png';
import man from '../assets/image-1.png';

export default{
  components:{
    navbar,
    homeSection2,
    homeSection3,
    homeSection4,
  },
  data(){
    return{
     man : '' ,
     house: '' ,
     house,
     man,
    }
    
  }
}
</script>

<template>
  <main>
    <header>
    <navbar/>
    <img :src="house" class="house">
    <img :src="man" class="man">
    <div class="text">
      <h2>VISION IN </h2>
    <h1>BUIL<span>DING</span> </h1>
     <br>
     <p>
      The point of using Lorem Ipsum is that it <br>
has a more-or-less normal distribution of <br>
letters, as opposed to using content here <br>
normal distribution
     </p>
    </div>
    
  </header>
  <homeSection2/>
  <homeSection3/>
  <homeSection4/>
  </main>
</template>



<style lang="scss" scoped>
header{
    background-image: url('../assets/banner-1.jpg');
    background-size: cover;
    height: 120vh;
    font-family: Roboto, sans-serif;
    color:white;

    
.house{
  
  margin-left:54.5rem;
  margin-top: 16.8rem;
}
.man{
  margin-left: 40rem;
  margin-top: -44rem;
  height: 45rem;
}
.text{
  margin-top: -40rem;
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
  p{
    font-size: 20px;
    line-height: 1.7;
  }
}
}

</style>
