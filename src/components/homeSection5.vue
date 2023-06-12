<template>
    <div class="div">
        <div class="blue  btn_div">
            <div class="flex-col">
                <div class="flex-row flex">
                    <hr>
                    <h3>{{ header1 }}</h3>
                </div>
                <h1 class="text-5xl  font-bold  text-white mt-8">{{ header2 }}</h1>
            </div>
            <button @click.prevent=""
                class="  bg-red-500  anim"> {{ btntext }}</button>
        </div>
        <div class=" img_div">
            <img :src="roofImg" alt="" class="rounded-md img">
            <img :src="buildImg" alt="" class="rounded-md img">
            <img :src="generalContructionImg" alt="" class="rounded-md img">
        </div>
        <swiper :slides-per-view="1" :space-between="50" @swiper="onSwiper" @slideChange="onSlideChange"  :autoplay='{
            delay: 3500,
            disableOnInteraction: false,}' class="pad mySwiper">
            <swiper-slide class="text1">{{ text1 }}</swiper-slide>
            <swiper-slide class="text1">{{ text1 }}</swiper-slide>
            ...
        </swiper>
    </div>
</template>

<script >
import SwiperCore, {Autoplay} from 'swiper/core';
SwiperCore.use(Autoplay);
import 'swiper/css';
import { Swiper, SwiperSlide } from 'swiper/vue';
import roofImg from '../components/icons/gallery-1.jpg';
import buildImg from '../components/icons/gallery-2.jpg';
import generalContructionImg from '../components/icons/gallery-3.jpg';
 
export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    data() {
        return {
            roofImg,
            buildImg,
            generalContructionImg,
            text1: 'TECHNOLOGY CIVIL',
            header1: 'OUR WORKS',
            header2: 'Explore Recent Projects',
            btntext: 'VIEW ALL PROJECTS',
        }
    },
    methods:{
        SwiperSlide(){
            speed:3000
        }
    }
}
</script>

<style lang="css" scoped>
.img_div{
    justify-content: space-between;
    display: flex;
    flex-direction: row;
    padding: 1.5rem;
    padding-top: 0rem;
    margin-top: -18rem/* -288px */;
}
.btn_div{
    padding: 5rem;
    display: flex;
    flex-direction: row;
    
}
.div {
    margin-top: -0.7rem;
}

.text1 {
    -webkit-text-stroke-width: 2px;
    -webkit-text-stroke-color: rgba(173, 167, 167, 0.6);
    color: transparent;
    font-size: 9rem;
}

img {
    width: 26.3rem;
    height: 25rem;
}

.blue {
    height: 33rem;
    background-color: #13203b;
}

h3 {
    color: orangered;
    margin-left: 1rem;
    font-family: Roboto, sans-serif;
    font-size: 1rem;
    font-weight: 550;

}

hr {
    width: 2.5rem;
    height: 2px;
    margin-top: 10px;
    background-color: orangered;
    border: none;
}

.anim {
    font-family: Roboto, sans-serif;
    font-size: 1rem;
    font-weight: 550;
    transition: 0.9s;
    border-radius: 8px;
    height: 5rem;
    width: 18rem;
    margin-top:2rem ;
    text-align: center;

}

.anim:hover {
    background-color: rgb(11, 11, 39);
    color: white
}

.pad {
    padding: 2.5rem;
    padding-top: 0rem;
    margin-top: -2rem;
}


@media (max-width:1024px) {
    .btn_div{
        display: flex;
        flex-direction:column;
        padding: 1.5rem;
    }
    .img_div{
        display: flex;
        flex-direction: column;
        margin-top: -9rem;
    }
    .img{
        margin-top: 1.5rem;
    }
    .pad{
        display: none;
    }
    .anim{
        margin-top: 3rem;
    }
}

@media (min-width: 1100px) {
    .btn_div{
        display: flex;
        justify-content: space-between;
    }
}
</style>