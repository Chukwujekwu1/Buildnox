<template>
  <main>
    <header>
      <navbar />
      <h1 class="pageName">{{ pageName }}</h1>
      <img :src="house" alt="">
    </header>
    <p class="h-24"></p>
    <aboutSection2 />
    <aboutSection3/>
    <aboutSection4 />
    <aboutSection5/>
    <aboutSection6/>



  </main>
</template>






<script>
import navbar from '../components/navbar.vue';
import house from '../assets/building3.png';
import aboutSection2 from '../components/aboutComponents/aboutSection2.vue';
import aboutSection3 from '../components/aboutComponents/aboutSection3.vue';
import aboutSection4 from '../components/aboutComponents/aboutSection4.vue';
import aboutSection5 from '../components/aboutComponents/aboutSection5.vue';
import aboutSection6 from '../components/aboutComponents/aboutSection6.vue';
export default {
  components: {
    navbar,
    aboutSection2,
    aboutSection3,
    aboutSection4,
    aboutSection5,
    aboutSection6,
  },
  data() {
    return {
      house,
      pageName: 'About'
    }
  }
}
</script>
<style scoped>
header {
  background-image: url('../assets/banner-1.jpg');
  background-size: cover;
  height: 70vh;
  font-family: Roboto, sans-serif;
  color: white;
  text-align: center;
}

img {
  margin-left: 65.2%;
  margin-top: -7.2rem;
}

.pageName {
  font-size: 3.6rem;
  font-weight: 750;
  color: white;
  margin-top: 5.5rem;
}

@media (max-width: 1024px) {
  img {
    display: none;
  }
}
</style>
