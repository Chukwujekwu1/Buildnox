<template>
    <main>
        <header>
      <navbar/>
      <h1 class="pageName">{{ pageName }}</h1>
      <img :src="house" alt="">
    </header>
 
   
    <contactSection2/>
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2611002.5713613164!2d11.13022558156816!3d50.27685846089855!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47c609c3db87e4bb%3A0xb3a175ceffbd0a9f!2sNetherlands!5e0!3m2!1sen!2sng!4v1686828554833!5m2!1sen!2sng" width="100%" height="400" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
    <footer_div />
    </main>
</template>












<script >
import navbar from '../components/navbar.vue';
import footer_div from '../components/footer.vue'
import house from '../assets/building3.png';
import contactSection2 from '../components/contactComponents/contactSection1.vue'

export default {
  components: {
    navbar,
    contactSection2,
    footer_div ,
  },
  data() {
    return {
      house,
      pageName: 'Contact'
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