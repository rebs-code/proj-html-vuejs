<script>
//import components into the AppHeader.vue file
import AppHeaderLogo from './AppHeaderLogo.vue'
import AppHeaderMenu from './AppHeaderMenu.vue'

export default {
    name: 'AppHeader',
    components: {
        AppHeaderLogo
    }
}


</script>

<template>
    <div class="app-header">
        <AppHeaderLogo />
        <AppHeaderMenu />
    </div>
</template>

<style scoped lang="scss">
.app-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
    height: 80px;
    background-color: dodgerblue;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
</style>