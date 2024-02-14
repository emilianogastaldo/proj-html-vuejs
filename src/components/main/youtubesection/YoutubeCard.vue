<script>
import PlayButton from '../../PlayButton.vue';
export default {
    name: 'YoutubeCard',
    components: {
        PlayButton
    },
    props: {
        id: Number,
        title: String,
        subtitle: String,
        img: String,
        url: String,
        alt: String
    },
    computed: {
        imagePath() {
            const path = new URL(`../../../assets/images/${this.img}`, import.meta.url);
            return path.href;
        }
    }
}
</script>
<template>
    <a :href="url">
        <div class="position-relative">
            <img :src="imagePath" :alt="alt" class="img-fluid">
            <PlayButton />
        </div>

        <h2>{{ title }}</h2>
        <h5>{{ subtitle }}</h5>

    </a>
</template>
<style lang="scss" scoped>
@use '../../../assets/scss/style.scss';

img {
    border-radius: 0 5px 25px 0;
}

a {
    text-decoration: none;
}

h2 {
    margin-top: 1.5rem;
    font-size: 25px;
    font-weight: 600;
    color: black;
}

h5 {
    color: #4154FF;
    font-weight: 600;
}

.play-button {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
</style>