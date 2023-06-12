<template>
  <div class="not">
    <div class="bg">
      <div class="flex flex-col">
        <div class="hr3">
          <hr>
          <h3>{{ header1 }} </h3>
        </div>
        <h1 class="header2">
          {{ header2 }}
        </h1>
        <p class="text">{{ text }}</p>
      </div>




      <div class='central'>
        <div class="div">
          <img :src="img[0]" alt="" class="w-20 h-20">
          <div class="fin">
            <h1 class="num">{{ num[0] }}</h1>
            <p class="text1">{{ text1[0] }}</p>
          </div>
        </div>

        <div class="div">
          <img :src="img[1]" alt="" class="w-20 h-20">
          <div class="fin">
            <h1 class="num">{{ num[1] }}</h1>
            <p class="text1">{{ text1[1] }}</p>
          </div>
        </div>

        <div class="div">
          <img :src="img[2]" alt="" class="w-20 h-20">
          <div class="fin">
            <h1 class="num">{{ num[2] }}</h1>
            <p class="text1">{{ text1[2] }}</p>
          </div>
        </div>

        <div class="div">
          <img :src="img[2]" alt="" class="w-20 h-20">
          <div class="fin">
            <h1 class="num">{{ num[3] }}</h1>
            <p class="text1">{{ text1[0] }}</p>
          </div>
        </div>

      </div>


    </div>
  </div>
</template>

<script>
import model from '../icons/model.png'
import tenant from '../icons/tenant.png'
import certificate from '../icons/certificate.png'
export default {
  data() {
    return {
      img: [certificate, model, tenant, tenant,],
      num: ['2,786', '788', '270', '57',],
      text1: ['Total Projects', 'Qualified Workers', 'Get Awards'],
      header1: 'STATISTICS',
      header2: 'Know More About Our Success',
      text: 'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going for ward, a new normal.'
    }
  }
}
</script>

<style lang="css" scoped>
.bg {
  color: #13203b;
  background-color: #e6e6e6;
  display: flex;
 
  padding: 5rem;
  padding-top: 10rem;
  padding-bottom:10rem;
  justify-content: space-between;
}

* {
  font-family: Roboto, sans-serif;
}
.text{
  font-size: large;
  margin-top: 15px;
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

.header2 {

  font-size: 2.6rem;
  font-weight: 750;
  margin-top: 1.5rem;
}
.fin{
  margin-left: 1rem;
}
.div {
  width: 18rem;
  height: 8rem;
  background-color: white;
  display: flex;
  padding: 1rem;
}

.num {
  font-size: 3rem;
  font-weight: 600;
  color: orangered;
}

.text1 {
  font-size: 1.3rem;
  font-weight: 200;
}

.central {
  display: grid;
  column-gap: 20px;
  row-gap: 20px;
  grid-template-columns: auto auto ;
}

@media (max-width:1050px) {
  .not {
    display: none;
  }
}</style>
  