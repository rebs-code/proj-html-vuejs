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
        <div class="header-container large-container">
            <AppHeaderLogo />
            <AppHeaderMenu />
        </div>
    </div>
</template>

<style scoped lang="scss">
.app-header {
    background-color: dodgerblue;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.header-container {
    background-color: red;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0 auto
}
</style>