<script>
export default {
    name: 'SubscribePlanCard'
}
</script>

<template>
    <div class="col">
        <div class="card text-center">
            <div class="icona"><i class="fa-solid fa-stopwatch fa-2xl"></i></div>
            <div class="card-body">
                <h5 class="card-title">Team training</h5>
                <h6>Find a partner</h6>
                <p class="card-text">Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit
                    fames amet senectus eget sed duis vehicula. Tristique.</p>
                <a href="#">Find a partner <span><i class="fa-solid fa-chevron-right fa-2xs"></i></span></a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    background-color: black;
    border: solid 3px #4154FF;
    min-height: 350px;
    max-width: 250px;
    cursor: pointer;
    margin-top: 50px;
}

.card:hover {
    transition: all .2s ease-in-out;
    transform: scale(1.1);
}

.icona {
    color: white;
    margin-top: 30px;
}


h5 {
    color: white;
}

h6 {
    color: #FFF941;
}

p {
    color: white;
    margin: 30px 0;
}

a {
    color: white;
    text-decoration: none;
}

i {
    color: white;
}
</style>