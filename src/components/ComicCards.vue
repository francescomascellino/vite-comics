<template>
    <div class="col-8 p-4">
        <div class="row row-cols-6 g-3 ">

            <div class="col-2" v-for="comic in comics">
                <div class="card bg-transparent">

                    <div class="p-1 dc-coverContainer" :style="{ backgroundImage: `url(${comic.thumb})` }">
                    </div>

                    <div class="card-body p-0 pt-3">

                        <p class="card-title text-uppercase">{{ comic.series }}</p>
                        <p class="card-text text-capitalize">{{ comic.type }}, price: {{ comic.price }}</p>

                    </div>
                </div>
            </div>

        </div>
    </div>
</template>

<script>

import comics from '../comics.js';
export default {
    name: "ComicCards",
    data() {
        return {
            comics,
        }
    }
}
</script>

<style lang="scss" scoped>
// VARIABLES LINK
@use '../assets/scss/partials/variables.scss' as *;

.card {

    .dc-coverContainer {
        width: 100%;
        aspect-ratio: 1/1;
        background-position: top center;
        background-size: cover;
        background-repeat: no-repeat;
    }


    p {
        color: $dc-light;

        font-size: 0.7rem;
    }

}
</style>