<script>
export default {
    name: 'Subscribeplan'
}
</script>

<template>
    <section id="subscribe-plan">
        <div class="container d-flex align-item-center justify-content-center">
            <div class="row g-3 row-col-3">
                <div class="col">
                    <div class="card text-center">
                        <img src="..." class="card-img-top" alt="...">
                        <div class="card-body">
                            <h5 class="card-title">Team training</h5>
                            <h6>Find a partner</h6>
                            <p class="card-text">Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit
                                fames amet senectus eget sed duis vehicula. Tristique.</p>
                            <p>At laoreet senectus volutpat diam vel sed sed amet pellentesque. Lobortis ut aliquam risus
                                purus. A tellus ut etiam.</p>
                            <a href="#">Find a partner <span><i class="fa-solid fa-chevron-right fa-2xs"
                                        style="color: white;"></i></span></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
#subscribe-plan {
    background-color: black;
    min-height: 500px;
}

.card {
    background-color: black;
    border: solid 3px #4154FF;
    min-height: 350px;
    max-width: 250px;
    cursor: pointer;
    margin-top: 50px;
}



h5 {
    color: white;
}

h6 {
    color: #FFF941;
}

p {
    color: white;
}

a {
    color: white;
    text-decoration: none;
}
</style>