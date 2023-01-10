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
    <section id="jumbotron" class="container">
        <h3 class="title">--&#62; Content goes here &#60;--</h3>
        <section id="comics-container">
            <SingleComic v-for="comicInfo in json" :thumb="comicInfo.thumb" :price="comicInfo.price"
                :series="comicInfo.series" :type="json.type" />
        </section>
    </section>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;



#jumbotron {
    background-color: $secondary--color;

    .title {
        padding: 1.2rem 0;
    }
}
</style>