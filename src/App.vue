<!-- TEMPLATE -->
<template>
    <AppHeader />

    <AppMain />

    <AppMenu />

    <AppFooter />
</template>

<!-- SCRIPTS -->
<script>

import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppMenu from './components/AppMenu.vue';

export default {

    components: {
        AppHeader,
        AppMain,
        AppFooter,
        AppMenu
    }
}
</script>

<!-- STYLE -->
<style lang="scss" scoped></style>
