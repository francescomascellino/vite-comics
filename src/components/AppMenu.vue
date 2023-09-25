<!-- TEMPLATE -->
<template>
    <div class="container min-vw-100 dc-menuCont">

        <div class="row justify-content-center">

            <div class="col-8 p-0">

                <div class="d-flex align-items-center justify-content-evenly flex-wrap p-4 dcMenuEl">

                    <a :href="link.path" class="text-uppercase m-3" v-for="link in servicesLinks"><img
                            :src="getImageUrl(link.img)" alt=""><span class="ms-4">{{ link.text }}</span></a>

                </div>

            </div>

        </div>

    </div>
</template>

<!-- EXPORT & SCRIPTS -->
<script>
export default {
    name: "AppMenu",

    data() {
        return {
            servicesLinks: [
                {
                    text: "digital comics",
                    img: "../assets/img/buy-comics-digital-comics.png",
                    path: "#"
                },

                {
                    text: "dc merchandise",
                    img: "../assets/img/buy-comics-merchandise.png",
                    path: "#"
                },

                {
                    text: "subscription",
                    img: "../assets/img/buy-comics-subscriptions.png",
                    path: "#"
                },

                {
                    text: "comic shop location",
                    img: "../assets/img/buy-comics-shop-locator.png",
                    path: "#"
                },

                {
                    text: "dc power visa",
                    img: "../assets/img/buy-dc-power-visa.svg",
                    path: "#"
                }

            ],

        }
    },

    methods: {
        //PRENDE IL PERCORSO CHE VERRRA' LETTO DALL'OGGETTO
        getImageUrl(path) {
            return new URL(`${path}`, import.meta.url).href
        }
    }
}
</script>

<!-- STYLE -->
<style lang="scss" scoped>
// STYLESHEET LINK
@use '../assets/scss/partials/AppMenu.scss' as *;
</style>