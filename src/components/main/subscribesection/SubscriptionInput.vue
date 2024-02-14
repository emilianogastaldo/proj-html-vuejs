<script>
export default {
    name: 'SubscribtionInput',
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
            <span><i class="fa-solid fa-chevron-up" style="color: #FFF941;"></i><i class="fa-solid fa-chevron-up"
                    style="color: #FFF941;"></i><i class="fa-solid fa-chevron-up" style="color: #FFF941;"></i></span>
            <div class="mb-3">
                <input type="email" placeholder="Insert your email ...*" v-model.trim="email">
                <button @click="email = ''">Subscribe</button>
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
    border-radius: 12px;
    padding: 5px 10px;
    width: 400px;
}

button {
    margin-left: 30px;
    background-color: #4154FF;
    color: white;
    border: solid 1px transparent;
    border-radius: 15px;
    padding: 5px 10px;
    width: 200px;
}

button:hover {
    background-color: #FF414B;
    transition: all .2s ease-in-out;
}

p {
    margin-top: 20px;
    color: #98939F;
    font-size: 23px;
}
</style>