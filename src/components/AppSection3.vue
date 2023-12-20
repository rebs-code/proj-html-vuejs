<script>
export default {
    name: 'AppSection3',
}
</script>

<template>
    <div class="section-3">
        <img src="/img/page52x.jpg" alt="Kung Pao Chicken" class="w-100">
        <h4 class="text-uppercase">Kung Pao Chicken - $32</h4>
    </div>
</template>

<style scoped lang="scss">
.section-3 {
    position: relative;

    img {
        filter: brightness(75%);
    }

    h4 {
        font-size: 1rem;
        color: white;
        position: absolute;
        bottom: 10px;
        left: 50%;
        transform: translateX(-50%);
    }
}
</style>