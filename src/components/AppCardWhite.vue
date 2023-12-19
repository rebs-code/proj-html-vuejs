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
            <div class="image-div">
                <img :src="cardImage" :alt="cardImage" class="m-auto">
                <hr>
            </div>
            <div class="info">
                <h4>{{ cardTitle }}</h4>
                <p class="text-size">{{ cardText }}</p>
                <AppButtonComponent :buttonText="buttonText" />
            </div>
        </div>

    </div>
</template>

<style scoped lang="scss">
.info {
    height: 330px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;

    button {

        &:hover {
            background-color: black;
            color: white;
        }
    }
}

.image-div hr {
    width: 50px;
    border: 1px solid;
    margin: 50px auto 50px auto;
}
</style>