<script>
import Navbar from './header/Navbar.vue'
import Jumbotron from './header/Jumbotron.vue'
export default {
    name: 'AppHeader'
    , components: {
        Navbar,
        Jumbotron
    }
}
</script>

<template>
    <!-- Amarildo -->
    <Navbar />
    <Jumbotron />
</template>

<style lang="scss" scoped></style>
