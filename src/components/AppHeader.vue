<script>
//import components into the AppHeader.vue file
import AppHeaderLogo from './AppHeaderLogo.vue'
import AppHeaderMenu from './AppHeaderMenu.vue'

export default {
    name: 'AppHeader',
    components: {
        AppHeaderLogo,
        AppHeaderMenu
    }
}


</script>

<template>
    <div class="app-header">
        <div class="header-container container-fluid px-5">
            <AppHeaderLogo />
            <AppHeaderMenu />
        </div>
    </div>
</template>

<style scoped lang="scss">
.app-header {
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
}

.header-container {
    height: 160px;
    display: flex;
    align-items: center;
    padding: 1rem 1rem;
}
</style>