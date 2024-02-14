<script>
export default {
    name: 'CardSpotlight',
    props: {
        card: Object
    }
}
</script>

<template>
    <div class="col card" :class="card.image">
        <div>
            <i v-for="n in 3" class="fa-solid fa-chevron-up color-white"></i>
        </div>
        <p class="my-text-white ">{{ card.title }}</p>
        <p class="my-text-yellow">{{ card.subtitle }}</p>
    </div>
</template>

<style lang="scss" scoped>
.card {
    height: 26rem;
    background-color: #fff;
    border-radius: 0 0 2.5rem 0;
    box-shadow: 2px 1px 8px 8px rgb(0 0 0 / 10%);
    padding: 20px;
    transition: transform 0.3s ease-out;
    margin-top: -100px;

    filter: brightness(0.9);
    border: none;
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: flex-end;

    p {
        text-align: start;
        margin-bottom: 0;
    }
}

.card:hover {
    transform: scale(1.05);
}

.bg-disset {
    background: linear-gradient(to top, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0)), url(../../assets/images/service6-2x.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}

.bg-gym-clothes {
    background: linear-gradient(to top, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0)), url(../../assets/images/box1-2x.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}

.bg-gym {
    background: linear-gradient(to top, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0)), url(../../assets/images/box3-2x.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}

.my-text-white {
    color: #fff;
    font-size: 1.5rem;
    font-weight: 600;
}

.color-white {
    color: white;
}

.my-text-yellow {
    color: #FFF941;
    font-size: 1.2rem;
    font-weight: 600;
}
</style>
