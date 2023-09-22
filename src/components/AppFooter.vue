<template>
    <div class="container min-vw-100">

        <div class="row flex-column justify-content-flex-end dc-footerCont">

            <footer class="p-0">

                <h1 class="text-danger">TEST</h1>

                <div class="dc-logoBig">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>

                <div class="d-flex justify-content-center dc-contacts">

                    <div class="col-10 d-flex align-items-center justify-content-between">

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
.dc-footerCont {
    background-image: url("../assets/img/footer-bg.jpg");
    position: relative;
}

.dc-logoBig {
    border: 1px solid red;
    z-index: -1;
}

.dc-contacts {
    padding: 1.5rem 0;
    background-color: darkgrey;
    z-index: 10;
}

.dc-signUpBtn {
    border: 3px solid blue;
    border-radius: 0;
    padding: 0.7rem 0.8rem;
    font-weight: bold;
    color: white;
}
</style>