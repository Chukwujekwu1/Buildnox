<template>
  <div class="div">

    <img :src="walk" alt="" class="walk">

    <div class=" flex-col divv">

      <div class="hr3">
        <hr>
        <h3>{{ h3 }}</h3>
      </div>

      <h1 class="con">
        {{ con }}<span class="bus"> {{ bus }} </span>
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

        <div class="signature">
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
  
  padding: 5rem;
  
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  font-family: Roboto, sans-serif;
  color: white;

}

.walk {
  height: 80%;
}

.signature{
  margin-left:8rem ;
}

.hr3 {
  display: flex;
  margin-top: 3rem;
  
  padding-top: 0;
}

.divv{
  margin-left: 4rem;
}

hr {
  width: 2.5rem;
  height: 2px;
  margin-top: 10px;
  background-color: rgb(255, 85, 24);
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
  margin-left: 10px;

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
}


@media (max-width:1024px) {
  .div{
    display: flex;
    flex-direction: column; 
    padding: 1.5rem;
    padding-top: 0;
  }
  .hr3{
    color:black;
    padding: 0;
  }
  .con{
    font-size: 1.9rem;
    font-weight: 600;
  }
  .we{
    font-size: 1.2rem;

  }
  .for{
    font-size: 1.2rem;
  }
  .fS{
    display: flex;
    flex-direction:column;
  }
  .signature{
    margin-left: 0;
    margin-top: 2rem;
  }
  .divv{
    margin-left: 0;
  }
}
</style>