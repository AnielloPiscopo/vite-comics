<script>
import { stringifyExpression } from '@vue/compiler-core';
import SingleComic from './SingleComic.vue';
console.log(json)
import json from './../../assets/json/dc-comics.json';

export default {
    name: 'MainJumbotron',

    components: {
        SingleComic,
    },

    data() {
        return {
            json,
        }
    },
}
</script>

<template>
    <section id="jumbotron">
        <div class="background"></div>

        <section id="comics-container" class="container">
            <h2 class="title text-uppercase btn">Current Series</h2>
            <SingleComic v-for="comicInfo in json" :thumb="comicInfo.thumb" :price="comicInfo.price"
                :series="comicInfo.series" :type="json.type" />

            <a href="#" class="btn text-uppercase">Load More</a>
        </section>
    </section>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;




.background {
    background-image: url('../../assets/img/jumbotron.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 350px;
}

#comics-container {
    background-color: $secondary--color;

    .btn {
        background-color: $complementary--color;
        display: inline-block;
        padding: 0.7rem 0;

        &.title {
            padding-left: 2rem;
            padding-right: 2rem;
        }
    }

    a.btn {
        padding-left: 5rem;
        padding-right: 5rem;
        color: $primary--color;
    }
}
</style>