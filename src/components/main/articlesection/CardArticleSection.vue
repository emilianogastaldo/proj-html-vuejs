<script>
export default {
    name: 'CardArticleSection',
    props: {
        article: Object
    },
    computed: {
        articleImg() {
            return new URL(`../../../assets/images/${this.article.img}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <li>
        <a :href="article.url">
            <div class="position-relative">
                <img class="img-fluid" :src="articleImg" :alt="article.alt">
                <div class="overlay"></div>
            </div>
            <h5 class="title mt-3 ms-3">{{ article.title }}</h5>
        </a>
        <div class="ms-3">
            <p>By {{ article.creator }} | Published On: {{ article.date }} | {{ article.subject }}</p>
        </div>
    </li>
</template>

<style lang="scss" scoped>
.title {
    font-weight: 600;
}

a {
    text-decoration: none;
    color: black;
}

.overlay {
    position: absolute;
    background: linear-gradient(to bottom, rgba(0, 0, 0, 0) 0%, rgba(65, 84, 255, 0.6) 100%);
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    display: none;
}

a:hover .overlay {
    display: block;
}
</style>
