<script>
//import components into the App.vue file
import AppHeader from './components/AppHeader.vue'
import AppJumbo from './components/AppJumbo.vue'
import AppSection1 from './components/AppSection1.vue';
import AppSection2 from './components/AppSection2.vue';
export default {
  name: 'App',
  components: {
    AppHeader,
    AppJumbo,
    AppSection1,
    AppSection2
  }
}

</script>

<template>
  <div id="app">
    <!-- app-header component -->
    <AppHeader />
    <!-- app-jumbo component -->
    <AppJumbo cardIntro='The Best Table in Town' cardTitle='Fine dining experience'
      cardText='Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelrisque nisi in urna nulla. Sit tempor a et nisl, ac felis.'
      buttonText='Explore the menu' imageUrl='../public/img/slider52x.jpg' />
    <!-- app-section-1 component -->
    <AppSection1 />
    <!-- app section 2 component -->
    <AppJumbo class="jumbo-2" cardIntro='Fine dining experience' cardTitle='The Best Table in Town'
      cardText='Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelrisque nisi in urna nulla. Sit tempor a et nisl, ac felis.'
      buttonText='Explore the menu' />

  </div>
</template>

<style scoped lang="scss" deep>
.jumbo-2 .jumbo-container {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  background-image: url('../public/img/sushi-2.png');
  background-size: 36% 980px;
  background-repeat: repeat;
  background-position: right;
}
</style>
