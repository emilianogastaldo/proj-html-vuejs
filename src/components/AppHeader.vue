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
    <h1>SONO L'HEADER</h1>
</template>

<style lang="scss" scoped></style>
