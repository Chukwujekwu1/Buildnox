<template>
    <div>
        <div class='hr3'>
            <hr>
            <h3>{{ h3 }}</h3>
        </div>
       <h1 class="our" >{{ our }}</h1>
       <p class="iF">{{ iF }}</p>
      <ul >  
     <li v-for="image in images" :key="image.id" >
        <img :src="image.src" alt="" style="width:6rem" >
        <h1 class="text text-3xl font-bold">{{ image.text }}</h1>
        <h1 class="text1 text-3xl font-bold" >{{ image.text1 }}</h1>
        <img :src="image.workPics" alt="" class="workpics">
     </li>
    </ul>
    <p style="height: 10rem;"></p>
    </div>
</template>

<script >
import  roof from './icons/roof.png';
import sketch from './icons/sketch.png';
import service from './icons/service-1.jpg';
import construction from './icons/construction.png';
import plan from './icons/image-26.jpg';
import  roofing from './icons/image-28.jpg'

export default{
    data(){
        return{
        service,
        h3:'WHAT WE DO',
        our:'Our Services That We Provide',
        iF:'If you need to repair or replace your Plumbing system, call today and talk to one of our Plumbing specialists. They’ll answer all your questions and arrange an appointment at your convenience.',
        images:[
            {
             text:'Flooring',
             text1:'& Roofing',
             src: roof,
             id:1000,
             workPics: roofing
            },
            {
             text:'Archetecture',
             text1: 'Design',
             src: sketch,
             id:2000,
             workPics:plan
            },
            {
             text:'Building',
             text1:'Construction',
             src: construction,
             id:3000,
             workPics: service
            },
        ]
        }
    }
}
</script>

<style lang="scss" scoped>
div{ 
    padding-left: 3rem;
    padding-right: 3rem;
    padding-top: 4rem;
    background-color: rgb(219, 219, 219);
    
    .hr3{
    display:flex;
   
    h3{
        color:orangered;
        margin-left: 1rem;
        font-family: Roboto, sans-serif;
        
    }
    hr {
        width: 2.5rem;
        height: 2px;
        margin-top: 10px;
        background-color: orangered;
        border: none;
      }

    }
    .our{
        margin-left:2.6rem;
        font-size:2.6rem;
        font-weight: 750;
        margin-top: 3rem;
        color:#13203b;
    }
    .iF{
        width: 55rem;
        margin-left: 2.6rem;
        font-size: 1.2rem;
      margin-top: 2rem;
      line-height: 2rem;
    }
    ul{
        display: flex;
        justify-content: space-between;
        margin-top: 3.5rem;
        margin-left: 2rem;
        margin-right: 2rem;

       
      li{

        &:hover{
            background-color: #13203b;
            color: #fff;
            transition: .9s ;
            
        }
        padding: 43px 35px 0;
        height:20rem;
        width:20rem;
        background: #fff;
        list-style: none;
        color:#13203b;
        border-radius: 8px;
        .text{
            margin-top: 1.5rem;
        }
        .workpics{
            width: 18rem;
             margin-top: 2rem;
             background-color: transparent;
             &:hover{
                background-color: red;
                transition: 0.9s;
             }
        }
      }
    }
}
</style>