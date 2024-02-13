<script>
import YoutubeCard from './YoutubeCard.vue';
export default {
    name: 'YoutubePlaylist',
    props: {
        youtubeLinks: Array
    },
    components: {
        YoutubeCard
    }
}
</script>
<template>
    <figure class="container my-5">
        <ul class="d-flex gap-5 text-center">
            <li v-for="youtubeLink in youtubeLinks" :key="youtubeLink.id">
                <YoutubeCard v-bind="youtubeLink" />
            </li>
        </ul>
    </figure>
</template>
<style lang="scss" scoped>
@use '../../assets/scss/style.scss';

ul {
    list-style-type: none;
}
</style>