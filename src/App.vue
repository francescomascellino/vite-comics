<!-- TEMPLATE -->

<template>
    <div class="container">

        <AppHeader></AppHeader>

        <AppMain></AppMain>

    </div>
</template>

<!-- SCRIPTS -->

<script>

import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';

export default {

    components: {
        AppHeader,
        AppMain
    }
}
</script>

<!-- STYLE -->

<style lang="scss" scoped>
* {
    border: 1px solid red;
}
</style>
