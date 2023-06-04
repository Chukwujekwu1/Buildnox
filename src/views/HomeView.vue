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
  </header>
  </main>
</template>
<style scoped>
header{
    background-image: url('../assets/banner-1.jpg');
    background-size: cover;
    height: 95vh;
}

</style>
