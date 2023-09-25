<!-- TEMPLATE -->
<template>
    <div class="container min-vw-100 dc-mainContainer">
        <div class="row justify-content-center">

            <main class="col-8 p-0">

                <div class="d-flex align-items-center dc-comicCards">

                    <ComicCards />

                </div>

            </main>

        </div>

    </div>
</template>

<!-- EXPORT & SCRIPTS -->
<script>
import ComicCards from './ComicCards.vue';

export default {
    name: "AppMain",

    components: {
        ComicCards
    }
};


</script>

<!-- STYLE -->
<style lang="scss" scoped>
// STYLESHEET LINK
@use '../assets/scss/partials/AppMain.scss';
</style>