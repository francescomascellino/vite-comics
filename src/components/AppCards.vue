<template>
    <div class="card bg-transparent">

        <div class="p-1 dc-coverContainer" :style="{ backgroundImage: `url(${cover})` }">
        </div>

        <div class="card-body p-0 pt-3">

            <p class="card-title text-uppercase">{{ serie }}</p>
            <p class="card-text text-capitalize">{{ type }}, price: {{ price }}</p>

        </div>

    </div>
</template>

<script>
export default {
    name: "AppCards",

    props: {
        dcCover: String,
        dcSeries: String,
        dcType: String,
        dcPrice: String,
    }

}
</script>

<style lang="scss" scoped>
@use '../assets/scss/partials/AppCards.scss';
</style>