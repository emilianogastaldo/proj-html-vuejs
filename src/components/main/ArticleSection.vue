<script>
export default {
    name: 'ArticleSection'
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
                        <li>
                            <a href="#"><img class="img-fluid" src="../../assets/images/blog1-2x-1200x773.jpg" alt=""></a>
                            <div class="mt-3 ms-3">
                                <h5><a href="#" class="title">The best protein shake</a></h5>
                                <p>By adim | Published On: November 26th, 2019 | Gym</p>
                            </div>
                        </li>
                        <li>
                            <a href="#"><img class="img-fluid" src="../../assets/images/blog1-2x-1200x773.jpg" alt=""></a>
                            <div class="mt-3 ms-3">
                                <h5><a href="#" class="title">The best protein shake</a></h5>
                                <p>By adim | Published On: November 26th, 2019 | Gym</p>
                            </div>
                        </li>
                        <li>
                            <a href="#"><img class="img-fluid" src="../../assets/images/blog1-2x-1200x773.jpg" alt=""></a>
                            <div class="mt-3 ms-3">
                                <h5><a href="#" class="title">The best protein shake</a></h5>
                                <p>By adim | Published On: November 26th, 2019 | Gym</p>
                            </div>
                        </li>
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

    li {
        display: flex;
        flex-direction: column;
    }

}
</style>
