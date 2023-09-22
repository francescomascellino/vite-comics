<template>
    <div class="container min-vw-100">

        <div class="row flex-column justify-content-flex-end dc-footerCont">

            <footer class="p-0 ">

                <div class="d-flex justify-content-center dc-footerLinks">

                    <div class="col-8 d-flex">

                        <div>
                            <h5 class="text-uppercase text-light">dc comics</h5>

                            <ol class="list-unstyled text-light">
                                <li class="text-capitalize">Character</li>
                                <li class="text-capitalize">Comics</li>
                                <li class="text-capitalize">Movies</li>
                                <li class="text-capitalize">TV</li>
                                <li class="text-capitalize">Games</li>
                                <li class="text-capitalize">Videos</li>
                                <li class="text-capitalize">News</li>
                            </ol>

                            <h5 class="text-uppercase text-light">shop</h5>

                            <ol class="list-unstyled text-light">
                                <li class="text-capitalize">Shop DC</li>
                                <li class="text-capitalize">Shop DC Collectibles</li>
                            </ol>
                        </div>

                        <div>
                            <h5 class="text-uppercase text-light">dc</h5>

                            <ol class="list-unstyled text-light">
                                <li class="text-capitalize">terms of use</li>
                                <li class="text-capitalize">privacy policy</li>
                                <li class="text-capitalize">ad choices</li>
                                <li class="text-capitalize">advertising</li>
                                <li class="text-capitalize">jobs</li>
                                <li class="text-capitalize">subscriptions</li>
                                <li class="text-capitalize">talent workshops</li>
                                <li class="text-capitalize">CPSC certificates</li>
                                <li class="text-capitalize">ratings</li>
                                <li class="text-capitalize">shop help</li>
                                <li class="text-capitalize">contact us</li>
                            </ol>
                        </div>

                        <div>
                            <h5 class="text-uppercase text-light">sites</h5>

                            <ol class="list-unstyled text-light">
                                <li class="text-capitalize">dc</li>
                                <li class="text-capitalize">MAD magazine</li>
                                <li class="text-capitalize">dc kids</li>
                                <li class="text-capitalize">dc universe</li>
                                <li class="text-capitalize">dc power visa</li>
                            </ol>
                        </div>

                    </div>

                </div>

                <div class="d-flex justify-content-center dc-contacts">

                    <div class="col-8 d-flex align-items-center justify-content-between">

                        <button class="btn text-uppercase dc-signUpBtn">sign-up now!</button>

                        <div class="d-flex align-items-center dc-followCont">

                            <h4 class="text-uppercase m-0">follow us</h4>
                            <a href="#" class="ms-3"><img src="../assets/img/footer-facebook.png" alt=""></a>
                            <a href="#" class="ms-3"><img src="../assets/img/footer-twitter.png" alt=""></a>
                            <a href="#" class="ms-3"><img src="../assets/img/footer-youtube.png" alt=""></a>
                            <a href="#" class="ms-3"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                            <a href="#" class="ms-3"><img src="../assets/img/footer-periscope.png" alt=""></a>

                        </div>

                    </div>

                </div>

            </footer>

        </div>

    </div>
</template>

<script>
export default {
    name: "AppFooter"
}
</script>

<style lang="scss" scoped>
// VARIABLES LINK
@use '../assets/scss/partials/variables.scss' as *;

.dc-footerCont {
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;

}

.dc-footerLinks {

    padding: 2rem 0;

    .col-8 {
        div {
            margin-right: 2rem;

            h5 {
                font-weight: bold;
            }

            li {
                font-size: medium;
                color: $dc-secondary;
            }
        }
    }
}

footer {
    min-height: 325px;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-size: contain;
    background-position: right;
}

.dc-contacts {
    padding: 1.5rem 0;
    background-color: $dc-tertiary;
}

.dc-signUpBtn {
    border: 3px solid $dc-info;
    border-radius: 0;
    padding: 0.7rem 0.8rem;
    font-weight: bold;
    color: white;
}

h4 {
    color: $dc-info;
    font-weight: bold;
}
</style>