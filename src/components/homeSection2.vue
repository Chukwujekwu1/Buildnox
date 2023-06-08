<template>
  <div>

    <img :src="walk" alt="" class="walk" >

    <div class="htext flex-col">

      <div class="hr3">
        <hr>
        <h3 >{{ h3 }}</h3>
      </div>

      <h1 class="con">
        {{ con }}<span class="bus">{{ bus }}</span>
      </h1>

      <p class="we">
       {{ we }}
      </p>

      <p class="for">
       {{ for }}
      </p>

      <div class="fS">

        <div class="foundee">

          <img :src="author" alt="">

           <div class="ro">

            <h2>{{ rob }}</h2>
            <p>{{ founder }}</p>

           </div>

        </div>

        <div>
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
  data(){
    return{
      walk ,
      author,
      signature,
     h3:"WELCOME TO COMPANY",
     con:'Construction Company With Strategy In',
     bus: 'Business Growth',
     we:' We have been the trusted name in heating, air conditioning and plumbing businesses. Throughout the years, our number one goal',     
     for:' For over 80 years, We have been the trusted name in heating, air conditioning and plumbing businesses. Throughout the years, our number one goal has been to accurately . For over 80 years, We have been the trusted name in heating, air conditioning and plumbing businesses. Throughout the years, our number one goal has been to accurately .For over 80 years, We have been the trusted name in heating.',
    rob:'Robert Joe Kerry',
    founder: 'Founder',
    }
  },


}
</script>

<style lang="scss" scoped>
div {

  background-color: #13203b;
  padding-left: 3.5rem;
  padding-right: 3.5rem;
  font-family: Roboto, sans-serif;
  color: white;


  .walk {
    height: 80%;
  }

  .htext {

    margin-left: 15rem;

    .hr3 {
      display: flex;
      margin-top: -40rem;

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
    }

    .con {
      margin-left: 4rem;
      font-size: 2.6rem;
      font-weight: 750;
      margin-top: 3rem;

      .bus {
        font-weight: 20;
        font-size: 2rem;
      }
    }

    .we {
      margin-left: 4rem;
      font-size: 1.5rem;
      margin-top: 3rem;
      line-height: 2.5rem;
    }

    .for {
      margin-left: 4rem;
      font-size: 1.2rem;
      margin-top: 2rem;
      line-height: 2rem;
    }

    .fS {
      margin-left: -2.8rem;
      margin-top: 1.7rem;
      display: flex;

      .foundee {
        display: flex;

        img {
          border-radius: 360%;
        }

        .ro {
          margin-top: 1rem;
          

          p {
            margin-top: 10px;
          }
        }
      }
    }
  }
  .bottom{
    height:7rem;
  }

}
</style>