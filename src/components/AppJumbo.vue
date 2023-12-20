<script>
import AppCardBlack from './AppCardBlack.vue';
export default {
    name: 'AppJumbo',
    components: {
        AppCardBlack
    },
    props: {
        cardIntro: String,
        cardTitle: String,
        cardText: String,
        buttonText: String
    },
}
</script>

<template>
    <div class="app-jumbo">
        <div class="jumbo-container container-fluid px-5">
            <!-- AppCardBlack component with props -->
            <AppCardBlack class="col-4" :cardIntro="cardIntro" :cardTitle="cardTitle" :cardText="cardText"
                :buttonText="buttonText" />
            <!-- <img src="../assets/img/slider52x.jpg" alt=""> -->
        </div>
    </div>
</template>

<style scoped lang="scss">
.app-jumbo {
    height: 980px;
    background-color: black;
    // background-image: url('../assets/img/slider52x.jpg');
    // background-size: 66% 980px;
    // background-repeat: no-repeat;
    // background-position: right;
    // display: flex;
    // justify-content: center;

    // img {
    //     height: 100%;
    //     flex-grow: 1;
    // }

    .jumbo-container {
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: flex-start;
        background-image: url('../assets/img/slider52x.jpg');
        background-size: 66% 980px;
        background-repeat: no-repeat;
        background-position: right;
    }
}
</style>