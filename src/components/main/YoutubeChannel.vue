<script>
export default {
    name: 'YoutubeChannel'
}
</script>

<template>
    <section class="row my-4">
        <div class="col-6 position-relative">
            <div class="image-section">
                <img class="img-fluid" src="../../assets/images/service15-2x.jpg" alt="woman">
            </div>
        </div>
        <div class="col-6">
            <div class="text px-5">
                <p>Tune up your works</p>
                <h1>The best health & fitness advice online</h1>
                <div class="youtube-avatar d-flex">
                    <img class="img-fluid" src="../../assets/images/unnamed.jpg" alt="channel avatar">
                    <div>
                        <p class="m-0">ThemeFusion</p>
                        <button>Youtube</button>
                        <button>999+</button>
                    </div>
                </div>
                <p>Arcu eu facilisi ut quisque placerat nunc habitant. Magna semper mauris, venenatis, leo integer sit
                    pellentesque.</p>
                <button>Visit my YouTube channel</button>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
.image-section {
    height: 300px;
    position: absolute;
    top: -150px;
    left: 10px;

    img {
        border-radius: 0 5px 50px 0;
    }
}

.text {
    padding-top: 100px;
    padding-bottom: 400px;

}
</style>
