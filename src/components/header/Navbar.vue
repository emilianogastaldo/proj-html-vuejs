<script>

import headerLinks from '../../data/_headerLinks';
export default {
    name: 'Navbar',
    data() {
        return {
            headerLinks: headerLinks,
            showSearchBar: false, // variabile show su non visibile
        };
    },
    methods: {
        goToSchedule() {
            window.location.href = 'https://avada.website/fitness/contact/';
        },
        goToCart() {
            window.location.href = 'https://avada.website/fitness/cart/';
        },
        toggleSearchBar() {
            // Inverto lo stato di showSearchBar al click sull'icona
            this.showSearchBar = !this.showSearchBar;
        },
    },
};
</script>

<template>
    <!-- Amarildo -->

    <div class="navbar d-flex">
        <div class="d-flex justify-content-between container">
            <div>
                <img src="../../assets/images/logo.png" alt="Logo" />
            </div>

            <div class="">
                <ul>
                    <li v-for="link in headerLinks" :key="link.text">
                        <a :href="link.url" :class="{ 'active': link.current }">{{ link.text }}</a>

                        <!-- <template v-if="link.text !== 'Home'">
                            <Dropdown :options="dropdownOptions" />
                        </template> -->
                    </li>
                    <button @click="goToSchedule">Schedule a workout</button>
                    <i class="icon fa-solid fa-cart-shopping" @click="goToCart"></i>
                    <i class="icon fa fa-search" @click="toggleSearchBar"></i>
                </ul>

                <!-- Barra di ricerca -->
                <div class="search-bar" :class="{ 'active': showSearchBar }">
                    <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="name@example.com">
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.search-bar {
    position: fixed;
    top: 70px;
    left: 0;
    width: 100%;
    background-color: #fff;
    z-index: 1;
    display: none;
}

.search-bar.active {
    display: block;
}

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
    cursor: pointer;
}
</style>
