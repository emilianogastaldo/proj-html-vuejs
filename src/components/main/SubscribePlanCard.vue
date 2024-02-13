<script>
import { subPlan } from '../../data/index';
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
        <div class="icona"><i class="fa-solid fa-2xl" :class="icon"></i></div>
        <div class="card-body">
            <h5 class="card-title">{{ title }}</h5>
            <h6>{{ subtitle }}</h6>
            <p class="card-text">{{ paragrph }}</p>
            <a :href="url">{{ link }} <span><i class="fa-solid fa-chevron-right fa-2xs"></i></span></a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    background-color: black;
    border: solid 3px #4154FF;
    min-height: 450px;
    max-width: 350px;
    cursor: pointer;
    margin-top: 70px;
}

.card:hover {
    transition: all .2s ease-in-out;
    transform: scale(1.1);
}

.icona {
    color: white;
    margin-top: 70px;
}


h5 {
    color: white;
}

h6 {
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
}

i {
    color: white;
}
</style>