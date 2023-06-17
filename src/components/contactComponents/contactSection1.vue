<template>
    <div class="div ">
        <div class="blue  btn_div">
            <div class="flex-col">
                <div class="flex-row flex">
                    <hr>
                    <h3 class="header1">{{ header1 }}</h3>
                </div>
                <h1 class="text-5xl  font-bold   mt-8">{{ header2 }}</h1>
            </div>
        </div>
        <div class="sub_div">
            <div class="img_div">
                <input type="name" placeholder="Your Name">
                <input type="email" placeholder="Your Email">
                <input type="text" placeholder="Subject">
                <input type="text" placeholder="Message" style=" height: 7rem;">
                <button class='btn'> submit</button>
            </div>
            <div class="div_sub">
                <h1 class="Header1">{{ Header1 }}</h1>
                <p class="text1 mt-5">{{ text1 }}</p>

                <div class="">
                    <div class="flex-row flex mt-6">
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

            </div>




        </div>
    </div>
</template>

<script >
import location from '../icons/pin.png';
import email from '../icons/email.png';
import phone from '../icons/telephone.png'

export default {
    data() {
        return {
            location,
            email,
            phone,
            h3_1: 'Address :',
            p_1: '54B, Tailstoi Town 5238 MT, La city, IA 5224',
            h3_2: 'Phone :',
            p_2: '1800-456-7890',
            h3_3: 'Email :',
            p_3: 'buildnox@gmail.com',
            Header1: 'Our Address',
            text1: 'Completely synergize resource taxing relationships via premier niche markets. Professionally cultivate one-to-one customer service.',
            header1: 'GET IN TOUCH',
            header2: 'We Would Love To Hear From You',
            btntext: 'VIEW ALL PROJECTS',
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
.div_sub{
    margin-top: -19rem;
    margin-left: 4rem;
}

.h3_class{
    font-size: 1.5rem;
    color: #13203b;
    font-weight: 700;
}
.sub_div {
    display: flex;
    flex-direction: row;
    padding: 4rem;
    padding-top: 0rem;
}

.text1 {
    font-size: large;
    line-height: 2rem;
    color: #13203b;
}

.Header1 {
    font-weight: 600;
    font-size: 2rem;
}


h1 {
    color: #13203b;
}

.img_div {

    display: flex;
    flex-direction: column;


    margin-top: -20rem
        /* -288px */
    ;
}

.btn_div {
    padding: 5rem;
    display: flex;
    flex-direction: row;

}

.div {

    background-color:aliceblue;

}

input {
    width: 40rem;
    height: 4rem;
    border: 0.5px solid grey;
    padding: 1rem;
    margin-top: 2rem;
}

.blue {
    height: 33rem;

}

.header1 {
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

.btn {
    height: 3rem;
    width: 12rem;
    background-color: rgb(255, 30, 0);
    margin-top: 2rem;
}

.icon {
    height: 3rem;
    width: 3rem;
}


@media (max-width:1024px) {
    .btn_div {
        display: flex;
        flex-direction: column;
        padding: 0rem;
        padding-top: 3rem;
        margin-bottom: 3rem;
    }

    .img_div {
        display: flex;
        flex-direction: column;
        

    }
   .sub_div{
    display: flex;
    flex-direction: column;
    padding:0;
   }
   input{
    width: 100%;
   }
   .div_sub{
    margin-top: 1rem;
    margin-left: 0rem;
   }
   .div{
    padding: 1.5rem;
   }

}
</style>