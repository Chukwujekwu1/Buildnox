<template>
    <div class='main'>
        



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
                <img :src="work_img" alt="" class="work_img">
            </div>
            
        </div>
    
   
</template>

<script >
import check from '../icons/check-circle.png'
import contractor from '../icons/contractor-2.jpg'
import work_img from '../icons/image-25.jpg'
export default {
    data() {
        return {
            check,
            work_img,
            contractor,
            call: 'CALL FOR CONTRACTOR NOW',
            number: '+1800-(676)-5432',
            header1: 'OUR KEY POINTS',
            header2: 'Why Choose Us',
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





.div {
    padding: 5rem;
    padding-bottom: 0rem;
    display:flex;
    justify-content: space-between;
}


.our {
    height: 50rem;
    width: 36rem;
    
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
    background-color:#F1F4FB;
    height: 57rem;
   
    
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

@media (max-width:1024px) {
    .div{
        display:flex;
        flex-direction: reverse-column;
    }
}
</style>