<script>
import SponsorCard from './SponsorCard.vue';
// importare dati da data 
import sponsors from '../../../data/_sponsorImages'
export default {
    name: 'SponsorLinks',
    data: () => ({
        sponsors
    }),
    components: { SponsorCard }

}
</script>

<template>
    <section id="sponsor" class="container">
        <ul class="row justify-content-center align-items-center text-center">
            <li class="col" v-for="sponsor in sponsors" :key="sponsor.id">
                <SponsorCard v-bind="sponsor" />
            </li>
        </ul>
    </section>
</template>

<style scoped>
#sponsor {
    min-height: 600px;
    padding: 100px 0 100px 0;
}

ul {
    list-style-type: none;
    display: flex;
    padding-inline-start: 0;
}
</style>