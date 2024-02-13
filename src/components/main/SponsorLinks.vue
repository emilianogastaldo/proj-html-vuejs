<script>
import ShopCards from './ShopCards.vue';
// importare dati da data 
import sponsors from '../../data/_sponsorImages'
export default {
    name: 'SponsorLinks',
    data: () => ({
        sponsors
    }),
    components: { ShopCards }

}
</script>

<template>
    <section id="sponsor" class="container">
        <div class="card-container d-flex justify-content-center align-items-center column-gap-3 text-center">
            <ShopCards v-for="sponsor in sponsors" :key="sponsor.id" v-bind="sponsor" />
        </div>
    </section>
</template>

<style scoped>
section #sponsor {
    min-height: 800px;
}
</style>