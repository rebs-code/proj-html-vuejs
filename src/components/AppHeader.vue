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

<style scoped lang="scss"></style>