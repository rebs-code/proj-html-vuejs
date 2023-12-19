<script>
//import components into the App.vue file
import AppHeader from './components/AppHeader.vue'
import AppJumbo from './components/AppJumbo.vue'
import AppSectionOne from './components/AppSectionOne.vue';
export default {
  name: 'App',
  components: {
    AppHeader,
    AppJumbo,
    AppSectionOne
  }
}

</script>

<template>
  <div id="app">
    <!-- app-header component -->
    <AppHeader />
    <!-- app-jumbo component -->
    <AppJumbo />
    <!-- app-section-one component -->
    <AppSectionOne />

  </div>
</template>

<style scoped lang="scss"></style>
