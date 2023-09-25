<!-- TEMPLATE -->
<template>
    <div class="container min-vw-100 dc-mainContainer">
        <main class="row justify-content-center">

            <AppCardsContainer />

        </main>

    </div>
</template>

<!-- EXPORT & SCRIPTS -->
<script>
import AppCardsContainer from './AppCardsContainer.vue';

export default {
    name: "AppMain",

    components: {
        AppCardsContainer
    }
};


</script>

<!-- STYLE -->
<style lang="scss" scoped>
// STYLESHEET LINK
@use '../assets/scss/partials/AppMain.scss';
</style>