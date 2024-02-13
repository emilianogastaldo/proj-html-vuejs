<script>
export default {
    name: 'MainSpotlight'
}
</script>

<template>
    <section id="mainspotlight">
        <div class="container">
            <div class=" card-container">
                <div class="card bg-disset">
                    <div>
                        <p class="my-text-white ">Crossfit workout</p>
                        <p class="my-text-yellow">Push your limits</p>
                    </div>

                </div>

                <div class="card bg-gym-clothes">
                    <div>
                        <p class="my-text-white ">New gym appare</p>
                        <p class="my-text-yellow">Look good, feel good</p>
                    </div>

                </div>

                <div class="card bg-gym">
                    <div>
                        <p class="my-text-white ">Team training</p>
                        <p class="my-text-yellow">Find a partner</p>
                    </div>
                </div>
            </div>

            <div class="text-under-cards">
                <h1>“How you respond to the challenge in the second half will determine what you become after the game,
                    whether
                    you are a winner or a loser.”</h1>
                <img src="" alt="">
                <div>
                    <img src="" alt="">
                    <span>Brad Johnson </span>
                    <span>Las Vegas</span>
                </div>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
#mainspotlight {

    margin-top: 100px;
    // togliere questa
    background: linear-gradient(to bottom right, #0215D8, #D70110);
}

.card-container {
    display: flex;
    justify-content: space-around;
    align-items: flex-end;
    padding: 20px;
    margin-top: -20px;
}

.card div {
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: flex-end;
    height: 100%;

}

.card div p {
    text-align: start;
    margin-bottom: 0;
}

.my-text-white {
    color: #fff;
    font-size: 1.5rem;
    font-weight: 600;
}

.my-text-yellow {
    color: #FFF941;
    font-size: 1.2rem;
    font-weight: 600;
}

// CARD SECTION--------------------

.bg-disset {
    background: linear-gradient(to top, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0)), url(../../assets/images/service6-2x.jpg);
    object-fit: cover;
}

.bg-gym-clothes {
    background: linear-gradient(to top, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0)), url(../../assets/images/box1-2x.jpg);
}

.bg-gym {
    background: linear-gradient(to top, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0)), url(../../assets/images/box3-2x.jpg);
}

.card {

    height: 20rem;
    width: 18rem;
    background-color: #fff;
    border-radius: 0 0 2.5rem 0;
    box-shadow: 2px 1px 8px 8px rgb(0 0 0 / 10%);
    padding: 20px;
    margin-top: -20px;
    transition: transform 0.3s ease-out;
    margin-top: -50px;

    background-position: center;
    background-size: cover;

    filter: brightness(0.9);
    border: none;


}

.card:hover {
    transform: scale(1.05);
}

.text-under-cards {
    padding-bottom: 5rem;
    text-align: center;
    margin: 4rem 10rem 0 10rem;
    color: white;
    font-weight: 600;

}

.text-under-cards h1 {
    font-weight: 600;
}
</style>

