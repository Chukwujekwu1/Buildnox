<script >

import navbar from '../components/navbar.vue';
import homeSection2 from '../components/homeSection2.vue';
import homeSection3 from '../components/homeSection3.vue';
import homeSection4 from '../components/homeSection4.vue';
import homeSection5 from '../components/homeSection5.vue';
import homeSection6 from '../components/homeSection6.vue';
import homeSection7 from '../components/homeSection7.vue';
import homeSection8 from '../components/homeSection8.vue';
import house from '../assets/image-2.png';
import man from '../assets/image-1.png';

export default {
  components: {
    navbar,
    homeSection2,
    homeSection3,
    homeSection4,
    homeSection5,
    homeSection6,
    homeSection7,
    homeSection8,
  },
  data() {
    return {
      man: '',
      house: '',
      house,
      man,
    }

  }
}
</script>

<template>
  <main>
    <header>
      <navbar />


      <img :src="house" class="house">
      <img :src="man" class="man">



      <div class="text">
        <h2>VISION IN </h2>
        <h1>BUIL<span>DING</span> </h1>
        <br>
        <div class="text-p">
         <p>
          The point of using Lorem Ipsum is that it 
          has a more-or-less normal distribution of 
          letters, as opposed to using content here 
          normal distribution
        </p> 
        </div>
        
      </div>

    </header>
    <homeSection2 />
    <homeSection3 />
    <homeSection4 />
    <homeSection5 />
    <homeSection6 />
    <homeSection7 />
    <homeSection8 />
  </main>
</template>



<style lang="css" scoped>
header {
  background-image: url('../assets/banner-1.jpg');
  background-size: cover;
  height: 120vh;
  font-family: Roboto, sans-serif;
  color: white;

}







span {
  -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: rgb(255 255 255 / 60%);
  color: transparent
}



@media (max-width:1024px) {
.man{
  display: none;
}
.house{
  display:none;
}
.text{
  margin-left:0 ;
  margin-top: 9rem;
  padding:1.2rem;
}
h2{
  font-size: 3rem;
}
h1{
  font-size: 4rem;
}
.text-p p{
  font-size:1.5rem ;
  line-height: 1.2;
}
.text-p{
  width: 100%;
}
header{
  height:90vh
}
}

@media (min-width: 1200px) {
  .house {
  margin-left: 54.5rem;
  margin-top: 13rem;
}

.man {
  height: 44rem;
  margin-top: -43rem;
  margin-left: 38.5rem;
  position: absolute;
}
.text {
  margin-top: -40rem;
  margin-left: 10rem;
  position: absolute;
}
h2 {
  font-size: 4rem;
}

h1 {
  font-size: 10rem;
}
.text-p p {
  font-size: 20px;
  line-height: 1.7;
  margin-top: -1rem;
}
.text-p{
  width:24rem ;
}

}
</style>
