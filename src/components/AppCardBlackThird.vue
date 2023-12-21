<script>
import AppButtonComponent from './AppButtonComponent.vue';
export default {
    name: 'AppCardBlackThird',
    components: {
        AppButtonComponent
    },
    props: {
        cardTitle: {
            type: String,

        },
        cardText: {
            type: String,

        },
        cardTextSecondary: {
            type: String,

        },
        cardInfo: {
            type: String,

        },
        buttonText: {
            type: String,

        },
    }
}
</script>

<template>
    <div class="app-card-black-secondary col-5">

        <div class="card-content">
            <div class="title d-flex justify-content-between">
                <h2 class="text-uppercase fw-bold">{{ cardTitle }}</h2>
                <span class="mt-3">$52</span>
            </div>
            <hr class="my-5">
            <p class="text-size">{{ cardText }} </p>
            <AppButtonComponent :buttonText="buttonText" class="mt-3" />
        </div>
    </div>
</template>

<style scoped lang="scss">
@use '../assets/scss/partials/variables' as *;

.app-card-black-secondary {
    background-color: black;
    color: white;
    padding: 80px;

    h2 {
        font-size: 3.2rem;
    }

    hr {
        width: 70px;
        border: 1px solid white;
    }
}

button {
    color: white;

    &:hover {
        color: black;
        background-color: white;
    }
}
</style>