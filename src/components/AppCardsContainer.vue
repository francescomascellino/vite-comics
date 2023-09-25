<template>
    <div class="col-8 py-5">

        <div class="row row-cols-6 g-3">

            <div class="col-2" v-for="comic in comics">

                <AppCards :dcCover="comic.thumb" :dcSeries="comic.series" :dcType="comic.type" :dcPrice="comic.price" />

            </div>
            <div class="col-12 d-flex justify-content-center align-items-center">
                <a href="#" class="btn text-uppercase px-5 dc-more">load more</a>
            </div>
        </div>

    </div>
</template>

<script>

import comics from '../comics.js';
import AppCards from './AppCards.vue';

export default {

    name: "AppCardsContainer",

    components: {
        AppCards
    },

    data() {
        return {
            comics
        }
    }

}
</script>

<style lang="scss" scoped>
@use '../assets/scss/partials/AppCardsContainer.scss';
</style>