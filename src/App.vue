<script >
import AppHeader from './components/AppHeader.vue'
import AppImportant from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
export default {
  name: "App",
  components: { AppHeader, AppImportant, AppFooter }
}
</script>

<template>
  <app-header></app-header>
  <app-important></app-important>
  <app-footer></app-footer>
</template>

<style lang="scss">
@use "./assets/scss/style.scss"
</style>
