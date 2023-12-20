<script>
import AppButtonComponent from './AppButtonComponent.vue';
export default {
    name: 'AppCardBlack',
    components: {
        AppButtonComponent
    },
    props: {
        cardIntro: {
            type: String,

        },
        cardTitle: {
            type: String,

        },
        cardText: {
            type: String,

        },
        cardInfo: {
            type: String,

        },
        buttonText: {
            type: String,

        }
    }
}
</script>

<template>
    <div class="app-card-black">

        <div class="card-content">
            <div class="title">
                <hr>
                <h4>{{ cardIntro }}</h4>
            </div>
            <div class="info">
                <h2>{{ cardTitle }}</h2>
                <p class="text-size">{{ cardText }}</p>
                <AppButtonComponent :buttonText="buttonText" />
            </div>

        </div>

    </div>
</template>

<style scoped lang="scss">
.app-card-black {
    background-color: transparent;
}

.card-content {
    color: white;
    padding: 2rem;
    padding-left: 0;

    h2 {
        font-size: 3.2rem;
        margin-bottom: 70px;
        text-transform: uppercase;
    }

    p {
        margin-bottom: 70px;
    }

    .title {
        display: flex;
        align-items: center;
        margin-bottom: 70px;

        hr {
            border: 1px solid white;
            width: 70px;
        }

        h4 {
            margin-left: 30px;
            font-size: 1.1rem;
        }
    }

    .info {
        margin-left: 100px;

        button {
            color: white;

            &:hover {
                background-color: white;
                color: black;
            }
        }
    }
}
</style>