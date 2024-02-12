<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
import { headerLinks, jumbrotronImage } from './data/index.js'
export default {
  name: 'AvadaFitness',
  components: { AppHeader, AppMain, AppFooter }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>
