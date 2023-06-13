<template>
    <div class="flex-row div">
        <div class='hr3'>
            <hr>
            <h3>{{ h3 }}</h3>
        </div>
        <h1 class="our">{{ our }}</h1>
        <p class="iF">{{ iF }}</p>
        <ul class="img_div">
            <li v-for="image in images" :key="image.id" class="images">
                <img :src="image.src" alt="" style="width:6rem">
                <h1 class="text text-3xl font-bold">{{ image.text }}</h1>
                <h1 class="text1 text-3xl font-bold">{{ image.text1 }}</h1>
                <img :src="image.workPics" alt="" class="workpics">
            </li>
        </ul>
        <p style="height: 6rem;"></p>
    </div>
</template>

<script>
import roof from '../icons/roof.png';
import sketch from '../icons/sketch.png';
import service from '../icons/service-1.jpg';
import construction from '../icons/construction.png';
import plan from '../icons/image-26.jpg';
import roofing from '../icons/image-28.jpg'
import renovation from '../icons/renovation.png'
import renovationImg from '../icons/image-27 (1).jpg'
import interior from '../icons/interior-design.png'
import interiorImg from '../icons/image-29.jpg'
import building from '../icons/building.png'
import buildingImg from '../icons/image-30.jpg'
import consulting from '../icons/engineer (1).png'
import consultingImg from '../icons/image-31.jpg'
import maintenance from '../icons/maintenance.png'
import maintenanceImg from '../icons/image-32.jpg'
export default {
    data() {
        return {
            service,
            h3: 'WHAT WE DO',
            our: 'Our Services That We Provide',
            iF: 'If you need to repair or replace your Plumbing system, call today and talk to one of our Plumbing specialists. They’ll answer all your questions and arrange an appointment at your convenience.',
            images: [
                {
                    text: 'Flooring',
                    text1: '& Roofing',
                    src: roof,
                    id: 1000,
                    workPics: roofing
                },
                {
                    text: 'Archetecture',
                    text1: 'Design',
                    src: sketch,
                    id: 2000,
                    workPics: plan
                },
                {
                    text: 'Building',
                    text1: 'Construction',
                    src: construction,
                    id: 3000,
                    workPics: service
                },
                {
                    text: 'Building',
                    text1: 'Renovation',
                    src: renovation,
                    id: 4000,
                    workPics: renovationImg
                },
                {
                    text: 'Interior',
                    text1: 'Design',
                    src: interior,
                    id: 5000,
                    workPics:interiorImg
                },
                {
                    text: 'Repair',
                    text1: 'And Expand',
                    src: building,
                    id: 6000,
                    workPics: buildingImg
                },
                {
                    text: 'Construction',
                    text1: 'Consulting',
                    src: consulting,
                    id: 7000,
                    workPics: consultingImg
                },
                {
                    text: 'Building',
                    text1: 'Maintenance',
                    src: maintenance,
                    id: 8000,
                    workPics: maintenanceImg
                },
            ]
        }
    }
}
</script>

<style lang="css" scoped>
.div {
    padding: 6rem;
    padding-top: 5rem;
    background-color: rgb(218, 218, 218);
}
.images{
    display: flex;
    flex-direction: column;
}
.img_div{
    display: grid;
    grid-template-columns: auto auto auto auto;
    row-gap: 3rem;
}

.hr3 {
    display: flex;

}

h3 {
    color: orangered;
    margin-left: 0.75rem;
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



.our {
    
    font-size: 2.6rem;
    font-weight: 750;
    margin-top: 3rem;
    color: #13203b;
}

.iF {
    width: 55rem;
    
    font-size: 1.2rem;
    margin-top: 2rem;
    line-height: 2rem;
}

ul {
    display: flex;
    justify-content: space-between;
    margin-top: 3.5rem;
}

li {

    padding: 43px 35px 0;
    height: fit-content;
    width: 17rem;
    background: #fff;
    list-style: none;
    color: #13203b;
    border-radius: 8px;

}

li:hover {
    background-color: #13203b;
    color: #fff;
    transition: .9s;

}


.text {
    margin-top: 1.5rem;
}

.workpics {
    width: 18rem;
    margin-top: 2rem;
    margin-bottom: 2rem;
   
}

@media (max-width:1024px) {
   
    .img_div{
        display: flex;
        justify-content: center;
        flex-direction: column;
        margin-top:2rem ;
    }
    .div{
        padding: 1.5rem;
    }
    .iF{
        width: 100%;
    }
}


</style>