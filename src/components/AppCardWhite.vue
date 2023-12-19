<script>
export default {
    name: 'AppCardWhite',
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
                <button>{{ buttonText }}</button>
            </div>
        </div>

    </div>
</template>

<style scoped lang="scss"></style>