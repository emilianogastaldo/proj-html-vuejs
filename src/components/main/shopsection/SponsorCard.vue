<script>
export default {
    name: 'SponsorCard',
    props: {
        id: Number,
        text: String,
        url: String,
        img: String,
        link: String
    },
    computed: {
        imagePath() {
            const path = new URL(`../../../assets/images/${this.img}`, import.meta.url);
            return path.href;
        }
    }
}
</script>
<template>
    <div class="card">
        <a :href="url">
            <img :src="imagePath" class="card-img-top" :alt="link">
            <div class="card-body">
                <h5 class="card-title d-flex justify-content-center"><i class="fa-solid fa-chevron-up"></i><i
                        class="fa-solid fa-chevron-up"></i><i class="fa-solid fa-chevron-up"></i></h5>
                <p class="card-text mt-3">{{ text }} </p>
                <span class="d-flex align-items-center justify-content-center gap-2">{{ link }} <i
                        class="fa-solid fa-chevron-right"></i>
                </span>

            </div>
        </a>
    </div>
</template>
<style scoped>
.card {
    border-color: transparent;
}

h5 i {
    color: #4154ff;
}

a {
    color: black;
    text-decoration: none;
}

span {
    font-weight: 600;
    margin-top: 50px
}

p {
    font-size: 1.2rem;
    color: #88828f
}

img {
    display: block;
    margin: 0 auto;
    width: 50%;
}
</style>