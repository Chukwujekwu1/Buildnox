<template>
    <div>
        <div>
            {{ brand1 }}
        </div>
    </div>
</template>

<script>
import brand1 from './icons/brand-logo-1.png';
import brand2 from './icons/brand-logo-2.png';
import brand3 from './icons/brand-logo-3.png';
import brand4 from './icons/brand-logo-4.png';
import brand5 from './icons/brand-logo-5.png';

export default {
    data() {
        return {
            brands: [ brand1 ,  brand2 , brand3 , brand4 ,  brand5 ],
            brand1
        }
    }
}
</script>

<style lang="css" scoped></style>