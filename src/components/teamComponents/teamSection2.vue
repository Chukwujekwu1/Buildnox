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
            <img :src="team5" alt="" class="rounded-md img">
            <img :src="team6" alt="" class="rounded-md img">
            <img :src="team7" alt="" class="rounded-md img">
            <img :src="team8" alt="" class="rounded-md img">
            
        </div>
    </div>
</template>

<script >
import team1 from '../icons/team-1.jpg';
import team2 from '../icons/team-2.jpg';
import team3 from '../icons/team-3.jpg';
import team4 from '../icons/team-4.jpg';
import team5 from '../icons/team-11.jpg';
import team6 from '../icons/team-12.jpg';
import team7 from '../icons/team-13.jpg';
import team8 from '../icons/team-14.jpg';
 
export default {
    
    data() {
        return {
            team1,
            team2,
            team3,
            team4,
            team5,
            team6,
            team7,
            team8,
            text1: 'TECHNOLOGY CIVIL',
            header1: 'OUR PROFESSIONALS',
            header2: 'Our Dedicated Team',
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
    
    display: grid;
    grid-template-columns: auto auto auto auto;
    row-gap: 2rem;
    column-gap: 2rem;
    padding: 5rem;
    padding-top: 0rem;
    padding-bottom: 9rem;
    
}
.btn_div{
    padding: 5rem;
    display: flex;
    flex-direction: row;
    
}
.div {
    
  background-color: rgb(214, 214, 214);
  
}



.img {
    width: auto;
    height: auto;
}

.blue {
    height: fit-content;
    
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
        padding-top: 3rem;
        margin-bottom: 3rem;
    }
    .img_div{
        display: flex;
        flex-direction: column;
        padding: 1.5rem;
      
    }
    .img{
        margin-top: 1.5rem;
    }
    
}


</style>