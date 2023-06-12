<template>
    <div class='main'>
        <div class="bg">



            <div class=" div">
                <div class=" our ">
                    <div class='hr3 '>
                        <hr>
                        <h3>{{ header1 }}</h3>
                    </div>
                    <h1 class="header2 blue">{{ header2 }}</h1>
                    <p class="text1">{{ text1 }} </p>
                    <div v-for="word in words" class="word">
                        <img :src="word.img" alt="" class="word_img">
                        <h1 class='word_text'>{{ word.text }}</h1>
                    </div>
                    <div class="contractor_div">
                        <img :src="contractor" alt="">
                        <div class="call_div">
                            <h1 class=" text-md call orangered">{{ call }}</h1>
                            <h1 class=' blue hov'>{{ number }}</h1>
                        </div>
                    </div>
                </div>

                <div class="hug">
                    <div class="  flex-col">
                        <div class=" justify-center w-40 bg-red-500 h-36 -mt-16 play items-center flex">
                            <div
                                class="w-28 h-28 bg-green-400 mx-auto my-auto rounded-full  justify-center items-center flex  bg-transparent border-white-100 border-8 hover:bg-white hover:border-blue-950">
                                <img :src="play" alt="" class="w-16 h-16 animate-none">
                            </div>
                        </div>
                    </div>
                    <div class='flex-col   cla mt-28 mr-10'>
                        <div class='hr3'>
                            <hr>
                            <h3>{{ Header1 }}</h3>
                        </div>
                        <h1 class="text-5xl  font-bold mt-4 text-white">{{ Header2 }}</h1>
                        <p class='text-xl font-normal mt-6  text-white'>{{ Text1 }}</p>
                    </div>
                </div>


            </div>
            
        </div>
    </div>
   
</template>

<script >
import bgImage from './icons/bg-1.jpg'
import check from './icons/check-circle.png'
import contractor from './icons/contractor-2.jpg'
import play from './icons/play.png'

export default {
    data() {
        return {
            bgImage,
            check,
            contractor,
            play,
            call: 'CALL FOR CONTRACTOR NOW',
            number: '+1800-(676)-5432',
            header1: 'OUR KEY POINTS',
            header2: 'Why Choose Us',
            Header1: 'BIGGER, BETTER, FASTER',
            Text1: 'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved.',
            Header2: 'Leading Way In Civil Construction',
            text1: 'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation . Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward.',
            words:
                [
                    {
                        text: 'Experienced Construction Professional',
                        img: check
                    },
                    {
                        text: 'Committted to Helping Our Clients',
                        img: check
                    },
                    {
                        text: 'Building Maintenance & Renovation',
                        img: check
                    },
                    {
                        text: 'Innovative Eco Power Technologies',
                        img: check
                    }
                ]
        }

    }
}
</script>

<style lang="css" scoped>
.cla{
    margin-left: -32rem;
}
.call{
    font-weight: 700;
}
.call_div {
    flex-direction: column;
    display: flex;
    margin-left: 3rem;
}

.contractor_div {
    margin-left: -0.5rem;
    margin-top: 3rem;
    display: flex;
}

.word_text {
    font-size: 1.25rem;
    line-height: 1.75rem;
    margin-left: 1rem;
    font-weight: 500;
}

.word {
    margin-left: -0.5rem;
    margin-top: 1.25rem;
    display: flex;
}

.word_img {
    height: 1.5rem;
    width: 1.5rem;
}

.text1 {
    margin-bottom: 3rem;
    margin-top: 3rem;
    font-weight: 400;
    font-size: 1.25rem;
    line-height: 1.75rem;
}

.header2 {
    font-size: 3rem;
    line-height: 1;
    font-weight: 700;
    margin-top: 3rem
}



.bg {
    background-image: url('./icons/bg-1.jpg');
    width: 100%;
    height: 30rem;
    background-size: cover;
    background-repeat: no-repeat;
    margin-top:-14rem;
    padding:6rem ;
    padding-top: 0;
}

.div {
    
    display:inline;
    flex-direction:row;
}

.play {
    margin-left: 25rem;
   
}

.our {
    height: 50rem;
    
    width: 36rem;
    
    background-color: white;
    padding: 2rem;

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
.main{
    background-color: rgb(218, 218, 218);
    height: 60rem;
    margin-top: 13rem;
    
}
.hr3 {
    display: flex;
}

.hov{
    font-size: 1.875rem;
    line-height: 2.25rem;
    font-weight: 700;
}
.hov :hover {
    color: orangered;
}

.hug {
    width: 36rem;
    height: 30rem;
    background-color: #13203b;
    
    margin-left: 36rem;
    margin-top: -30rem;

  display: flex;

}

@media (max-width:1024px) {
    .main{
        display: none;
    }
}
</style>