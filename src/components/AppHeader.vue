<!-- TEMPLATE -->
<template>
    <div class="container min-vw-100">

        <div class="row justify-content-center">

            <div class="col-8 p-0">

                <nav class="navbar navbar-expand-lg py-0">

                    <a class="navbar-brand flex-grow-1" href="#"><img src="../assets/img/dc-logo.png" alt=""></a>

                    <div class="navbar-nav d-flex justify-content-between text-uppercase">

                        <a class="nav-link px-4 py-5" href="#">Characters</a>

                        <a class="nav-link px-4 py-5" href="#">Movies</a>

                        <a class="nav-link px-4 py-5" href="#">TV</a>

                        <a class="nav-link px-4 py-5" href="#">Games</a>

                        <a class="nav-link px-4 py-5" href="#">Collectibles</a>

                        <a class="nav-link px-4 py-5" href="#">Videos</a>

                        <a class="nav-link px-4 py-5" href="#">Fans</a>

                        <a class="nav-link px-4 py-5" href="#">News</a>

                        <a class="nav-link px-4 py-5" href="#">Shop</a>

                    </div>

                </nav>

            </div>

        </div>

        <!-- SPOSTARE IL JUMBOTRON IN UNCOMPONENTE SEPARATO. CONTROLLARE LINK IMG -->
        <div class="col-12 p-0 dc-jumbotron">

        </div>

    </div>
</template>

<!-- EXPORT & SCRIPTS -->
<script>

export default {
    name: "AppHeader"
}

</script>

<!-- STYLE -->
<style lang="scss" scoped>
// STYLESHEET LINK
@use '../assets/scss/partials/AppHeader.scss' as *;

.dc-jumbotron {
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}
</style>