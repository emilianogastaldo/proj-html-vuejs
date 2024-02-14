<script>
import PlayButton from '../PlayButton.vue';
import AppButton from '../AppButton.vue';
export default {
    name: 'Jumbotron'
    , components: { PlayButton, AppButton }
}
</script>

<template>
    <!-- Amarildo -->
    <!-- Jumbotron -->

    <div class="jumbotron">
        <div class="container ">
            <div class="row justify-content-between align-items-center">
                <div class="col-9 content fade-in-down">
                    <h3>Certified fitness pofessional</h3>
                    <h1>Take control of your health</h1>
                    <p>
                        <i v-for="n in 3" class="fas fa-chevron-up color-yellow"></i>
                    </p>
                    <p>Curabitu non nula sit amen nisl tempus convallis quis ac lectus dolor sit amet</p>
                    <div class="buttons-container">
                        <AppButton>
                            <i class="fa-brands fa-youtube"></i> Visit my YouTube channel
                        </AppButton>
                        <AppButton class="btn-transparent">
                            Buy Avada today <i class="fa-solid fa-arrow-right"></i>
                        </AppButton>
                    </div>
                </div>
                <div class="col fade-in-down">
                    <PlayButton />
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.jumbotron {
    background: linear-gradient(to right,
            rgba(0, 0, 0, 1) 45%,
            rgba(0, 0, 0, 0) 100%),
        url(../../assets/images/slider82x-scaled.jpg);
    background-size: cover;

    background-position: top;
    color: white;
    text-align: center;
    padding: 200px 0;
}

.content {
    text-align: start;
}

h3 {
    font-size: 1.5em;
    font-weight: 600;
    color: #FF414B;
}

.color-yellow {
    color: #FFF941;
}

h1 {
    font-size: 4rem;
    margin-top: 10px;
    font-weight: 600;
}

p {
    font-size: 1.2rem;
    margin-top: 10px;
    color: #98939F;
}

// BUTTON--------------
.buttons-container {
    display: flex;
    margin-top: 1rem;
    gap: 0.5rem;
}

.row {
    transform: translate(0, -20%);
}

// EFFECT
.fade-in-down {
    opacity: 0;
    transform: translateY(-20px);
    animation: fadeInDown 2s ease-out forwards;
}

@keyframes fadeInDown {
    to {
        opacity: 1;
        transform: translateY(0);
    }
}
</style>