<template>
    <div v-for="comic in comics">

        <h1>COMIC SERIE {{ comic.series }}</h1>

    </div>
</template>

<script>

import comics from '../comics.js';
export default {
    name: "ComicCards",
    data() {
        return {
            comics
        }
    }
}
</script>

<style lang="scss" scoped></style>