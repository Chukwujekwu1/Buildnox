<template>
    <div class='main'>
        <div class="bg">

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
                        <h1 class="text-5xl  font-bold mt-4 text-white header2">{{ Header2 }}</h1>
                        <p class='text-xl font-normal mt-6  text-white text1'>{{ Text1 }}</p>
                    </div>
                </div>


            
            
        </div>
    </div>
   
</template>

<script >
import bgImage from '../icons/bg-1.jpg'
import check from '../icons/check-circle.png'
import contractor from '../icons/contractor-2.jpg'
import play from '../icons/play.png'

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



.bg {
    background-image: url('../icons/bg-1.jpg');
    width: 100%;
    height: 30rem;
    background-size: cover;
    background-repeat: no-repeat;
    padding:6rem ;
    padding-top: 0;
}



.play {
    margin-left: 25rem;
   
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


.hug {
    width: 36rem;
    height: 30rem;
    background-color: #13203b;
    
  display: flex;

}

@media (max-width:1024px) {
    .bg{
        padding: 1.5rem;
        padding-top: 0;
        display: flex;
        justify-content: center;
    }
    .hug{
        width: 100%;
        padding: 2rem;
        padding-top: 3rem;
        
    }
    .play{
      display: none;
    }
    .cla{
        margin-left: 0;
        margin-top: 0;
        margin-right: 0;
    }
    .header2{
        font-size: 2rem;
        margin-top: 2.5rem;
    }
    .text1{
        margin-top: 2rem;
        line-height: 2.5rem;
    }
}

</style>