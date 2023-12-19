<script>
import AppCardBlack from '../AppCardBlack.vue';
export default {
    name: 'AppJumbo',
    components: {
        AppCardBlack
    }
}
</script>

<template>
    <div class="app-jumbo">
        <AppCardBlack />
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