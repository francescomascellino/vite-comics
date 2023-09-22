<!-- TEMPLATE -->

<template>
    <div class="container min-vw-100">
        <div class="row justify-content-center">
            <div class="col-10 p-0">
                <nav class="navbar navbar-expand-lg py-0">

                    <a class="navbar-brand flex-grow-1" href="#"><img src="../assets/img/dc-logo.png" alt=""></a>

                    <div class="navbar-nav d-flex justify-content-between text-uppercase">

                        <a class="nav-link px-4 py-5" href="#">Characters</a>

                        <a class="nav-link px-4 py-5" href="#">Movies</a>

                        <a class="nav-link px-4 py-5" href="#">TV</a>

                        <a class="nav-link px-4 py-5" href="#">Games</a>

                        <a class="nav-link px-4 py-5" href="#">Collectibles</a>

                        <a class="nav-link px-4 py-5" href="#">Videos</a>

                        <a class="nav-link px-4 py-5" href="#">Fanse</a>

                        <a class="nav-link px-4 py-5" href="#">News</a>

                        <a class="nav-link px-4 py-5" href="#">Shop</a>

                    </div>
                </nav>
            </div>
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
// VARIABLES LINK
@use '../assets/scss/partials/variables.scss' as *;

.navbar-nav a.nav-link {
    font-weight: bold;
    color: $dc-secondary;
    border-bottom: 5px solid transparent;
}

// QUESTA REGOLA SI PUO' INNESTARE SOPRA?
.navbar-nav a.nav-link:hover {
    color: $dc-info;
    border-bottom: 5px solid $dc-info;
}
</style>