<script>
//import components into the App.vue file
import AppHeader from './components/AppHeader.vue'
import AppJumbo from './components/AppJumbo.vue'
export default {
  name: 'App',
  components: {
    AppHeader,
    AppJumbo
  }
}

</script>

<template>
  <div id="app">
    <!-- app-header component -->
    <AppHeader />
    <!-- app-jumbo component -->
    <AppJumbo />
  </div>
</template>

<style scoped lang="scss"></style>
