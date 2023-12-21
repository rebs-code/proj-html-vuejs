<script>
export default {
    name: 'AppFooterBottom',
}
</script>

<template>
    <div class="footer-bottom d-flex align-items-center justify-content-center">
        <p class="text-size mb-0">Copyright 2012 - 2019 Avada | All rights Reserved | Powered by <span
                class="fw-bold text-white">WordPress | ThemeFusion</span>
        </p>
    </div>
</template>

<style scoped lang="scss">
@use '../assets/scss/partials/variables' as *;

.footer-bottom {
    padding: 30px;
    background-color: black;

    p {
        color: $silver;
        font-size: 1rem
    }

    ;
}
</style>