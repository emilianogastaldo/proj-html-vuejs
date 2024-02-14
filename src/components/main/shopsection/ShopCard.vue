<script>
import AppButton from '../../AppButton.vue';
export default {
    name: 'ShopCard',
    components: { AppButton },
    props: {
        id: Number,
        quote: String,
        text: String,
        button: String
    }
}
</script>

<template>
    <div class="card d-flex justify-content-center align-items-center text-center">
        <div class="card-body">
            <h5 class="card-title mb-4">"{{ quote }}"</h5>
            <span><i v-for="n in 3" class="fa-solid fa-chevron-up"></i> </span>
            <p class="card-text mt-4">{{ text }}</p>
            <AppButton class="mt-2">
                {{ button }} <i class="fa-solid fa-chevron-right"></i>
            </AppButton>

        </div>
    </div>
</template>

<style scoped>
.card {
    border-color: transparent;
    background-color: transparent;
    color: white;
}

span {
    color: #fff941;
}

h5 {
    font-size: 3.5rem;
    font-weight: 600;
}

p {
    font-size: 1.5rem;
}
</style>