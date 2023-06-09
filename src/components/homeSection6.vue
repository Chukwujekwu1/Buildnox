<template>
    <div class="p-20 pt-0 div flex-row flex justify-between">

        <img :src="roller" alt="" class="walk">

        <div class=" flex-col  p-12 pr-0 pt-0">

            <div class="hr3">
                <hr>
                <h3>{{ header1 }}</h3>
            </div>

            <h1 class="header2">
                {{ header2 }}
            </h1>

            <p class="text-base font-medium mt-5 mb-12 leading-8 ">
                {{ text1 }}
            </p>
          <div class="flex-row flex">
           <div class="flex-col flex">    
            <div class="flex-row flex">
              <img :src="engineer" alt="" class="w-20">
              <div class="flex-col ml-6">
                 <h2 class=" font-bold text-3xl  ">{{ header3 }}</h2>
               <h2 class=" font-bold text-3xl  ">{{ header3c }}</h2>
              </div>
            </div>
            <p class="font-normal text-xl mt-6">{{ text2 }}</p>
           </div>

           <div class="flex-col flex">    
            <div class="flex-row flex ">
              <img :src="hook" alt="" class="w-20">
              <div class="flex-col ml-6">
               <h2 class=" font-bold text-3xl "> {{ header4 }}</h2>
               <h2 class="font-bold text-3xl">{{ header4c }}</h2>
               </div>
            </div>
            <p class="font-normal text-xl mt-6">{{ text2 }}</p>
           </div>
        </div>

        </div>

    </div>

</template>
  
<script>
import roller from './icons/roller.png';
import engineer from './icons/engineer.png';
import hook from './icons/hook.png';
export default {
    data() {
        return {
            roller,
            engineer,
            hook,
            header1: "ABOUT COMPANY",
            header2: 'We Provide the Guaranteed Quality in Construction',
            header3:'Professional ',
            header3c:'Team',
            header4:'Quality ',
            header4c:'Service',
            text1: 'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution. strategies to ensure proactive domination.',
            text2:'Our gutter protection simply works better than any other product.',
        }
    },


}
</script>
  
<style lang="css" scoped>
.div {
    font-family: Roboto, sans-serif;

}

.walk {
    height: 100%;
}



.hr3 {
    display: flex;
    
}

hr {
    width: 2.5rem;
    height: 2px;
    margin-top: 10px;
    background-color: orangered;
    border: none;
}

h3 {
    color: orangered;
    margin-left: 1rem;
    font-size: 1rem;
    font-weight: 550;

}

h2 ,p {
    color: #13203b;
}
.header2 {
    color: #13203b;
    font-size: 2.6rem;
    font-weight: 750;
    margin-top: 1.5rem;
}

</style>