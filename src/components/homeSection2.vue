<template>
  <div class="p-20 pt-0 div flex-row flex justify-between">

    <img :src="walk" alt="" class="walk">

    <div class=" flex-col  p-20 pr-0">

      <div class="hr3">
        <hr>
        <h3>{{ h3 }}</h3>
      </div>

      <h1 class="con">
        {{ con }}<span class="bus ml-4"> {{ bus }} </span>
      </h1>

      <p class="we">
        {{ we }}
      </p>

      <p class="for">
        {{ for }}
      </p>

      <div class="fS">

        <div class="foundee">

          <img :src="author" alt="" class="author">

          <div class="ro">

            <h2>{{ rob }}</h2>
            <p>{{ founder }}</p>

          </div>

        </div>

        <div class="ml-32">
          <img :src="signature" alt="">
        </div>

      </div>

    </div>
    <p class="bottom">

    </p>

  </div>
</template>

<script>
import walk from './icons/image-3.png';
import author from './icons/author-1.jpg';
import signature from './icons/signature.png';
export default {
  data() {
    return {
      walk,
      author,
      signature,
      h3: "WELCOME TO COMPANY",
      con: 'Construction Company With Strategy In',
      bus: 'Business Growth',
      we: ' We have been the trusted name in heating, air conditioning and plumbing businesses. Throughout the years, our number one goal',
      for: ' For over 80 years, We have been the trusted name in heating, air conditioning and plumbing businesses. Throughout the years, our number one goal has been to accurately . For over 80 years, We have been the trusted name in heating, air conditioning and plumbing businesses. Throughout the years, our number one goal has been to accurately .For over 80 years, We have been the trusted name in heating.',
      rob: 'Robert Joe Kerry',
      founder: 'Founder',
    }
  },


}
</script>

<style lang="css" scoped>
.div {

  background-color: #13203b;
  
  font-family: Roboto, sans-serif;
  color: white;

}

.walk {
  height: 80%;
}



.hr3 {
  display: flex;
  margin-top: 2rem;
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


.con {
 
  font-size: 2.6rem;
  font-weight: 750;
  margin-top: 3rem;
}

.bus {
  font-weight: 20;
  font-size: 2rem;

}

.we {
  
  font-size: 1.5rem;
  margin-top: 3rem;
  line-height: 2.5rem;
}

.for {
 
  font-size: 1.2rem;
  margin-top: 2rem;
  line-height: 2rem;
}

.fS {
  
  margin-top: 1.7rem;
  display: flex;
  
}

.foundee {
  display: flex;
}

.author {
  border-radius: 360%;
}

.ro {
  margin-top: 1rem;
  margin-left: 1rem;
}

.bottom {
  height: 7rem;
}

p {
  margin-top: 10px;
}</style>