<template>
    <div >

        <img :src="logo" alt="" class="xl:w-48     sm:w-40">

        <ul class=" ul">
            <li class="">
                <a href="/" >Home </a>
                <a href="/about">About</a>
                <a href="/project">Project</a>
                <a href="/service">Services</a>
                <a href="/page">Pages</a>
                <a href="/contact">Contact</a>
            </li>
        </ul>
        <img :src="icon" alt="" class="icon">
    </div>
    <div v-if="mobile_nav_view" class="mobile_view">
        
    </div>
</template>

<script>
import logo from './icons/logo-light (1).png';
import icon from './icons/more.png';

export default {
    data() {
        return {
            mobile_nav_view:false,
            logo,
            icon,
        }
    }
}
</script>

<style lang="css" scoped>
div {
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    text-align: center;

}


.mobile_view{
   width: 15rem;
   height: 100vh;
   background-color:black;
   position: relative;
}

 


@media (max-width:1024px) {
    ul li a{
        display: none;
    }
    .icon{
        width: 2rem;
        height: 2rem;
    }
    div{
        padding:1rem ;
    }.ul{
        position:absolute;
    }
}
@media (min-width: 1200px) {
    
    ul li a {
    text-decoration: none;
    margin-left: 1.3rem;
    font-size: 1.3rem;
    font-weight: 2.5rem;
    color: white;
    font-family: Roboto;
    }
    ul li a:hover {
    color: orangered;
}
.icon{
    display: none;
}
div{
    padding: 4.2rem;
    padding-top:2rem;
}
}
</style>