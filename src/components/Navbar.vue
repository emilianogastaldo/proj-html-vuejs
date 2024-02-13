<script>
export default {
    name: 'Navbar'
}
</script>

<template>
    <!-- Amarildo -->

    <div class="navbar d-flex">
        <div class="d-flex justify-content-between container">
            <div>
                <img src="../assets/images/logo.png" alt="Logo" />
            </div>

            <div class="">
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Services</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">Blog</a></li>
                    <li><a href="#">Store</a></li>
                    <button>Schedule a workout</button>
                    <i class="icon fa-solid fa-cart-shopping"></i>
                    <i class="icon fa fa-search"></i>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.navbar {
    background-color: #060607;
}

.navbar img {
    height: 50px;
    padding: 10px;
}

.navbar ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}

.navbar li {
    display: inline-block;
}

.navbar a {
    font-weight: 600;
    display: block;
    color: #98939F;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
}

.navbar a:hover {

    color: #FFFFFF;
}



.navbar button {
    font-weight: 600;
    background-color: #4154FF;
    color: white;
    border-radius: 2rem;
    border: none;
    padding: 10px 20px;
    display: inline-block;
    font-size: 14px;
    cursor: pointer;
}

.navbar button:hover {
    background-color: #152cff;
}

.icon {
    padding: 0.8rem;
    color: #98939F;
}
</style>
