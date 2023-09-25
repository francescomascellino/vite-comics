<!-- TEMPLATE -->
<template>
    <div class="container min-vw-100 dc-mainContainer">
        <main class="row justify-content-center">

            <ComicCards />

        </main>

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