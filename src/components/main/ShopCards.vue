<script>
export default {
    name: 'ShopCards',
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
            <h5 class="card-title">{{ quote }}</h5>
            <span><i class="fa-solid fa-chevron-up"></i><i class="fa-solid fa-chevron-up"></i><i
                    class="fa-solid fa-chevron-up"></i></span>
            <p class="card-text">{{ text }}</p>
            <a href="#" class="btn btn-primary">{{ button }} <i class="fa-solid fa-chevron-right"></i></a>
        </div>
    </div>
</template>

<style scoped>
.card {
    border-color: transparent;
}

span {
    color: #fff941
}

h5 {
    font-size: 4rem;
    font-weight: 600;
}

p {
    font-size: 1.5rem;
}
</style>