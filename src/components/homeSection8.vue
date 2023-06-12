<template>
    <div>
        <div class="flex justify-between p-16 brand">
            <img v-for="brand in brands" :src="brand.img" alt="" class="hover:h-9 h-8">
        </div>

        <div class="bg">
            <div class="div">
                <h1 class="font-bold text-2xl">{{ header1 }}</h1>
                <hr class="">
                <p class="mt-12 text-lg font-bold">{{ text }}</p>
                <p class=" font-bold  text-lg">{{ text1 }}</p>
                <p class="mt-10 text-lg font-bold">{{ phone }}</p>
            </div>
        </div>
    </div>
</template>

<script>
import brand1 from './icons/brand-logo-1.png';
import brand2 from './icons/brand-logo-2.png';
import brand3 from './icons/brand-logo-3.png';
import brand4 from './icons/brand-logo-4.png';
import brand5 from './icons/brand-logo-5.png';


export default {
    data() {
        return {
            header1: 'Office Address',
            text: 'PO Box 5849 Collins Street West',
            text1: 'Victoria 9005 Australia',
            phone: 'Phone: +1800-456-7890',
            brands: [{ img: brand1 }, { img: brand2 }, { img: brand3 }, { img: brand4 }, { img: brand5 }]
        }
    },
}
</script>

<style lang="css" scoped>
* {
    color: white;
}

hr {
    width: 1.7rem;
    height: 2px;
    margin-top: 0.5rem;
    background-color: white;
    border: none;
}

.div {
    background-color: #01609d;
    height: 25rem;
    padding: 4rem;
    width:24rem;
    
    flex-direction: column;
    
}
.bg{
    background-image: url('./icons/map.png');
    width: 100%;
    height: 25rem;
    display: flex;
    justify-content: end;
    padding-right: 5rem;
   
}

@media (max-width:1024px) {
    .brand{
        display: none;
    }
    .bg{
      display: flex;
      padding: 1.5rem;
      padding-top: 0;
    }
}


</style>