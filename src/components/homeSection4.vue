<template>
    <div class="bg">
        <img :src='bgImage' alt='' class=" w-full " style="height:30rem">


        <div class="flex-row ">
            <div class=" bg-white our ml-24 px-12 ">
                <div class='hr3 pt-12 '>
                    <hr>
                    <h3>{{ h3 }}</h3>
                </div>
                <h1 class="text-5xl  font-bold mt-12 blue">{{ our }}</h1>
                <p class="text-xl font-normal mt-12 mb-12">{{ bring }} </p>
                <div v-for="word in words" class="flex -ml-2 mt-5">
                    <img :src="word.img" alt="" class="w-6 h-6">
                    <h1 class='ml-4 text-xl font-medium'>{{ word.text }}</h1>
                </div>
                <div class="flex mt-12 -ml-2">
                    <img :src="contractor" alt="">
                    <div class="ml-12 flex-col">
                        <h1 class="text-md font-bold orangered">{{ call }}</h1>
                        <h1 class='font-bold text-3xl blue hov'>{{ number }}</h1>
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
                <div class='flex-col  ml-10  mt-4 mr-10'>
                    <div class='hr3'>
                        <hr>
                        <h3>{{ 'BIGGER, BETTER, FASTER' }}</h3>
                    </div>
                    <h1 class="text-5xl  font-bold mt-4 text-white">{{ leading }}</h1>
                    <p class='text-xl font-normal mt-6  text-white' >{{ bRing }}</p>
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
            h3: 'OUR KEY POINTS',
            our: 'Why Choose Us',
            bRing:'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved.',
            leading: 'Leading Way In Civil Construction',
            bring: 'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation . Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward.',
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
.bg {
    background-color: rgb(233, 233, 233);
    height: 100rem;
    background-size: cover;
    background-repeat: no-repeat;
}

.play {
    margin-left: 25rem;
}

.our {
    height: 50rem;
    margin-top: -30rem;
    width: 37rem;
    position: absolute;
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

.hr3 {
    display: flex;
}

.hov :hover {
    color: orangered;
}

.hug {
    width: 36rem;
    height: 30rem;
    background-color: #13203b;
    position: absolute;
    margin-left: 43rem;
    margin-top: -10rem;
    

}
</style>