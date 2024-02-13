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
                <p class="color-blue up-title">Tune up your works</p>
                <h2>The best health & fitness advice online</h2>
                <div class="youtube-avatar d-flex my-4 gap-1">
                    <img class="img-fluid" src="../../assets/images/unnamed.jpg" alt="channel avatar">
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
                <button>Visit my YouTube channel</button>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
.color-blue {
    color: #4154ff;
}

.color-gray {
    color: #98939F;
}

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
