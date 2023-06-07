<template>
    <div>

        <img :src="logo" alt="">

        <ul>
            <li>
                <a href="/">Home </a>
                <a href="/about">About</a>
                <a href="/project">Project</a>
                <a href="/service">Services</a>
                <a href="/page">Pages</a>
                <a href="/contact">Contact</a>
            </li>
        </ul>

    </div>
</template>

<script>
import logo from './icons/logo-light (1).png';

export default{
    data(){
        return{
            logo,
        }
    }
}
</script>

<style lang="scss" scoped>
div {
 display: flex;
 justify-content: space-between;
 padding-top: 2rem;
 text-align: center;
 padding-left: 4rem;
 padding-right: 4rem;
 
 
 ul{
  list-style: none;
  margin-top: 18px;  
 }
li{
  text-decoration: none,  
}
a{
    text-decoration:none;
    margin-left: 1.3rem;
    font-size: 1.3rem;
    font-weight:2.5rem;
    color: white;
    font-family: Roboto;
    &:hover{
        color:orangered;
    }
    
}   
  

}

;
</style>