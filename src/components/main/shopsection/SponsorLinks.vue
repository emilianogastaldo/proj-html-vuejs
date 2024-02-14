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
        <div class="card-container d-flex justify-content-center align-items-center column-gap-3 text-center">
            <ul>
                <li v-for="sponsor in sponsors" :key="sponsor.id">
                    <SponsorCard v-bind="sponsor" />
                </li>
            </ul>
        </div>
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
}
</style>