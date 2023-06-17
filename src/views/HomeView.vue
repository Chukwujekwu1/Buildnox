<script >

import navbar from '../components/navbar.vue';
import footer_div from '../components/footer.vue';
import homeSection2 from '../components/homeSection2.vue';
import homeSection3 from '../components/homeSection3.vue';
import homeSection4 from '../components/homeSection4.vue'
import homeSection5 from '../components/homeSection5.vue';
import homeSection6 from '../components/homeSection6.vue';
import homeSection7 from '../components/homeSection7.vue';
import homeSection8 from '../components/homeSection8.vue';
import house from '../assets/image-2.png';
import man from '../assets/image-1.png';

export default {

  components: {
    navbar,
    footer_div,
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
      mobile_nav: false,
      man,
      links: [
        {
          text: 'Home',
          path: '/'
        },
        {
          text: 'About',
          path: '/about'
        },
        {
          text: 'Contact',
          path: '/contact'
        },
        {
          text: 'Project',
          path: '/project'
        },
        {
          text: 'Team',
          path: '/team'
        },
        {
          text: 'Services',
          path: '/services'
        },
      ],
    }
  },
  methods: {
    show() {
      this.mobile_nav = !this.mobile_nav
    }
  }
}
</script>

<template>
  <main>
    <header>
      <navbar @my-event="show" />


      <img :src="house" class="house">
      <img :src="man" class="man">


      <div class="mobile">
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
        <div v-if="mobile_nav" class="mobile_view">
          
             <p class="text3"><a :href="link.path" v-for="link in links" class="flex flex-col text-3xl mt-6 ">{{ link.text }}</a>
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
    <footer_div />
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

.mobile_view {
  width: 100%;
  height: 88vh;
  margin: auto;
  background-color: rgba(0,0,0,0.9);
  position: absolute;
  justify-self: end;
  text-align: end;
  padding: 3rem;
  padding-top: 1rem;


}


.text3{
    color:white;
}



span {
  -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: rgb(255 255 255 / 60%);
  color: transparent
}



@media (max-width:1024px) {
  .man {
    display: none;
  }

  .house {
    display: none;
  }

  .text {
    margin-left: 0;
    margin-top: 9rem;
  }

  h2 {
    font-size: 3rem;
  }

  h1 {
    font-size: 4rem;
  }

  .text-p p {
    font-size: 1.5rem;
    line-height: 1.2;
  }

  .text-p {
    width: 100%;
  }

  header {
    height: 100vh
  }

  .mobile {
    display: grid;
    grid-template-columns: auto auto;
    padding: 1.2rem;
    padding-right: 0rem;
    padding-top: 0rem;
  }
}

@media (min-width: 1100px) {
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

  .text-p {
    width: 24rem;
  }

}</style>
