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

                    </div>

                </div>

                <div class="d-flex justify-content-center dc-contacts">

                    <div class="col-8 d-flex align-items-center justify-content-between">

                        <button class="btn text-uppercase dc-signUpBtn">sign-up now!</button>

                        <div class="d-flex align-items-center dc-followCont">

                            <h4 class="text-uppercase m-0">follow us</h4>

                            <a :href="link.path" class="ms-3" v-for="link in socialLinks"><img :src="getImageUrl(link.img)"
                                    :alt="link.name"></a>

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

            ],

            socialLinks: [
                {
                    img: "../assets/img/footer-facebook.png",
                    name: "facebook",
                    path: "#"
                },

                {
                    img: "../assets/img/footer-twitter.png",
                    name: "twitter",
                    path: "#"
                },

                {
                    img: "../assets/img/footer-youtube.png",
                    name: "youtube",
                    path: "#"
                },

                {
                    img: "../assets/img/footer-pinterest.png",
                    name: "pinterest",
                    path: "#"
                },


                {
                    img: "../assets/img/footer-periscope.png",
                    name: "periscope",
                    path: "#"
                },
            ]

        }

    },
    methods: {

        //PRENDE IL PERCORSO CHE VERRA' LETTO DALL'OGGETTO
        getImageUrl(path) {
            return new URL(`${path}`, import.meta.url).href
        }

    }
}
</script>

<!-- STYLE -->
<style lang="scss" scoped>
// STYLESHEET LINK
@use '../assets/scss/partials/AppFooter.scss' as *;
</style>