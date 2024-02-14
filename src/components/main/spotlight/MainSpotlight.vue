<script>
import CardSpotlight from './CardSpotlight.vue';
import { storeSpotlight } from '../../data/index.js'
export default {
    name: 'MainSpotlight',
    components: {
        CardSpotlight
    },
    data: () => ({
        storeSpotlight
    })
}
</script>

<template>
    <section id="mainspotlight">
        <div class="container">
            <div class="row gap-5 card-container">
                <CardSpotlight v-for="card in storeSpotlight" :key="storeSpotlight.id" :card="card" />
            </div>

            <div class="text-under-cards">
                <h1>“How you respond to the challenge in the second half will determine what you become after the game,
                    whether
                    you are a winner or a loser.”</h1>
                <p>
                    <i v-for="n in 3" class="fa-solid fa-chevron-up color-yellow"></i>
                </p>
                <div class="runner">
                    <img class="circle-img" src="../../assets/images/avatar-1-2x.jpg" alt="runner">
                    <span>Brad Johnson </span>
                    <span class="fw-normal">Las Vegas</span>
                </div>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
#mainspotlight {
    background: linear-gradient(to bottom right, #0215D8, #D70110);
    padding-bottom: 100px;
}

.color-yellow {
    color: #FFF941;
}

.card-container {
    display: flex;
    justify-content: space-around;
    align-items: flex-end;
}

.text-under-cards {
    padding-bottom: 5rem;
    text-align: center;
    margin: 4rem 10rem 0 10rem;
    color: white;
    font-weight: 600;
}

.text-under-cards h1 {
    font-weight: 600;
}

.circle-img {
    border-radius: 50%;
    height: 4rem;
}

.runner {
    margin-top: 2rem;
}

.runner * {
    align-items: center;
    padding: 5px;
}
</style>

