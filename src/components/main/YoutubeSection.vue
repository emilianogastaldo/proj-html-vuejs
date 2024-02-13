<script>
import YoutubePlaylist from './YoutubePlaylist.vue';
import { youtubeLinks } from '../../data';
import YoutubeChannel from './YoutubeChannel.vue'
export default {
    name: 'YoutubeSection',
    data: () => ({
        youtubeLinks
    }),
    components: { YoutubeChannel, YoutubePlaylist }
}
</script>

<template>
    <YoutubeChannel />
    <YoutubePlaylist :youtubeLinks="youtubeLinks" />
</template>

<style lang="scss" scoped></style>
