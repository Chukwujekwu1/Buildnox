<template>
    <main>
        <header>
      <navbar/>
      <h1 class="pageName">{{ pageName }}</h1>
      <img :src="house" alt="">
    </header>
    <p class="h-24"></p>
    <projectSection2/>

    </main>
</template>












<script >
import navbar from '../components/navbar.vue';
import house from '../assets/building3.png';
import projectSection2 from '../components/projectComponents/projectSection2.vue'
export default {
  components: {
    navbar,
    projectSection2,
  },
  data() {
    return {
      house,
      pageName: 'Projects'
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