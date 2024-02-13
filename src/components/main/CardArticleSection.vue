<script>
export default {
    name: 'CardArticleSection',
    props: {
        article: Object
    },
    computed: {
        articleImg() {
            return new URL(`../../assets/images/${this.article.img}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <li>
        <a :href="article.url"><img class="img-fluid" :src="articleImg" :alt="article.alt"></a>
        <div class="mt-3 ms-3">
            <h5><a href="#" class="title">{{ article.title }}</a></h5>
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
</style>
