<script>
import AppButtonComponent from './AppButtonComponent.vue';
export default {
    name: 'AppCardBlackSecondary',
    components: {
        AppButtonComponent
    },
    props: {
        cardCritic: {
            type: String,

        },
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
    <div class="app-card-black-secondary">

        <div class="card-content">
            <h4>{{ cardCritic }}</h4>
            <h2 class="fw-bold">{{ cardTitle }}</h2>
            <span v-for="n in 5" class="me-1"><font-awesome-icon icon="fa-solid fa-star" /></span>
            <hr class="my-5">
            <p class="text-size">{{ cardText }} </p>
            <p class="text-size">{{ cardTextSecondary }} </p>
            <AppButtonComponent :buttonText="buttonText" class="mt-3" />
        </div>
    </div>
</template>

<style scoped lang="scss">
@use '../assets/scss/partials/variables' as *;

.app-card-black-secondary {

    color: white;
}


h4 {
    font-size: 1.1rem;
    margin-bottom: 40px;
    text-transform: uppercase;
    color: $silver;
}

h2 {
    font-size: 2.8rem;
    margin-bottom: 40px;
    text-transform: uppercase;
}

p {
    margin-bottom: 30px;
}

hr {
    border: 1px solid white;
    width: 70px;
}

button {
    color: white;

    &:hover {
        color: black;
        background-color: white;
    }
}
</style>