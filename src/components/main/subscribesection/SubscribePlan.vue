<script>
import SubscribePlanCard from './SubscribePlanCard.vue';
import { subPlan } from '../../../data/index';
export default {
    name: 'SubscribePlan',
    data: () => ({
        subPlan
    }),
    components: {
        SubscribePlanCard,
    }
}
</script>

<template>
    <section id="subscribe-plan">
        <div class="container align-item-center justify-content-center">
            <div class="row g-5 row-col-3">
                <a class="col" v-for="card in subPlan" :key="card.id" :href="card.url">
                    <SubscribePlanCard :icon="card.icon" :title="card.title" :subtitle="card.subtitle"
                        :paragrph="card.paragrph" :link="card.link" :url="card.url" />
                </a>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
#subscribe-plan {
    background-color: black;
    padding: 7rem 0;
}

a {
    color: white;
    text-decoration: none;
}
</style>