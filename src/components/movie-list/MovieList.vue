<template lang="">
    <ul class="movie-list list-group">
        <MovieListItem 
            v-for="movie in movies" 
            v-bind:movie="movie" :key="movie.id" 
            @onTogggle='$emit("onTogggle", $event)'
            @onRemove='$emit("onRemove", $event)'
        />
    </ul>
</template>
<script>
import MovieListItem from '../movie-list-item/MovieListItem.vue';
export default {
    components:{MovieListItem},
    props:{
        movies:{
            type: Array,
            required:true,
        }
    }
    }
</script>