<template>
    <div >

        <img :src="logo" alt="" class="xl:w-48     sm:w-40">

        <ul class=" ul">
            <li class="">
                <a href="/" >Home </a>
                <a href="/about">About</a>
                <a href="/project">Project</a>
                <a href="/service">Services</a>
                <a href="/team">Team</a>
                <a href="/contact">Contact</a>
            </li>
        </ul>
        <img :src="icon" alt="" class="icon" @click="mobile_nav_view">
    </div>
</template>

<script>
import logo from './icons/logo-light (1).png';
import icon from './icons/more.png';

export default {
    data() {
        return {
           
            logo,
            icon,
        }
    },
    methods:{
        mobile_nav_view(){
            this.$emit('my-event', true)
        }
    }
}
</script>

<style lang="css" scoped>

.mobile_view{
   width: 15rem;
   height: 10vh;
   background-color:black;
   position:sticky ;
}


div {
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    text-align: center;

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