<script>
export default {
    name: 'Jumbotron'
    , components: {
    }
}
</script>

<template>
    <!-- Amarildo -->
    <!-- Jumbotron -->

    <div class="jumbotron">
        <div class="container d-flex justify-content-between align-items-center">
            <div class="content fade-in-down">
                <h3>Certified fitness pofessional</h3>
                <h1>Take control of your helth</h1>
                <p>
                    <i v-for="n in 3" class="fa-solid fa-chevron-up color-yellow"></i>
                </p>
                <p>Curabitu non nula sit amen nisl tempus convallis quis ac lectus dolor sit amet</p>
                <div class="buttons-container">
                    <button class="btn-blue"><i class="fa-brands fa-youtube"></i> Visit my YouTube channel</button>
                    <button class="btn">Buy Avada today <i class="fa-solid fa-arrow-right"></i></button>
                </div>
            </div>
            <div>
                <button class="play-btn fade-in-down">
                    <i class="fa-solid fa-play"></i>
                </button>
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
    padding: 200px;
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
    font-size: 2.5em;
    margin-top: 10px;
    font-weight: 600;
}

p {
    font-weight: 600;
    font-size: 1em;
    margin-top: 10px;
    color: #98939F;
}

// BUTTON--------------
.buttons-container {
    display: flex;
    margin-top: 1rem;
    gap: 0.5rem;
}

.btn {
    font-weight: 600;
    color: #98939F;
    border-radius: 2rem;
    border: 1px solid #98939F;
    padding: 10px 20px;
    display: inline-block;
    font-size: 16px;
    cursor: pointer;
}

.btn-blue {
    font-weight: 600;
    background-color: #4154FF;
    color: white;
    border-radius: 2rem;
    border: none;
    padding: 10px 20px;
    display: inline-block;
    font-size: 16px;
    cursor: pointer;
}

.play-btn {
    background-color: #fff;
    border: none;
    width: 5rem;
    height: 5rem;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 20px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    cursor: pointer;

    transform: translate(-180px, -10px);
}

.play-btn i {
    color: #4154FF;
}

.play-btn i:hover {
    color: #FF414B;
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