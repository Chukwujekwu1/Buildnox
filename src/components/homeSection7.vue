<template>
  <div class="bg  flex-row flex p-24 pt-28">
    <div class="flex flex-col">
      <div class="hr3">
        <hr>
        <h3>{{ header1 }} </h3>
      </div>
      <h1 class="header2">
        {{ header2 }}
      </h1>
    </div>




    <swiper :slides-per-view="2" :space-between="0" @swiper="onSwiper" @slideChange="onSlideChange"
      :autoplay='{ delay: 9000, disableOnInteraction: false }' class="flex flex-row mySwiper ">
      <swiper-slide>
        <div class="flex flex-col">
          <div class="flex flex-col w-96 h-72 rounded-lg bg-white p-12  ">
            <img :src="quotes" alt="" class="h-12 w-12">
            <p class="font-normal text-base leading-8  mt-2">{{ text }}</p>
          </div>
          <div class="flex flex-row mt-7 ml-12">
            <img :src="img[0]" class="rounded-full">
            <div class=" flex flex-col ml-4">
              <h2 class="font-bold text-2xl  text-white">{{ names[0] }}</h2>
              <p class=" text_col">{{ personel }}</p>
            </div>
          </div>
        </div>
      </swiper-slide>
      <swiper-slide>
        <div class="flex flex-col">
          <div class="flex flex-col w-96 h-72 rounded-lg bg-white p-12  ">
            <img :src="quotes" alt="" class="h-12 w-12">
            <p class="font-normal text-base leading-8  mt-2">{{ text }}</p>
          </div>
          <div class="flex flex-row mt-7 ml-12">
            <img :src="img[1]" class="rounded-full">
            <div class=" flex flex-col ml-4">
              <h2 class="font-bold text-2xl  text-white">{{ names[1] }}</h2>
              <p class=" text_col">{{ personel }}</p>
            </div>
          </div>
        </div>

      </swiper-slide>
      <swiper-slide>
        <div class="flex flex-col">
          <div class="flex flex-col w-96 h-72 rounded-lg bg-white p-12  ">
            <img :src="quotes" alt="" class="h-12 w-12">
            <p class="font-normal text-base leading-8  mt-2">{{ text }}</p>
          </div>
          <div class="flex flex-row mt-7 ml-12">
            <img :src="img[2]" class="rounded-full">
            <div class=" flex flex-col ml-4">
              <h2 class="font-bold text-2xl  text-white">{{ names[2] }}</h2>
              <p class=" text_col">{{ personel }}</p>
            </div>
          </div>
        </div>

      </swiper-slide>
      <swiper-slide>
        <div class="flex flex-col">
          <div class="flex flex-col w-96 h-72 rounded-lg bg-white p-12  ">
            <img :src="quotes" alt="" class="h-12 w-12">
            <p class="font-normal text-base leading-8  mt-2">{{ text }}</p>
          </div>
          <div class="flex flex-row mt-7 ml-12">
            <img :src="img[3]" class="rounded-full">
            <div class=" flex flex-col ml-4">
              <h2 class="font-bold text-2xl  text-white">{{ names[3] }}</h2>
              <p class=" text_col">{{ personel }}</p>
            </div>
          </div>
        </div>

      </swiper-slide>

      <swiper-slide>
        <div class="flex flex-col">
          <div class="flex flex-col w-96 h-72 rounded-lg bg-white p-12  ">
            <img :src="quotes" alt="" class="h-12 w-12">
            <p class="font-normal text-base leading-8  mt-2">{{ text }}</p>
          </div>
          <div class="flex flex-row mt-7 ml-12">
            <img :src="img[4]" class="rounded-full">
            <div class=" flex flex-col ml-4">
              <h2 class="font-bold text-2xl  text-white">{{ names[4] }}</h2>
              <p class=" text_col">{{ personel }}</p>
            </div>
          </div>
        </div>

      </swiper-slide>
      ...
    </swiper>













  </div>
</template>

<script>
import SwiperCore, { Autoplay } from 'swiper/core';
SwiperCore.use(Autoplay);
import 'swiper/css';
import { Swiper, SwiperSlide } from 'swiper/vue';
import customer1 from './icons/author-1.jpg'
import customer3 from './icons/author-3.jpg'
import customer4 from './icons/author-4.jpg'
import customer7 from './icons/author-7.jpg'
import customer8 from './icons/author-8.jpg'
import quotes from './icons/open.png'
export default {
  components: {
      Swiper,
      SwiperSlide,
    },
  data() {
    return {
      quotes,
      header1: 'TESTIMONIALS',
      header2: 'What They’re Talking About Comapany ?',
      names: ['ALBERT JOE', 'Adam Jumpa', 'Ben Duck', 'Robert Mick', 'Marray joe',],
      text: 'Normal that has evolved from gene ration X is on the runway heading towards a streamlined we normal that has evolved from generation X ...',
      personel: 'Customers',
      img: [customer1, customer3, customer4, customer7, customer8,],
    }
  },
  methods: {
    SwiperSlide() {
      speed: 9000
    }
  }
}
</script>

<style lang="css" scoped>
.text_col {
  color: orangered;
}

.bg {
  background-color: #13203b;
}

* {
  font-family: Roboto, sans-serif;
}

.hr3 {
  display: flex;

}

hr {
  width: 2.5rem;
  height: 2px;
  margin-top: 10px;
  background-color: orangered;
  border: none;
}

h3 {
  color: orangered;
  margin-left: 1rem;
  font-size: 1rem;
  font-weight: 550;

}

.header2 {
  color: white;
  font-size: 2.6rem;
  font-weight: 750;
  margin-top: 1.5rem;
}</style>