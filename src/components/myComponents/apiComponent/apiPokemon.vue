<script>
import axios from 'axios'
export default {
    data() {
        return {
            pokemonData : null,
        }
    },
    created() {
        axios.get('https://pokeapi.co/api/v2/pokemon/pikachu').then((result) => {this.pokemonData = result.data
        })
    }
}

</script>

<template>
    <div>
        <div v-if="pokemonData">
            <h2>{{ pokemonData.name }}</h2>    
            <img class="imgPokemon" : src="">

        </div>
    </div>
    
</template>

<style></style>