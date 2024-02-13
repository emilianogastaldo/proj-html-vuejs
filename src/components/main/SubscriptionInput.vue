<script>
export default {
    name: 'SubscribtionInput'
}
</script>

<template>
    <div class="image d-flex align-items-center">
        <div class="container">
            <h4>Join our mailing list today</h4>
            <h1> Insider offers & flash sales in your<br>
                inbox every week.</h1>
            <span><i class="fa-solid fa-chevron-up" style="color: #FFF941;"></i><i class="fa-solid fa-chevron-up"
                    style="color: #FFF941;"></i><i class="fa-solid fa-chevron-up" style="color: #FFF941;"></i></span>
            <div class="mb-3">
                <input type="email" placeholder="Insert your email ...*">
                <button>Subscribe</button>
            </div>
            <p>Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet, consectetur<br> adipiscing
                elit
                sed porttitor lectus.</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.image {
    min-height: 800px;
    background-image: url("../../assets/images/banner1-2x.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    width: 100%;
    height: auto;
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

p {
    margin-top: 20px;
    color: #85939f;
    font-size: 23px;
}
</style>