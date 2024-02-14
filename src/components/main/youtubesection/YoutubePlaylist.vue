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
    <figure class="container">
        <div class="row justify-content-between h3 mb-5">
            <div class="col">Featured playlists</div>
            <div class="col text-end">
                <a href="https://avada.website/fitness/playlists/">View all videos
                    <i class="fa-solid fa-angle-right"></i></a>
            </div>
        </div>
        <ul class="d-flex gap-5 text-center">
            <li v-for="youtubeLink in youtubeLinks" :key="youtubeLink.id">
                <YoutubeCard v-bind="youtubeLink" />
            </li>
        </ul>
    </figure>
</template>
<style lang="scss" scoped>
@use '../../../assets/scss/style.scss';

figure {
    margin-bottom: 150px;
}

ul {
    list-style-type: none;
    padding-left: 0;
}

a {
    text-decoration: none;
    color: black;
}

.row {
    font-weight: 600;
}
</style>