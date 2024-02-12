<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
    <!-- Claudio -->
    <footer class="container">
        <div class="footer-top">
            <div class="row row-cols-3 text-center">
                <div class="col border-white border">
                    <img src="../assets/images/logo.png" alt="" class="my-3">
                    <p>
                        Ac aliquam neque sagittis diam faucibus vitae purus turpis phasellus. Pellentesque consectetur amet
                        purus ultrices mauris.
                    </p>
                    <ul class="d-flex justify-content-around">
                        <li>
                            <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-brands fa-twitter"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-brands fa-youtube"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-brands fa-instagram"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-brands fa-linkedin"></i></a>
                        </li>
                    </ul>
                </div>
                <div class="col border-white border">
                    <ul>
                        <li>RECENT POST</li>
                        <li>
                            <a href="#"><i class="fa-solid fa-chevron-right"></i>The best protein shake</a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-solid fa-chevron-right"></i>Ultimate cardio workout</a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-solid fa-chevron-right"></i>New juices available now</a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-solid fa-chevron-right"></i>Tips to find training partners</a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-solid fa-chevron-right"></i>20 best healthy recipes</a>
                        </li>
                    </ul>
                </div>
                <div class="col border-white border">wgrwgrgrw</div>
                <!-- fare terza col, fare il footer bottom, sistemare il layout, fare lista per dati dinaminci  -->
            </div>
        </div>
        <div class="footer-bottom"></div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/style.scss';

footer {
    background-color: #060607;
    color: white;
    max-width: 100vw;

    p {
        color: #C8C8CA;
    }

    ul {
        list-style-type: none;
        padding-left: 0;
    }

    li a {
        text-decoration: none;

        .fa-brands {
            color: red;
        }
    }
}
</style>
