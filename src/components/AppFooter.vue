<template>
    <div class="container min-vw-100">

        <div class="row flex-column justify-content-flex-end dc-footerCont">

            <footer class="p-0 ">

                <div class="d-flex justify-content-center dc-footerLinks">

                    <div class="col-8 d-flex dc-bigLogo">

                        <div class="dc-listContainer">
                            <h5 class="text-uppercase text-light">dc comics</h5>

                            <ol class="list-unstyled text-light">
                                <li class="text-capitalize"><a href="#">Character</a></li>
                                <li class="text-capitalize"><a href="#">Comics</a></li>
                                <li class="text-capitalize"><a href="#">Movies</a></li>
                                <li class="text-capitalize"><a href="#">TV</a></li>
                                <li class="text-capitalize"><a href="#">Games</a></li>
                                <li class="text-capitalize"><a href="#">Videos</a></li>
                                <li class="text-capitalize"><a href="#">News</a></li>
                            </ol>

                            <h5 class="text-uppercase text-light">shop</h5>

                            <ol class="list-unstyled text-light">
                                <li class="text-capitalize"><a href="#">Shop DC</a></li>
                                <li class="text-capitalize"><a href="#">Shop DC Collectibles</a></li>
                            </ol>
                        </div>

                        <div class="dc-listContainer">
                            <h5 class="text-uppercase text-light">dc</h5>

                            <ol class="list-unstyled text-light">
                                <li class="text-capitalize"><a href="#">terms of use</a></li>
                                <li class="text-capitalize"><a href="#">privacy policy</a></li>
                                <li class="text-capitalize"><a href="#">ad choices</a></li>
                                <li class="text-capitalize"><a href="#">advertising</a></li>
                                <li class="text-capitalize"><a href="#">jobs</a></li>
                                <li class="text-capitalize"><a href="#">subscriptions</a></li>
                                <li class="text-capitalize"><a href="#">talent workshops</a></li>
                                <li class="text-capitalize"><a href="#">CPSC certificates</a></li>
                                <li class="text-capitalize"><a href="#">ratings</a></li>
                                <li class="text-capitalize"><a href="#">shop help</a></li>
                                <li class="text-capitalize"><a href="#">contact us</a></li>
                            </ol>
                        </div>

                        <div class="dc-listContainer">
                            <h5 class="text-uppercase text-light">sites</h5>

                            <ol class="list-unstyled text-light">
                                <li class="text-capitalize"><a href="#">dc</a></li>
                                <li class="text-capitalize"><a href="#">MAD magazine</a></li>
                                <li class="text-capitalize"><a href="#">dc kids</a></li>
                                <li class="text-capitalize"><a href="#">dc universe</a></li>
                                <li class="text-capitalize"><a href="#">dc power visa</a></li>
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

footer {
    min-height: 325px;
}


.dc-footerLinks {

    .dc-bigLogo {
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: right;
    }


    .dc-listContainer {

        padding: 2rem 0;

        margin-right: 2rem;

        h5 {
            font-weight: bold;
        }

        li a {
            font-size: medium;
            text-decoration: none;
            color: $dc-secondary;

            &:hover {
                color: $dc-info;
            }
        }
    }

}

.dc-contacts {
    padding: 1.5rem 0;
    background-color: $dc-tertiary;

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

}
</style>