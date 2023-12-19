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

        <div class="card-content p-2">
            <div class="image-div mb-5">
                <img :src="cardImage" :alt="cardImage" class="m-auto">

            </div>
            <div class="info">
                <h4>{{ cardTitle }}</h4>
                <hr>
                <p class="text-size pb-3">{{ cardText }}</p>
                <AppButtonComponent :buttonText="buttonText" />
            </div>
        </div>

    </div>
</template>

<style scoped lang="scss">
.app-card-white {}

.info {
    display: flex;
    flex-direction: column;
    align-items: center;

    button {
        margin-top: auto;

        &:hover {
            background-color: black;
            color: white;
        }
    }
}

.info hr {
    width: 50px;
    border: 1px solid;
    margin: 25px auto 25px auto;
}
</style>