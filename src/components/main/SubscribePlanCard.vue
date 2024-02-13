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
            <a href="#">{{ link }} <span><i class="fa-solid fa-chevron-right fa-2xs"></i></span></a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    background-color: black;
    border: solid 3px #4154FF;
    min-height: 350px;
    max-width: 250px;
    cursor: pointer;
    margin-top: 50px;
}

.card:hover {
    transition: all .2s ease-in-out;
    transform: scale(1.1);
}

.icona {
    color: white;
    margin-top: 30px;
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
}

a {
    color: white;
    text-decoration: none;
}

i {
    color: white;
}
</style>