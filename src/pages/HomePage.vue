<script>
        import SearchBar from "../components/SearchBar.vue"
        import CarouselJumbo from "../components/CarouselJumbo.vue"


        import {VueWriter} from 'vue-writer';
    export default {
        name: "HomePage",
        components:{VueWriter, SearchBar, CarouselJumbo }
    }


</script>

<template>
    <div class="ms_cont">
        <CarouselJumbo/>
        <div class="container d-flex flex-column justify-content-center py-2">
            <div class="row">
                <h1> Voglio andare a <VueWriter style="color: #FE5D26;" class="d-inline" :eraseSpeed="50" :array="['Londra','Parigi','Roma','Berlino','Madrid','Milano']"/></h1> 
            </div>
            
            <div class="row">
                <SearchBar/>
            </div>
            
        </div>
    </div>
</template>

<style scoped lang="scss">
    @use "../style/partials/palette" as *;
    @import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@300..700&display=swap');

    .container {
        height: 100vh;
        font-family: "Quicksand", Arial, Helvetica, sans-serif;
        padding-top: 100px;
        position: relative;
        z-index: 2;
        h1{
            font-weight: bold;
            color: $white;
        }
    }

    


</style>