<script>
import PlayButton from '../PlayButton.vue';
export default {
    name: 'EventSection',
    components: {
        PlayButton
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="wrapper color-white">
                <PlayButton />
                <h2>Crossfit workout of the day</h2>
                <p>November 15th, 20219</p>
                <a href="#" class="color-white">View all videos <i class="fa-solid fa-arrow-right-long"></i> </a>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    filter: contrast(200%);
    background: linear-gradient(to bottom right,
            rgb(65, 84, 255, 0.4) 0%,
            rgba(255, 65, 75, 0.3) 100%),
        url("../../assets/images/banner14-2x.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    padding: 170px 0;
}

.wrapper {
    filter: contrast(100%);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    h2 {
        font-size: 58px;
    }

    p {
        font-size: 38px;
        color: #FFF941;
        font-weight: 600;
    }

    a {
        text-decoration: none;
        font-size: 20px;
    }
}

.color-white {
    color: white;
}
</style>
