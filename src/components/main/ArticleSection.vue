<script>
import { articleDatas } from '../../data/index.js';
import CardArticleSection from './CardArticleSection.vue';
export default {
    name: 'ArticleSection',
    data: () => ({
        articleDatas
    }),
    components: {
        CardArticleSection
    }

}
</script>

<template>
    <section id="lastest-articles">
        <div class="container">
            <div class="row">
                <div class="col-6">
                    <h4 class="title">Latest articles</h4>
                </div>
                <div class="col-6">
                    <div class="text-end">
                        <a class="title" href="#">Read all articles <i class="fas fa-angle-right"></i></a>
                    </div>
                </div>
                <div class="col-12">
                    <ul class="d-flex gap-5 mt-4">
                        <CardArticleSection v-for="article in articleDatas" :key="article.id" :article="article" />
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.title {
    font-weight: 600;
}

a {
    text-decoration: none;
    color: black;
}

ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}
</style>
