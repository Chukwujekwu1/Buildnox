<template>
    <div class="div blue">
        <div class="blue  btn_div">
            <div class="flex-col">
                <div class="flex-row flex">
                    <hr>
                    <h3>{{ header1 }}</h3>
                </div>
                <h1 class="text-5xl  font-bold   mt-8">{{ header2 }}</h1>
            </div>
        </div>
        <div class="img_div">
            <img :src="team1" alt="" class="rounded-md img">
            <img :src="team2" alt="" class="rounded-md img">
            <img :src="team3" alt="" class="rounded-md img">
            <img :src="team4" alt="" class="rounded-md img">
        </div>
    </div>
</template>

<script >
import team1 from '../icons/team-1.jpg';
import team2 from '../icons/team-2.jpg';
import team3 from '../icons/team-3.jpg';
import team4 from '../icons/team-4.jpg';
 
export default {
    
    data() {
        return {
            team1,
            team2,
            team3,
            team4,
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
h1{
    color:#13203b; 
}

.img_div{
    justify-content: space-between;
    display: flex;
    flex-direction: row;
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
  background-color: rgb(253, 253, 253);
  
}



.img {
    width: auto;
    height: auto;
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
        display: flex;
        flex-direction: column;
        margin-top: -9rem;
    }
    .img{
        margin-top: 1.5rem;
    }
    
}


</style>