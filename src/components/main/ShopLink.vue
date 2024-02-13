<script>
import ShopCards from './ShopCards.vue';
import shops from '../../data/_shopData'
export default {
    name: 'ShopLink',
    data: () => ({
        shops
    }),
    components: { ShopCards }
}
</script>

<template>
    <section id="shop" class="container">
        <div class="card-container ">
            <ShopCards v-for="shop in shops" :key="shop.id" v-bind="shop" />
        </div>
    </section>
</template>

<style scoped>
section #shop {
    min-height: 1000px;
    padding: 50px 0 50px 0;
    background-image: url(../../assets/images/banner2-2x.jpg);
}

.card-container {
    padding: 0 200px 0 200px;
}
</style>