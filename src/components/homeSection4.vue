<template>
    <div class="bg ">
    </div>
    <div class="">

        <div class=" bg-white our ml-20 px-12 rounded-lg">
            <div class='hr3 pt-12 '>
                <hr>
                <h3>{{ h3 }}</h3>
            </div>
            <h1 class="text-5xl  font-bold mt-12" >{{ our }}</h1>
            <p class="text-xl font-normal mt-12 mb-12">{{ bring }} </p>
            <div v-for="word in words" class="flex -ml-2 mt-5" >
                <img :src="word.img" alt="" class="w-6 h-6">
                <h1 class='ml-4 text-xl font-medium'>{{ word.text }}</h1>
            </div>
            

        </div>
    </div>
</template>

<script >
import bgImage from './icons/bg-1.jpg'
import check from './icons/check-circle.png'
export default {
    data() {
        return {
            bgImage,
            check,
            h3: 'OUR KEY POINTS',
            our: 'Why Choose Us',
            bring:'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation . Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward.',
            words:
            [
              {
                text:'Experienced Construction Professional',
                img: check
              },
              {
                text:'Committted to Helping Our Clients',
                img: check
              },
              {
                text:'Building Maintenance & Renovation',
                img:check
              },
              {
                text:'Innovative Eco Power Technologies',
                img: check
              }
            ]
        }

    }
}
</script>

<style lang="scss" scoped>
.bg {
    background-image: url('./icons/bg-1.jpg');
    height: 30rem;
    background-size: cover;
    background-repeat: no-repeat;
}

.our {
    height: 50rem;
    margin-top: -30rem;
    width: 35rem;

    .hr3 {
        display: flex;

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

        ;

    }
}</style>