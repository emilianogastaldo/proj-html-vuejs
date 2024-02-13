<script>
export default {
    name: 'ShopCards',
    props: {
        id: Number,
        text: String,
        url: String,
        img: String,
        link: String
    }
}
</script>
<template>
    <div class="card" style="width: 18rem;">
        <img :src="img" class="card-img-top" alt="...">
        <div class="card-body">
            <h5 class="card-title d-flex justify-content-center"><i class="fa-solid fa-chevron-up"></i><i
                    class="fa-solid fa-chevron-up"></i><i class="fa-solid fa-chevron-up"></i></h5>
            <p class="card-text">{{ text }}</p>
            <a :href="url">{{ link }}</a>
        </div>
    </div>
</template>
<style scoped>
i {
    color: #4154ff;
}
</style>