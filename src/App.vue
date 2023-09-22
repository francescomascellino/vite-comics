<!-- TEMPLATE -->

<template>
    <AppHeader></AppHeader>

    <AppMain></AppMain>

    <AppFooter></AppFooter>
</template>

<!-- SCRIPTS -->

<script>

import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {

    components: {
        AppHeader,
        AppMain,
        AppFooter
    }
}
</script>

<!-- STYLE -->

<style lang="scss" scoped></style>
