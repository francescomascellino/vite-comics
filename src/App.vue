<template>
    <div class="container">

        <AppHeader></AppHeader>

        <div>

            <div class="row">
                <h1 class="text-danger text-center">APP</h1>
            </div>



        </div>
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
    border: 1px solid red;
}
</style>
