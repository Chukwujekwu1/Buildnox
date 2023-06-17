<template>
    <main>
        <header>
      <navbar/>
      <h1 class="pageName">{{ pageName }}</h1>
      <img :src="house" alt="">
    </header>
    <!-- <p class="h-2"></p> -->
    <teamSection2/>
    <teamSection3/>
    <footer_div/>
    </main>
</template>












<script >
import navbar from '../components/navbar.vue';
import footer_div from '../components/footer.vue';
import house from '../assets/building3.png';
import teamSection2 from '../components/teamComponents/teamSection2.vue'
import teamSection3 from '../components/teamComponents/teamSection3.vue'
export default {
  components: {
    navbar,
    teamSection2,
    teamSection3,
    footer_div,
  },
  data() {
    return {
      house,
      pageName: 'Team'
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