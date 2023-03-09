<script>
import axios from 'axios'
export default {
    data() {
        return {
            chuckNorrisData : null,
        }
    },
    created() {
        axios.get('https://api.chucknorris.io/jokes/random').then((result) => {this.chuckNorrisData = result.data
        })
    }
}
</script>

<template>
    <div>
        <div v-if="chuckNorrisData">
            <h2>{{ chuckNorrisData.value }}</h2>  
            <h3>ID : {{ chuckNorrisData.id }}</h3>  
        </div>
    </div>
</template> 

<style lang="css" scoped>
    h2{
        color: aqua;
    }
    h3{
        color:rgb(191, 4, 191);
    }
</style>
