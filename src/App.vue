<template>
    <AppHeader></AppHeader>
    <div>
        <h1 class="text-danger text-center">APP</h1>
    </div>
</template>

<script>

import AppHeader from './components/AppHeader.vue';

export default {

    components: {
        AppHeader
    }
}
</script>

<style lang="scss" scoped>
div {
    background-color: azure;
}
</style>
