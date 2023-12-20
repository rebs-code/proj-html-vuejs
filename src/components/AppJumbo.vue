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
        buttonText: String,
        buttonIcon: String,
        imageUrl: String,
        applyReverseStyle: Boolean,
    },
}
</script>

<template>
    <div class="app-jumbo" :class="{ 'reverse-style': applyReverseStyle }">
        <div class="jumbo-container container-fluid" :style="{ backgroundImage: `url(${imageUrl})` }">
            <!-- AppCardBlack component with props -->
            <AppCardBlack class="col-4" :cardIntro="cardIntro" :cardTitle="cardTitle" :cardText="cardText"
                :buttonText="buttonText" :buttonIcon="buttonIcon" applyReverseStyle />
        </div>
    </div>
</template>

<style lang="scss">
.app-jumbo {
    height: 980px;
    background-color: black;

    .jumbo-container {
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: flex-start;
        background-size: 66% 980px;
        background-repeat: no-repeat;
        background-position: right;
        padding-left: 3rem;
    }
}

// custom property to reverse passed as a prop
.reverse-style .jumbo-container {
    justify-content: flex-end;
    background-position: left;
    padding-left: 0;
}
</style>