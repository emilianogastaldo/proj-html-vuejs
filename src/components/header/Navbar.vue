<script>
import AppButton from '../AppButton.vue';
import headerLinks from '../../data/_headerLinks';
export default {
    name: 'Navbar',
    data() {
        return {
            headerLinks: headerLinks,
            showSearchBar: false, // variabile show su non visibile
            search: '',
        };
    },
    components: { AppButton },
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
                <a href="#"><img src="../../assets/images/logo.png" alt="Logo" /></a>
            </div>

            <div class="">
                <ul v-if="!showSearchBar">
                    <li v-for="link in headerLinks" :key="link.text">
                        <a :href="link.url" :class="{ 'active': link.current }">{{ link.text }}
                            <span class="badge bg">{{ link.badge }}</span></a>

                        <!-- <template v-if="link.text !== 'Home'">
                            <Dropdown :options="dropdownOptions" />
                        </template> -->
                    </li>
                    <AppButton @click="goToSchedule" class="btn-small">
                        Schedule a workout
                    </AppButton>
                    <i class="icon fa fa-search" @click="toggleSearchBar"></i>
                    <i class="icon fa-solid fa-cart-shopping" @click="goToCart"></i>

                </ul>

                <!-- Barra di ricerca -->
                <div class="search-bar" :class="{ 'active': showSearchBar }">
                    <div class=" d-flex">
                        <input v-model="search" class="form-control" id="exampleFormControlInput1" placeholder="Search..."
                            @keyup.enter="search = ''">
                        <i class="icon fa fa-search search-icon" @click="search = ''"></i>
                        <i class="icon fa fa-times " @click="toggleSearchBar"></i>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
// SEARCHBAR SECTION
.search-bar {
    background-color: #060607;

    z-index: 1;
    display: none;
    border-radius: 15px;
    padding: 5px;
    align-items: center;

    .search-input {
        flex-grow: 1;
        border: none;
        border-radius: 10px;
        padding: 8px;
        margin-right: 10px;
    }

    .search-icon {
        color: white;
        border-radius: 0 20px 20px 0;
        cursor: pointer;
    }

    .search-icon:hover {
        background-color: #152cff;
    }

    .form-control {
        width: 40rem;
        border-radius: 20px 0px 0px 20px;
    }
}

.search-bar.active {
    display: block;
}

.fa-search:hover {
    color: white;
}

// NAVBAR SECTION-------------------
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

.icon {
    padding: 0.8rem;
    color: #98939F;
    cursor: pointer;
}

// BADGE
.bg {
    background-color: #FFF941;
    color: #060607;
    font-weight: 600;
}
</style>