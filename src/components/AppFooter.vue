<script>
import FooterBottom from './footer/FooterBottom.vue';
import FooterTop from './footer/FooterTop.vue';
import { footerLinks } from '../data/index';
export default {
    name: 'AppFooter',
    data: () => ({
        footerLinks
    }),
    components: { FooterTop, FooterBottom }


}
</script>

<template>
    <!-- Claudio -->
    <footer>
        <div class="text-center">
            <FooterTop :footerLinks="footerLinks" />
            <FooterBottom />
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/style.scss';

footer {
    background-color: #060607;
    color: white;
    font-size: 20px;
}
</style>
