<!-- TEMPLATE -->
<template>
    <div class="container min-vw-100">

        <div class="row justify-content-center">

            <div class="col-8 p-0">

                <nav class="navbar navbar-expand-lg py-0">

                    <a class="navbar-brand flex-grow-1" href="#"><img src="../assets/img/dc-logo.png" alt=""></a>

                    <div class="navbar-nav d-flex justify-content-between text-uppercase" v-for="(link, index) in navLinks">

                        <a class="nav-link px-4 py-5" :href="link.path" @click="turnActive(index)"
                            :class="(index == activeLink ? 'dc-active' : '')">
                            {{ link.text }}</a>

                    </div>

                </nav>

            </div>

        </div>
        <!-- SPOSTARE IL JUMBOTRON IN UNCOMPONENTE SEPARATO. CONTROLLARE LINK IMG -->
        <div class="row">

            <div class="col-12 d-flex justify-content-center p-0 dc-jumbotron">

                <div class="col-8 position position-relative">

                    <div class=" position-absolute top-100 translate-middle-y py-2 px-4 dc-currentSeries">
                        <h5 class="text-uppercase m-0">Current Series</h5>
                    </div>

                </div>

            </div>
        </div>

    </div>
</template>

<!-- EXPORT & SCRIPTS -->
<script>

export default {
    name: "AppHeader",


    data() {

        return {

            navLinks: [

                {
                    text: "characters",
                    path: "#"
                },


                {
                    text: "comics",
                    path: "#"
                },

                {
                    text: "movies",
                    path: "#"
                },

                {
                    text: "tv",
                    path: "#"
                },

                {
                    text: "games",
                    path: "#"
                },

                {
                    text: "collectibles",
                    path: "#"
                },

                {
                    text: "videos",
                    path: "#"
                },

                {
                    text: "fans",
                    path: "#"
                },

                {
                    text: "news",
                    path: "#"
                },

                {
                    text: "shop",
                    path: "#"
                }


            ],

            activeLink: 1

        }

    },

    methods: {

        turnActive(index) {
            this.activeLink = index
        }

    }

}

</script>

<!-- STYLE -->
<style lang="scss" scoped>
// STYLESHEET LINK
@use '../assets/scss/partials/AppHeader.scss' as *;
</style>