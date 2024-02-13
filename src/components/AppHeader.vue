<script>
import Navbar from './Navbar.vue'
import Jumbotron from './Jumbotron.vue'
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
