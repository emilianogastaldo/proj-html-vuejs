<script>
export default {
    name: 'ShopCard',
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
            <span><i class="fa-solid fa-chevron-up"></i><i class="fa-solid fa-chevron-up"></i><i
                    class="fa-solid fa-chevron-up"></i>
            </span>
            <p class="card-text mt-4">{{ text }}</p>
            <a href="#" class="btn btn-primary mt-2">{{ button }} <i class="fa-solid fa-chevron-right"></i></a>
        </div>
    </div>
</template>

<style scoped>
.card {
    border-color: transparent;
    background-color: transparent;
    color: white;
}

.btn {
    padding: 10px 30px 10px 30px;
    border-radius: 50px;
    font-weight: 600;
    border-color: transparent;
}

a:hover {
    background-color: #ff414b;
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