<script>
import AppCardBlackSecondary from './AppCardBlackSecondary.vue';

export default {
    name: 'AppSection2',
    components: { AppCardBlackSecondary }
}
</script>

<template>
    <div class="app-section-2">
        <div class="container py-5">
            <h2 class="py-5 text-center">What critics are saying about us</h2>
            <hr>

            <div class="col-12 section2-top d-flex justify-content-end">
                <div class="col-6 left d-flex align-items-center justify-content-center">
                    <AppCardBlackSecondary cardCritic="Meggy Stewart" cardTitle="New York Times"
                        cardText="Non arcu mauria tortor iutrices mollis tellus euismod fermentum. Habitant amet ticindunt id sapien accusamen sed at."
                        cardTextSecondary="Mmalesuada ullamcorper amet. Pretium pretium dignissim nisi."
                        buttonText="Read full article" class="cardBlack" />
                </div>


            </div>


            <div class="col-4 try">


            </div>
            <div class="col-4 try">


            </div>
        </div>


    </div>
</template>

<style scoped lang="scss">
.cardBlack {
    width: 400px;
    height: 550px;
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
</style>