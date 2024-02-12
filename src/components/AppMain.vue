<script>
import MainSpotlight from './main/MainSpotlight.vue';
import YoutubeSection from './main/YoutubeSection.vue';
import SubscribeSection from './main/SubscribeSection.vue';
import ArticleSection from './main/ArticleSection.vue';
import ShopSection from './main/ShopSection.vue';
import EventSection from './main/EventSection.vue';
export default {
    name: 'AppMain',
    components: { MainSpotlight, YoutubeSection, SubscribeSection, ArticleSection, ShopSection, EventSection }
}
</script>

<template>
    <!-- Amarildo -->
    <MainSpotlight />

    <!-- Claudio ed Emiliano -->
    <YoutubeSection />

    <!-- Mateusz -->
    <SubscribeSection />

    <!-- Emiliano -->
    <ArticleSection />

    <!-- Leonardo -->
    <ShopSection />

    <!-- Emiliano -->
    <EventSection />
</template>

<style lang="scss" scoped></style>
