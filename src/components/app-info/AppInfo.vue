<template>
    <Box>
        <p class="fs-3 text-uppercase">Barcha kinolar soni : {{allMoviesCount}}</p>
        <p class="fs-4 text-uppercase">Ko'rilgan kinolar soni : {{favouriteMoviesCount}}</p>
        <img src="./movies.jpg" class="img-fluid" style="height: 50%; " alt="movies image">
    </Box>
</template>

<script>
export default {
    props:{
        allMoviesCount:{
            type: Number,
            required:true,
        },
        favouriteMoviesCount: {
            type:Number,
            required:true,
        }
    }
}
</script>