<script>
import SubscribePlanCard from './SubscribePlanCard.vue';
import { subPlan } from '../../data/index';
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
        <div class="container d-flex align-item-center justify-content-center">
            <div class="row g-5 row-col-3">
                <div class="col" v-for="card in subPlan" :key="card.id">
                    <SubscribePlanCard :icon="card.icon" :title="card.title" :subtitle="card.subtitle"
                        :paragrph="card.paragrph" :link="card.link" :url="card.url" />
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
#subscribe-plan {
    background-color: black;
    min-height: 500px;
}
</style>