<script>
import { subPlan } from '../../../data/index';
export default {
    name: 'SubscribePlanCard',
    data: () => ({
        subPlan
    }),
    props: {
        icon: String,
        title: String,
        subtitle: String,
        paragrph: String,
        link: String,
        url: String
    }
}
</script>

<template>
    <div class="card text-center">
        <div class="card-body d-flex flex-column justify-content-center align-items-center">
            <div class="icona"><i class="fa-solid" :class="icon"></i></div>
            <h2 class="card-title">{{ title }}</h2>
            <h4>{{ subtitle }}</h4>
            <p class="card-text">{{ paragrph }}</p>
            <a :href="url">{{ link }} <span><i class="fa-solid fa-chevron-right fa-2xs"></i></span></a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    background-color: black;
    border: solid 3px #4154FF;
    min-height: 550px;
    cursor: pointer;
}

.card:hover {
    transition: all .2s ease-in-out;
    transform: scale(1.1);
}

.icona {
    font-size: 4rem;
    color: white;
    margin-bottom: 30px;
}


h2 {
    color: white;
}

h4 {
    color: #FFF941;
}

p {
    color: white;
    margin: 30px 0;
    padding: 20px;
    font-size: 20px;
}

a {
    color: white;
    text-decoration: none;
    font-weight: 600;
    font-size: 1.2rem;
}
</style>