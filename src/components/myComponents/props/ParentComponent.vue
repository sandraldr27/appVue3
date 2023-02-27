<script>
import ChildComponent from './ChildComponent.vue'
export default {
  components: { ChildComponent },
    data() {
        return {
            movieTitle: 'Superman',
            brandParent :"",
            count : 0,
        }
    },
    methods: {
        receivedBrand(data){
            this.$brand = data;
            this.count++;
        }
    },
}
</script>

<template>
    <h2>I'm your Father</h2>
    <span>{{ movieTitle }}</span>
    <child-component :movieTitle="movieTitle" @changeBrand="receivedBrand"></child-component>
    <span>BRAND : {{ brand }} / {{ count }}</span>
</template>

<style></style>
