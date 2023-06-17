<template>
    <div class="main">
           <div class=" div">
                    <div class="flex-row flex mt-6  contact-div">
                        <img :src="location" alt="" class="icon">
                        <div class=" flex-col flex ml-4">
                            <h3 class="h3_class">{{ h3_1 }}</h3>
                            <p class="text1">{{ p_1 }}</p>
                        </div>
                    </div>
                    <div class="flex-row flex  mt-6 ">
                        <img :src="email" alt="" class="icon">
                        <div class="  flex-col flex ml-4">
                            <h3 class="h3_class">{{ h3_2 }}</h3>
                            <p class="text1">{{ p_2 }}</p>
                        </div>
                    </div>
                    <div class="flex-row flex  mt-6">
                        <img :src="phone" alt="" class="icon">
                        <div class="  flex-col flex ml-4">
                            <h3 class="h3_class">{{ h3_3 }}</h3>
                            <p class="text1">{{ p_3 }}</p>
                        </div>
                    </div>
                </div>

                <hr>


                <div class="final">

                    <div>
                        <img :src="logo" alt="">
                        <p class="text2 w-80">{{ text2 }}</p>
                    </div>
                    
                    <div>
                        <h1 class="header">{{ header3 }}</h1>
                        <p class="text3"><a :href="link.path" v-for="link in links" class="flex flex-col text-2xl">{{ link.text }}</a></p>
                    </div>
                    


                    <div>
                        <h1 class="header">{{ header4 }}</h1>
                        <h2 class="text3">{{ text3 }}</h2>

                        <div class="flex flex-row mt-4">
                            <input type="mail" placeholder="Enter your email address" >
                            <button><img :src="send" alt="" class="send"></button>
                        </div>

                        <div class="flex flex-row mt-4">   
                            <img :src="social[0]" alt="" class="social">
                            <img :src="social[1]" alt="" class="social ml-4">
                            <img :src="social[2]" alt="" class="social ml-4">
                            <img :src="social[3]" alt="" class="social ml-4">
                        </div>
                    </div>
                </div>

              <hr>  
    </div>
</template>

<script>
import location from './icons/pin.png';
import email from './icons/email.png';
import phone from './icons/telephone.png';
import logo from './icons/logo-light (1).png';
import send from './icons/paper-plane.png';
import google from './icons/google.png';
import twitter from './icons/twitter.png';
import facebook from './icons/facebook.png';
import linkedin from './icons/linkedin.png'
export default {
    data() {
        return {
            location,
            email,
            phone,
            logo,
            send,
            social:[google, twitter,facebook,linkedin],  

            Header1: 'Our Address',
            text1: 'Completely synergize resource taxing relationships via premier niche markets. Professionally cultivate one-to-one customer service.',
            header1: 'GET IN TOUCH',
            header2: 'We Would Love To Hear From You',
            header3:'Useful Links',
            header4:'Newsletter',
            text3:'Get latest updates and offers.',
            text2:'Capitalize on low hanging fruit to identify a ballpark value added activity to beta test a the ballpark value added activity to beta test.',
            h3_1: 'Address :',
            p_1: '54B, Tailstoi Town 5238 MT, La city, IA 5224',
            h3_2: 'Phone :',
            p_2: '1800-456-7890',
            h3_3: 'Email :',
            p_3: 'buildnox@gmail.com',
            links:[ 
                {
                    text:'Home',
                    path: '/'
                },
                {
                    text:'About',
                    path: '/about'
                },
                {
                    text:'Contact',
                    path: '/contact'
                },
                {
                    text:'Project',
                    path: '/project'
                },
                {
                    text:'Team',
                    path: '/team'
                },
                {
                    text:'Services',
                    path: '/services'
                },
              ],
        }
    },
    methods: {
        SwiperSlide() {
            speed: 3000
        }
    }
}
</script>

<style lang="css" scoped>
.final{
    justify-content: space-between;
    display: flex;
    margin-top: 2.5rem;
    flex-direction: row;
}



.social{
    height:3rem;
    width: 3rem;
    border-radius: 360px;
}
.social:hover{
    background-color:rgb(255, 53, 2) ;
}
button{
    height: 3rem;
    width: 4rem;
    background-color:rgb(206, 41, 0);
    justify-content: center;
    align-items: center;
    display: flex;
    border-top-right-radius: 8px;
    border-bottom-right-radius: 8px;
}
button:hover{
    background-color: rgb(1, 1, 36);
}
.send{
    width: 1.5rem;
    height: 1.5rem;
   
}
input{
    background-color: transparent;
    height: 3rem;
    width: 15rem;
    border-bottom-left-radius: 8px;
    border-top-left-radius: 8px;
    padding: 1.5rem;
    padding-bottom: 0;
    padding-top: 0;
    color: #8e939f;
    border: 0.5px solid #8e939f ;
    outline: none;
    
}


.header{
    font-size: 2rem;
    font-weight: 600;
}
.text2{
    color: #8e939f;
    margin-top: 2rem;
    font-size: large;
}
.text3{
    color: #8e939f;
    font-size: larger;
    margin-top: 1rem;
}
hr{
    width: 100%;
    margin-top: 2rem;
}
 .h3_class{
    font-size: 1.5rem;
   
    font-weight: 700;
}
.main{
    background-color: #13203b;
    color: white;
    padding: 5rem;
    padding-top: 0;
}

.text1 {
    font-size: large;
    line-height: 2rem;
    
}
.icon {
    height: 3rem;
    width: 3rem;
}
.div{
    display: flex;
    flex-direction: row;
}






@media (max-width: 1024px) {
    .div{
        display: flex;
        flex-direction: column;
    }
    .final{
        display: flex;
        flex-direction: column;
    }
    input{
        width:85%;
    }
    .main{
        padding: 1.5rem;
        padding-top: 0;
    }
}





@media (min-width:1100px) {
    .div{
        justify-content: space-between;
    }
}
</style>