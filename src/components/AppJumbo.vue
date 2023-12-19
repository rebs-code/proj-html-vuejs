<script>
import AppCardBlack from '../AppCardBlack.vue';
export default {
    name: 'AppJumbo',
    data() {
        return {
            cardIntro: 'The Best Table in Town',
            cardTitle: 'Fine dining experience',
            cardText: 'Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelrisque nisi in urna nulla. Sit tempor a et nisl, ac felis.',
            buttonText: 'Explore the menu'
        }
    },
    components: {
        AppCardBlack
    }
}
</script>

<template>
    <div class="app-jumbo">
        <AppCardBlack :cardIntro="cardIntro" :cardTitle="cardTitle" :cardText="cardText" :buttonText="buttonText" />
        <img src="../assets/img/slider52x.jpg" alt="">
    </div>
</template>

<style scoped lang="scss">
.app-jumbo {
    height: 980px;
    background-color: black;
    display: flex;
    align-items: center;

    img {
        height: 100%;
    }
}
</style>