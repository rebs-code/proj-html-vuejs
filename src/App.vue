<script>
//import components into the App.vue file
import AppHeader from './components/AppHeader.vue'
export default {
  name: 'App',
  components: {
    AppHeader
  }
}

</script>

<template>
  <div id="app">
    <!-- app-header component -->
    <AppHeader />
  </div>
</template>

<style scoped lang="scss"></style>
