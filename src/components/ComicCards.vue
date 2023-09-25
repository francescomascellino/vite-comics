<template>
    <div class="col-8 p-4">
        <div class="row row-cols-6 g-3 ">

            <div class="col-2" v-for="(comic, index) in comics">
                <div class="card bg-transparent">

                    <div class="dc-coverContainer" :style="{ backgroundImage: `url(${comic.thumb})` }">
                    </div>

                    <div class="card-body">

                        <p class="card-title">{{ comic.series }}</p>
                        <p class="card-text">{{ comic.type }}</p>

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

h6 {
    color: $dc-light;
}

.card {

    .dc-coverContainer {
        width: 100%;
        aspect-ratio: 1/1;

        background-position: top center;
        background-size: cover;
        background-repeat: no-repeat;
        border: 1px solid rebeccapurple;
    }

}
</style>