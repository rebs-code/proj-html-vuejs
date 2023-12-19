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
            <div>
                <img :src="cardImage" :alt="cardImage" class="m-auto">
            </div>

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

<style scoped lang="scss">
.info {
    button {
        &:hover {
            background-color: black;
            color: white;
        }
    }

    p {
        margin-bottom: 50px;
    }
}

.title hr {
    width: 50px;
    border: 1px solid;
    margin: 50px auto 50px auto;
}
</style>