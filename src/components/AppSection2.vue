<script>
import AppCardBlackSecondary from './AppCardBlackSecondary.vue';

export default {
    name: 'AppSection2',
    components: { AppCardBlackSecondary }
}
</script>

<template>
    <section class="app-section-2">
        <!-- container -->
        <div class="container py-5">
            <div class="title d-flex flex-column align-items-center mb-5">
                <h2 class="py-5 fst-italic">What critics are saying about us</h2>
                <hr class="hr">
            </div>
            <!-- top section -->
            <div class="col-12 section2-top d-flex justify-content-end">
                <div class="col-6 left d-flex align-items-center justify-content-center">
                    <AppCardBlackSecondary cardCritic="Meggy Stewart" cardTitle="New York Times"
                        cardText="Non arcu mauria tortor iutrices mollis tellus euismod fermentum. Habitant amet ticindunt id sapien accusamen sed at."
                        cardTextSecondary="Mmalesuada ullamcorper amet. Pretium pretium dignissim nisi."
                        buttonText="Read full article" class="cardBlack" />
                </div>
            </div>
            <!-- bottom section -->
            <div class="col-12 section2-bottom">
                <div class="bottom-card card-1">
                    <AppCardBlackSecondary cardCritic="Mary Maxey" cardTitle="The Guardian"
                        cardText="Non arcu mauria tortor iutrices mollis tellus euismod fermentum. Habitant amet ticindunt id sapien accusamen sed at."
                        buttonText="Read full article" class="cardBlack" />

                </div>
                <div class="bottom-card">
                    <AppCardBlackSecondary cardCritic="Patrick Monroe" cardTitle="Globe and Mail"
                        cardText="Non arcu mauria tortor iutrices mollis tellus euismod fermentum. Habitant amet ticindunt id sapien accusamen sed at."
                        buttonText="Read full article" class="cardBlack" />
                </div>
            </div>


        </div>


    </section>
</template>

<style scoped lang="scss">
@use '../assets/scss/partials/variables' as *;

.cardBlack {
    width: 400px;
    height: 550px;
}

.hr {
    width: 70px;
    height: 1px;
    background-color: $silver;
}

.section2-top {
    height: 840px;
    background-image: url('../public/img/blog72x.jpg');
    background-repeat: no-repeat;
    background-size: 50% 100%;
    background-position: left;

    .left {
        background-color: black;
    }
}

.section2-bottom {
    height: 715px;
    display: flex;
    justify-content: space-between;
    margin-top: 60px;

    .bottom-card {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 47%;
    }

    &> :first-child {
        background-image: linear-gradient(to bottom, rgba(0, 0, 0, 1) 0%, rgba(0, 0, 0, 1) 20%, rgba(0, 0, 0, 0) 100%), url('../public/img/info52x.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;

    }

    &> :nth-child(2) {
        background-image: linear-gradient(to bottom, rgba(0, 0, 0, 1) 0%, rgba(0, 0, 0, 1) 20%, rgba(0, 0, 0, 0) 100%), url('../public/img/info12x.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
    }
}
</style>