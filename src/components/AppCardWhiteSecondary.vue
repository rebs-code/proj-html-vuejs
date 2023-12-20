<script>
export default {
    name: 'AppCardWhiteSecondary',
    props: {
        cardImg: {
            type: String,

        },
        cardTitle: {
            type: String,

        },
        cardText: {
            type: String,

        },
    }

}
</script>

<template>
    <div class="app-card-white-secondary text-center">
        <img :src="cardImg" alt="Kung Pao Chicken" class="w-100 mb-4">
        <h4 class="text-uppercase mb-3 fw-bold">{{ cardTitle }}</h4>
        <h6>{{ cardText }}</h6>
    </div>
</template>

<style scoped lang="scss">
h6 {
    font-size: 1rem;
    font-weight: 400;
}
</style>