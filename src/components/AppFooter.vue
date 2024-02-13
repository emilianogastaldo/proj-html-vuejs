<script>
import { footerLinks } from '../data/index';
export default {
    name: 'AppFooter',
    data: () => ({
        footerLinks
    })

}
</script>

<template>
    <!-- Claudio -->
    <footer class="container text-center">
        <div class="footer-top">
            <div class="row row-cols-3 py-5">
                <div class="col">
                    <img src="../assets/images/logo.png" alt="" class="my-3">
                    <p>
                        Ac aliquam neque sagittis diam faucibus vitae purus turpis phasellus. Pellentesque consectetur amet
                        purus ultrices mauris.
                    </p>
                    <ul class="d-flex justify-content-center gap-2">
                        <li>
                            <a href="#"><i class="fa-brands fa-facebook-f" title="facebook"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-brands fa-twitter" title="twitter"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-brands fa-youtube" title="youtube"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-brands fa-instagram" title="instagram"></i></a>
                        </li>
                        <li>
                            <a href="#"><i class="fa-brands fa-linkedin" title="linkedin"></i></a>
                        </li>
                    </ul>
                </div>
                <div class="col pt-4">
                    <h5>RECENT POST</h5>
                    <ul class="footer-menu">
                        <!-- aggiungi a footerlinks il percorso url -->
                        <li class="pb-3" v-for="(link, i) in footerLinks" :key="i">
                            <a :href="link.url"><i class="fa-solid fa-chevron-right me-1"></i>{{ link.text }}</a>
                        </li>

                    </ul>
                </div>
                <div class="col pt-4">
                    <h5>CONTACT INFORMATION</h5>
                    <p>4746 Tipple Road Michigan 48449</p>
                    <div>
                        Mobile : 1.800.000.0000
                    </div>
                    <div>
                        Email : info@your-company.com
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom pt-5 pb-2">
            © Copyright 2012 - 2024 | <span><a href="#">Avada Website Builder</a></span> by <span><a
                    href="#">ThemeFusion</a></span> | All Rights
            Reserved | Powered by <span><a href="#">WordPress</a></span>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/style.scss';

footer {
    background-color: #060607;
    color: white;
    max-width: 100vw;
    font-size: 20px;

    .row {
        border-bottom: 1px solid #98939F;
    }

    p {
        color: #98939F;
    }

    ul {
        list-style-type: none;
        padding-left: 0;
    }

    li a {
        text-decoration: none;

        .fa-brands {
            color: #FF414B;
        }

        .fa-brands:hover {
            color: #98939F;
            transition: color 1s;
        }
    }

    .footer-menu a {
        color: white;
    }

    a:hover {
        color: #4154FF;
    }


    h5 {
        font-size: 25px;
        font-weight: 600;
        padding-bottom: 10px;
    }

    .footer-bottom {
        color: #C8C8CA;
        font-weight: 600;

        span a {
            color: white;
            text-decoration: none;
        }

        span a:hover {
            color: #4154FF;
        }
    }
}
</style>
