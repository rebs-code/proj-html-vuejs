<script>
//import components into the App.vue file
import AppHeader from './components/AppHeader.vue'
import AppJumbo from './components/AppJumbo.vue'
import AppSection1 from './components/AppSection1.vue';
import AppSection2 from './components/AppSection2.vue';
import AppSection3 from './components/AppSection3.vue';
import AppSection4 from './components/AppSection4.vue';
import { faCar } from '@fortawesome/free-solid-svg-icons'
import AppSectionMenu from './components/AppSectionMenu.vue';
import AppSection5 from './components/AppSection5.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  name: 'App',
  components: {
    AppHeader,
    AppJumbo,
    AppSection1,
    AppSection2,
    AppSection3,
    AppSection4,
    AppSectionMenu,
    AppSection5,
    AppFooter

  },
  data() {
    return {
      faCar: faCar
    }
  },
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
    <!-- jumbo repeat component -->
    <AppJumbo class="jumbo-2" cardIntro='Fine dining experience' cardTitle='The Best Table in Town'
      cardText='Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelrisque nisi in urna nulla. Sit tempor a et nisl, ac felis.'
      buttonText='Explore the menu' imageUrl='../public/img/slider32x.jpg' applyReverseStyle />
    <!-- app section 2 component -->
    <AppSection2 />
    <!-- app section 3 component -->
    <AppSection3 />
    <!-- app section 4 component -->
    <AppSection4 />
    <!-- jumbo component repeats -->
    <AppJumbo cardIntro='Enjoy your meal at home' cardTitle='Takeout now available'
      cardText='Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelrisque nisi in urna nulla. Sit tempor a et nisl, ac felis.'
      buttonText='View Takeout Menu' :buttonIcon='faCar' imageUrl='img/slider72x-scaled.jpg' class="jumbo-3"
      applyReverseStyle />
    <!-- app section menu -->
    <AppSectionMenu />
    <!-- app section 5 -->
    <AppSection5 />
    <!-- app footer component -->
    <AppFooter />
  </div>
</template>

<style scoped lang="scss">
#app {
  max-width: 3000px;
  margin: 0 auto;
  border: 1px solid black;
}

.jumbo-2 {
  height: 880px;
}

.jumbo-3 {
  height: 880px;
}
</style>
