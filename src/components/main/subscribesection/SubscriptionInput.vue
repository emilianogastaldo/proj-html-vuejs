<script>
import AppButton from '../../AppButton.vue';
export default {
    name: 'SubscribtionInput',
    components: { AppButton },
    data: () => ({
        email: ''
    })
}
</script>

<template>
    <div class="image d-flex align-items-center py-5">
        <div class="container">
            <h4>Join our mailing list today</h4>
            <h1> Insider offers & flash sales in your<br>
                inbox every week.</h1>
            <span><i v-for="n in 3" class="fas fa-chevron-up color-yellow"></i></span>
            <div class="mb-3">
                <input type="email" @keyup.enter="email = ''" placeholder="Insert your email ...*" v-model.trim="email">
                <AppButton @click="email = ''" class="ms-4 btn-large">
                    Subscribe
                </AppButton>
            </div>
            <p>Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet, consectetur<br> adipiscing
                elit
                sed porttitor lectus.</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.image {
    background: linear-gradient(to right,
            rgba(0, 0, 0, 1) 36%,
            rgba(0, 0, 0, 0) 100%),
        url("../../../assets/images/banner1-2x.jpg");
    background-size: cover;
    background-repeat: no-repeat;
}

h4 {
    color: #FF414B;
}

h1 {
    margin: 20px 0;
    color: white;
    font-size: 50px;
}

input {
    margin: 20px 0;
    border: solid 1px black;
    border-radius: 40px;
    padding: 17px 40px;
    width: 550px;
}


p {
    margin-top: 20px;
    color: #98939F;
    font-size: 23px;
}

.color-yellow {
    color: #FFF941;
}
</style>