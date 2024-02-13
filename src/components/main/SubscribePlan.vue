<script>
import SubscribePlanCard from './SubscribePlanCard.vue';
export default {
    name: 'SubscribePlan',
    components: {
        SubscribePlanCard
    }
}
</script>

<template>
    <section id="subscribe-plan">
        <div class="container d-flex align-item-center justify-content-center">
            <div class="row g-3 row-col-3">
                <SubscribePlanCard />
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