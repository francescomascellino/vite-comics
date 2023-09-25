<template>
    <div class="col-8 p-4">
        <div class="row row-cols-6 g-3 ">

            <div class="col-2" v-for="comic in comics">

                <AppCards :dcCover="comic.thumb" :dcSeries="comic.series" :dcType="comic.type" :dcPrice="comic.price" />

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

<style lang="scss" scoped></style>