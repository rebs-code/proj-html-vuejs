<script>
import AppFooterTop from './AppFooterTop.vue';
import AppFooterBottom from './AppFooterBottom.vue';
export default {
    name: 'AppFooter',
    components: {
        AppFooterTop,
        AppFooterBottom
    },
}
</script>

<template>
    <div class="footer">
        <AppFooterTop />
        <AppFooterBottom />
    </div>
</template>

<style scoped lang="scss"></style>
