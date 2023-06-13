<template>
    <div class="div">
        <div class="blue  btn_div">
            <div class="flex-col">
                <div class="flex-row flex">
                    <hr>
                    <h3>{{ header1 }}</h3>
                </div>
                <h1 class="text-5xl  font-bold  blue mt-8">{{ header2 }}</h1>
            </div>
            <div class="gtext">
             <p class="text">{{ text[0] }}</p>
            <p class="text">{{ text[1] }}</p>   
            </div>
            
        </div>
        <div class=" img_div">
            <img :src="sitesourvayor" alt="" class="rounded-md img">
            <img :src="buildingplan" alt="" class="rounded-md img">
            <img :src="concret" alt="" class="rounded-md img">
            <img :src="completedbuilding" alt="" class="rounded-md img">
            <img :src="road" alt="" class="rounded-md img">
            <img :src="generalContructionImg" alt="" class="rounded-md img">
            <img :src="apartmentbuilding" alt="" class="rounded-md img">
            <img :src="tractor" alt="" class="rounded-md img">
        </div>
        
    </div>
</template>

<script >
import buildingplan from '../icons/gallery-46.jpg'
import sitesourvayor from '../icons/gallery-45.jpg';
import tractor from '../icons/gallery-44.jpg';
import apartmentbuilding from '../icons/gallery-43.jpg'
import generalContructionImg from '../icons/gallery-41.jpg'
import completedbuilding from '../icons/gallery-39.jpg' 
import road from '../icons/gallery-42.jpg'
import concret from '../icons/gallery-40.jpg'
export default {
   
    data() {
        return {
            completedbuilding,
            road,
            concret,
            apartmentbuilding,
            tractor,
            sitesourvayor,
            buildingplan,
            generalContructionImg,
           
            
            header1: 'OUR WORKS',
            header2: 'Explore Recent Projects',
            text: ['We shows only the best websites and portfolios built','completely with passion, simplicity & creativity.']
            
        }
    },
}
</script>

<style lang="css" scoped>
.img_div{
    display: grid;
    grid-template-columns: auto auto;
    row-gap: 50px;
    column-gap: 50px;
    padding: 5rem;
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

.text{
    font-size: large;
}



.blue {
    height: 33rem;
    
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




@media (max-width:1024px) {
    .btn_div{
        display: flex;
        flex-direction:column;
        padding: 1.5rem;
    }
    .img_div{
        display: grid;
        grid-template-columns: auto;
        margin-top: 1rem;
        padding: 1.5rem;
    }
    .blue{
        height: fit-content;
    }
   .gtext{
    margin-top: 2rem;
   }
   
    
}

@media (min-width: 1100px) {
    .btn_div{
        display: flex;
        justify-content: space-between;
    }
}
</style>