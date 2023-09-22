<!-- TEMPLATE -->

<template>
    <div class="container min-vw-100 dc-menuCont">
        <div class="row justify-content-center">
            <div class="col-10 p-0">

                <div class="d-flex align-items-center justify-content-evenly dcMenuEl">

                    <a href="#" class="text-uppercase m-3"><img src="../assets/img/buy-comics-digital-comics.png"
                            alt=""><span class="ms-4">digital comics</span></a>

                    <a href="#" class="text-uppercase m-3"><img src="../assets/img/buy-comics-merchandise.png" alt=""><span
                            class="ms-4">dc merchandise</span></a>

                    <a href="#" class="text-uppercase m-3"><img src="../assets/img//buy-comics-subscriptions.png"
                            alt=""><span class="ms-4">subscription</span></a>

                    <a href="#" class="text-uppercase m-3"><img src="../assets/img/buy-comics-shop-locator.png" alt=""><span
                            class="ms-4">comic shop location</span></a>

                    <a href="#" class="text-uppercase m-3"><img src="../assets/img/buy-dc-power-visa.svg" alt=""><span
                            class="ms-4">dc power visa</span></a>

                </div>

            </div>
        </div>

    </div>
</template>

<!-- EXPORT & SCRIPTS -->

<script>
export default {
    name: "AppMenu"
}
</script>

<!-- STYLE -->

<style lang="scss" scoped>
// VARIABLES LINK
@use '../assets/scss/partials/variables.scss' as *;

.dc-menuCont {
    background-color: $dc-info;

}

.dcMenuEl {

    min-height: 90px;

    a {
        color: $dc-light;
        text-decoration: none;
        font-weight: bold;
        font-size: small;

        img {
            height: 45px;
        }
    }
}
</style>