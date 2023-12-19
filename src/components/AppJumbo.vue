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
    </div>
</template>

<style scoped lang="scss">
.app-jumbo {
    height: 1000px;
    background-color: black;
    padding: 2rem 0;
    background-image: url('../assets/img/slider52x.jpg');
    background-size: contain;
    background-position: right;
    background-repeat: no-repeat;
    object-fit: scale-down;
}
</style>