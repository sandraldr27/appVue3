<script>
import ChildComponent from './ChildComponent.vue'
export default {
  components: { ChildComponent },
    data() {
        return {
            movieTitle: 'Shazam',
        }
    },
}
</script>

<template>
    <h2>I'm your Father</h2>
    <span>{{ movieTitle }}</span>
    <child-component></child-component>
</template>

<style>

</style>