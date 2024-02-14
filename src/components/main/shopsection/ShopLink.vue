<script>
import ShopCard from './ShopCard.vue';
import shops from '../../../data/_shopData'
export default {
    name: 'ShopLink',
    data: () => ({
        shops
    }),
    components: { ShopCard }
}
</script>

<template>
    <section id="shop">
        <div class="container">
            <div class="card-container">
                <ShopCard v-for="shop in shops" :key="shop.id" v-bind="shop" />
            </div>
        </div>
    </section>
</template>

<style scoped>
#shop {
    background: linear-gradient(to top,
            rgba(0, 0, 0, 1) 0%,
            rgba(0, 0, 0, 0) 100%), url("../../../assets/images/banner2-2x.jpg");
    background-size: cover;
    background-position: center;
    position: relative;
}

.card-container {
    padding: 200px;
}
</style>