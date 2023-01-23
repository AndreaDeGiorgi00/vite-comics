<script >
import AppHeader from './components/AppHeader.vue'
import AppImportant from './components/AppMain.vue'
export default {
  name: "App",
  components: { AppHeader, AppImportant }
}
</script>

<template>
  <app-header></app-header>
  <app-important></app-important>
</template>

<style lang="scss">
@use "./assets/scss/style.scss"
</style>
