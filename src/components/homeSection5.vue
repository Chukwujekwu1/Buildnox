<template>
    <div class="div">
       <div class="h-96 blue">
        <div class="flex-col">
            <div class="flex-row">
                <hr>
                <h3>{{ header1 }}</h3>
            </div>
        </div>
       </div>

    </div>
</template>

<script >
import roofImg from '../components/icons/gallery-1.jpg';
import consructionImg from '../components/icons/gallery-2.jpg';
import generalContructionImg from '../components/icons/gallery-3.jpg';
export default{
    data (){
        return{
            roofImg,
            consructionImg,
            generalContructionImg,
            header1:'OUR WORKS'

        }
    }
}
</script>

<style lang="css" scoped>
.div{
    margin-top: -0.7rem;
}
.blue{
 background-color: #13203b;
}

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
</style>