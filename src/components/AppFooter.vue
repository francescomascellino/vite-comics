<!-- TEMPLATE -->
<template>
    <div class="container min-vw-100">

        <div class="row flex-column justify-content-flex-end dc-footerCont">

            <footer class="p-0 ">

                <div class="d-flex justify-content-center dc-footerLinks">

                    <div class="col-8 pt-5 d-flex flex-column flex-wrap align-content-start dc-bigLogo">

                        <div class="col-2 dc-listContainer" v-for="(element) in footerLinks">

                            <h5 class="text-uppercase">{{ element.title }}</h5>

                            <ol class="list-unstyled">
                                <li v-for="(link) in element.links" key="index" class="text-capitalize"><a
                                        :href="link.path">{{ link.text }}</a></li>
                            </ol>

                        </div>

                        <!-- LISTE DEL MENU' SENZA V-FOR-->

                        <!--
                            <div class="dc-listContainer">

                                <h5 class="text-uppercase">dc comics</h5>

                                <ol class="list-unstyled">
                                    <li class="text-capitalize"><a href="#">Character</a></li>
                                    <li class="text-capitalize"><a href="#">Comics</a></li>
                                        <li class="text-capitalize"><a href="#">Movies</a></li>
                                    <li class="text-capitalize"><a href="#">TV</a></li>
                                        <li class="text-capitalize"><a href="#">Games</a></li>
                                    <li class="text-capitalize"><a href="#">Videos</a></li>
                                    <li class="text-capitalize"><a href="#">News</a></li>
                                </ol>

                                <h5 class="text-uppercase">shop</h5>

                                <ol class="list-unstyled">
                                    <li class="text-capitalize"><a href="#">Shop DC</a></li>
                                    <li class="text-capitalize"><a href="#">Shop DC Collectibles</a></li>
                                </ol>

                            </div> 

                            <div class="dc-listContainer">

                                <h5 class="text-uppercase">dc</h5>

                                <ol class="list-unstyled">
                                    <li class="text-capitalize"><a  href="#">terms of use</a></li>
                                    <li class="text-capitalize"><a  href="#">privacy policy</a></li>
                                    <li class="text-capitalize"><a  href="#">ad choices</a></li>
                                    <li class="text-capitalize"><a  href="#">advertising</a></li>
                                    <li class="text-capitalize"><a  href="#">jobs</a></li>
                                    <li class="text-capitalize"><a  href="#">subscriptions</a></li>
                                    <li class="text-capitalize"><a  href="#">talent workshops</a></li>
                                    <li class="text-capitalize"><a  href="#">CPSC certificates</a></li>
                                    <li class="text-capitalize"><a  href="#">ratings</a></li>
                                    <li class="text-capitalize"><a  href="#">shop help</a></li>
                                    <li class="text-capitalize"><a  href="#">contact us</a></li>
                                </ol>

                            </div>

                            <div class="dc-listContainer">

                                <h5 class="text-uppercase">sites</h5>

                                <ol class="list-unstyled">
                                    <li class="text-capitalize"><a  href="#">dc</a></li>
                                    <li class="text-capitalize"><a  href="#">MAD magazine</a></li>
                                    <li class="text-capitalize"><a  href="#">dc kids</a></li>
                                    <li class="text-capitalize"><a  href="#">dc universe</a></li>
                                    <li class="text-capitalize"><a  href="#">dc power visa</a></li>
                                </ol>

                            </div>
                        -->

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

<!-- EXPORT & SCRIPTS -->
<script>
export default {
    name: "AppFooter",
    data() {
        return {

            footerLinks: [

                {
                    title: "dc comics",
                    links: [
                        {
                            text: "Character",
                            path: "#"
                        },

                        {
                            text: "Comics",
                            path: "#"
                        },

                        {
                            text: "TV",
                            path: "#"
                        },

                        {
                            text: "Games",
                            path: "#"
                        },

                        {
                            text: "Videos",
                            path: "#"
                        },

                        {
                            text: "News",
                            path: "#"
                        }
                    ]
                },

                {
                    title: "shop",
                    links: [
                        {
                            text: "shop dc",
                            path: "#"
                        },
                        {
                            text: "shop dc collectibles",
                            path: "#"
                        }
                    ]
                },

                {
                    title: "dc",
                    links: [
                        {
                            text: "terms of use",
                            path: "#"
                        },

                        {
                            text: "privacy policy",
                            path: "#"
                        },

                        {
                            text: "ad choices",
                            path: "#"
                        },

                        {
                            text: "advertising",
                            path: "#"
                        },

                        {
                            text: "subscriptions",
                            path: "#"
                        },

                        {
                            text: "talent worshops",
                            path: "#"
                        },

                        {
                            text: "CPS certificates",
                            path: "#"
                        },

                        {
                            text: "ratings",
                            path: "#"
                        },

                        {
                            text: "shop help",
                            path: "#"
                        },

                        {
                            text: "contact us",
                            path: "#"
                        }
                    ]
                },

                {
                    title: "sites",
                    links: [
                        {
                            text: "dc",
                            path: "#"
                        },

                        {
                            text: "MAD magazine",
                            path: "#"
                        },

                        {
                            text: "dc kids",
                            path: "#"
                        },

                        {
                            text: "dc universe",
                            path: "#"
                        },

                        {
                            text: "dc power visa",
                            path: "#"
                        }
                    ]
                },

            ]

        }

    }
}
</script>

<!-- STYLE -->
<style lang="scss" scoped>
// STYLESHEET LINK
@use '../assets/scss/partials/AppFooter.scss' as *;
</style>