<script>
export default {
    data() {
        return {
            comicTitle: 'Amazing Spiderman - Vol.1',
            count:0,
        }
    },
    computed: {
        reversedComicTitle(){
            return this.comicTitle.split('').reverse().join('')
        },
        barColor() {
            return {
                'bg-sucess': this.count < 20,
                'bg-warning': this.count >= 20 && this.count <=30,
                'bg-danger': this.count > 30,
            }
        }
    }
}
</script>

<template>
    <div class="my-4">
        <h1>Computed Property</h1>
        <div>
            <p>{{ comicTitle }}</p>
            <p>{{ reversedComicTitle }}</p>
            <input type="text" v-model="comicTitle">
        </div>
        <div class="my-4">
            <button class="me-3 btn btn-primary" @click="count++">+</button>

        </div>

    </div>

</template>

<style lang="scss">
    @import "bootstrap/dist/css/bootstrap.min.css";
</style>