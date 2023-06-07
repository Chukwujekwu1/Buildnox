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
            <p class="text-xl font-normal mt-12">{{ bring }}</p>
        </div>
    </div>
</template>

<script >
import bgImage from './icons/bg-1.jpg'
export default {
    data() {
        return {
            bgImage,
            h3: 'OUR KEY POINTS',
            our: 'Why Choose Us',
            bring:'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation . Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward.'
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