<script>
import AppButtonComponent from './AppButtonComponent.vue';
export default {
    name: 'AppCardWhite',
    components: {
        AppButtonComponent
    },
    props: {
        cardImage: {
            type: String,

        },
        cardTitle: {
            type: String,

        },
        cardText: {
            type: String,

        },
        buttonText: {
            type: String,

        }
    },
}
</script>

<template>
    <div class="app-card-white">

        <div class="card-content">
            <img :src="cardImage" :alt="cardImage">
            <div class="title">
                <hr>
                <h4>{{ cardTitle }}</h4>
            </div>
            <div class="info">
                <p class="text-size">{{ cardText }}</p>
                <AppButtonComponent :buttonText="buttonText" />
            </div>
        </div>

    </div>
</template>

<style scoped lang="scss"></style>