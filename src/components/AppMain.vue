<script>
import MainSpotlight from './main/spotlight/MainSpotlight.vue';
import YoutubeSection from './main/youtubesection/YoutubeSection.vue';
import SubscribeSection from './main/subscribesection/SubscribeSection.vue';
import ArticleSection from './main/articlesection/ArticleSection.vue';
import ShopSection from './main/shopsection/ShopSection.vue';
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
