<script>
import { isIntegerKey } from '@vue/shared';

export default {
    props: {
        movieTitle: String,
    }, 
    data() {
        return {
            brandChild: 'DC Comics',
        }
    },
    methods:{
        sendBrand(){
            this.$emit('changeBrand', this.brand)
        }
    }
}
</script>

<template>
    <h2>Hijito {{ movieTitle }}ito</h2>
    <button @click="sendBrand">sendBrand</button>
</template>

<style></style> 