<!-- TEMPLATE -->

<template>
    <nav class="navbar py-0 navbar-expand-lg">

        <div class="container-fluid">

            <a class="navbar-brand" href="#"><img src="../assets/img/dc-logo.png" alt=""></a>

            <!-- CONTROLLARE PERCHE' NON FUNZIONA -->
            <!-- <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#dc-nav"
                aria-controls="dc-nav" aria-expanded="false" aria-label="Toggle navigation">

                <span class="navbar-toggler-icon"></span>

            </button> -->

            <!-- <div class="collapse navbar-collapse " id="dc-nav"> -->

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
            <!-- </div> -->
        </div>
    </nav>
</template>

<!-- EXPORT & SCRIPTS -->

<script>

export default {
    name: "AppHeader"

}

</script>

<!-- STYLE -->

<style lang="scss" scoped>
.navbar-nav a.nav-link {
    font-weight: bold;
    border-bottom: 5px solid transparent;
}

// QUESTA REGOLA SI PUO' INNESTARE SOPRA?
.navbar-nav a.nav-link:hover {
    border-bottom: 5px solid blue;
}
</style>