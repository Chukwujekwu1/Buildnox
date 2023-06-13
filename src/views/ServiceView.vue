<template>
    <main>
        <header>
      <navbar/>
      <h1 class="pageName">{{ pageName }}</h1>
      <img :src="house" alt="">
    </header>
    <serviceSection2 />
    <serviceSection3/>
    </main>
</template>












<script >
import navbar from '../components/navbar.vue';
import house from '../assets/building3.png';
import serviceSection2 from '../components/serviceComponents/serviceSection2.vue'
import serviceSection3 from '../components/serviceComponents/serviceSection3.vue';
export default {
  components: {
    navbar,
    serviceSection2, 
    serviceSection3,
  },
  data() {
    return {
      house,
      pageName: 'Services'
    }
  }
}

</script>

<style lang="css" scoped>
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