<script>
export default {
    name: 'EventSection'
}
</script>

<template>
    <section>
        <div class="container">
            <div class="wrapper color-white">
                <a href="#" class="play-button ">
                    <i class="fa-solid fa-play"></i>
                </a>
                <h2>Crossfit workout of the day</h2>
                <p>November 15th, 20219</p>
                <a href="#" class="color-white">View all videos <i class="fa-solid fa-arrow-right-long"></i> </a>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    // background-image: url('../../assets/images/banner14-2x.jpg');
    // background: linear-gradient(#0215D8, #D70110), url('../../assets/images/banner14-2x.jpg');

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

.play-button {
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
</style>
