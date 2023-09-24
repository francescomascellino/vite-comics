<!-- TEMPLATE -->
<template>
    <div class="container min-vw-100 dc-menuCont">

        <div class="row justify-content-center">

            <div class="col-8 p-0">

                <div class="d-flex align-items-center justify-content-evenly flex-wrap p-4 dcMenuEl">

                    <a :href="link.path" class="text-uppercase m-3" v-for="link in servicesLinks"><img :src="link.img"
                            alt=""><span class="ms-4">{{ link.text }}</span></a>

                    <!-- LINK SENZA V-FOR -->
                    <!-- 
                    <a href="#" class="text-uppercase m-3"><img src="../assets/img/buy-comics-digital-comics.png"
                            alt=""><span class="ms-4">digital comics</span></a>

                    <a href="#" class="text-uppercase m-3"><img src="../assets/img/buy-comics-merchandise.png" alt=""><span
                            class="ms-4">dc merchandise</span></a>

                    <a href="#" class="text-uppercase m-3"><img src="../assets/img/buy-comics-subscriptions.png"
                            alt=""><span class="ms-4">subscription</span></a>

                    <a href="#" class="text-uppercase m-3"><img src="../assets/img/buy-comics-shop-locator.png" alt=""><span
                            class="ms-4">comic shop location</span></a>

                    <a href="#" class="text-uppercase m-3"><img src="../assets/img/buy-dc-power-visa.svg" alt=""><span
                            class="ms-4">dc power visa</span></a>
                    
                    -->

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
                    img: "src/assets/img/buy-comics-digital-comics.png",
                    path: "#"
                },

                {
                    text: "dc merchandise",
                    img: "src/assets/img/buy-comics-merchandise.png",
                    path: "#"
                },

                {
                    text: "subscription",
                    img: "src/assets/img/buy-comics-subscriptions.png",
                    path: "#"
                },

                {
                    text: "comic shop location",
                    img: "src/assets/img/buy-comics-shop-locator.png",
                    path: "#"
                },

                {
                    text: "dc power visa",
                    img: "src/assets/img/buy-dc-power-visa.svg",
                    path: "#"
                }

            ]
        }
    }
}
</script>

<!-- STYLE -->
<style lang="scss" scoped>
// STYLESHEET LINK
@use '../assets/scss/partials/AppMenu.scss' as *;
</style>