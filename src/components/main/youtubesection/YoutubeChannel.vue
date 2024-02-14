<script>
import AppButton from '../AppButton.vue';
export default {
    name: 'YoutubeChannel',
    components: { AppButton }
}
</script>

<template>
    <section class=" d-flex my-5">
        <div class="col-6 position-relative">
            <div class="image-container">
                <div class="position-relative">
                    <img class="img-fluid" src="../../../assets/images/service15-2x.jpg" alt="woman">
                    <a href="#" class="play-button">
                        <i class="fas fa-play"></i>
                    </a>
                </div>
            </div>
        </div>
        <div class="col-6">
            <div class="text px-5">
                <p class="color-blue up-title">Tune up your works</p>
                <h2>The best health & fitness advice online</h2>
                <div class="youtube-avatar d-flex my-4 gap-1">
                    <img class="img-fluid" src="../../../assets/images/unnamed.jpg" alt="channel avatar">
                    <div class="channel-button">
                        <p class="m-0">ThemeFusion</p>
                        <button><i class="fa-brands fa-youtube"></i> Youtube</button>
                        <span> 999+</span>
                    </div>
                </div>
                <p class="paragraph color-gray">Arcu eu facilisi ut quisque placerat nunc habitant. Magna semper mauris,
                    venenatis, leo
                    integer sit
                    pellentesque.</p>
                <AppButton class="color-white bg-color-red">
                    <i class="fa-brands fa-youtube"></i> Visit my Youtube channel
                </AppButton>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.color-blue {
    color: #4154ff;
}

.color-white {
    color: white
}

.bg-color-red {
    background-color: red;
}

.bg-color-blue {
    background-color: #4154ff
}

.color-gray {
    color: #98939F;
}

.image-container {
    height: 100%;
    position: absolute;
    top: -100px;
    left: 0;

    img {
        border-radius: 0 5px 25px 0;
        width: 90%;
    }
}

.play-button {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    display: inline-block;
    line-height: 80px;
    text-align: center;
    height: 80px;
    width: 80px;
    border: none;
    color: blue;
    background-color: white;
    border-radius: 50%;
    font-size: 23px;
}

.play-button:hover {
    color: #FF414B;
}


.text {
    margin-bottom: 400px;

    h2 {
        font-size: 62px;
        font-weight: 600;
    }

    .up-title {
        font-size: 28px;
    }

    .paragraph {
        font-size: 23px;
    }

    .youtube-avatar {
        font-size: small;

        button {
            color: white;
            background-color: red;
            border: none;
        }

        span {
            border: 1px solid gray;
            display: inline-block;
            padding: 0 2px;
        }
    }
}
</style>
