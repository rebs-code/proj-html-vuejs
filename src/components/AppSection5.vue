<script>
import AppCardBlackThird from './AppCardBlackThird.vue';
export default {
    name: 'AppSection5',
    data() {
        return {
            card:
            {
                cardTitle: 'Braised Abalone',
                cardText: 'Pretium accumsan portittor viverra leo gravida millis imperdiet. Fringilla nibh pharetra sociis leo amet.',
                buttonText: 'View in the menu',
            }

        }
    },
    components: {
        AppCardBlackThird
    },
}
</script>

<template>
    <div class="section-5">
        <div class="container-fluid">
            <AppCardBlackThird :cardTitle="card.cardTitle" :cardText="card.cardText" :buttonText="card.buttonText" />
        </div>

    </div>
</template>

<style scoped lang="scss">
.section-5 {
    padding: 150px 170px 120px 170px;
    background-image: url('../public/img/braised-abalone.jpg');
    background-size: cover;
}
</style>