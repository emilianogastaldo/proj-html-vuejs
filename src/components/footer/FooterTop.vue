<script>
import { footerLinks } from '../../data';

export default {
    name: 'FooterTop',
    props: {
        footerLinks: Array
    }
}
</script>
<template>
    <div class="footer-top">
        <div class="container">
            <div class="row row-cols-3 py-5">
                <div class="col">
                    <img src="../../assets/images/logo.png" alt="" class="my-3">
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
    </div>
</template>
<style lang="scss" scoped>
@use '../../assets/scss/style.scss';

.footer-top {
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
</style>