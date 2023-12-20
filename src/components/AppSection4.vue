<script>
import AppCardWhiteSecondaryVue from './AppCardWhiteSecondary.vue';
export default {
    name: 'AppSection4',
    components: {
        AppCardWhiteSecondaryVue
    },
}
</script>

<template>
    <section class="app-section-4">
        <!-- container -->
        <div class="container py-5">
            <div class="title d-flex flex-column align-items-center mb-5">
                <h2 class="py-5 fst-italic">Latest news & promotions</h2>
                <hr>
            </div>
            <div class="section-4-container">
                <AppCardWhiteSecondaryVue cardImg="img/blog92x-1200x1375.jpg" cardTitle="The Best Coffee in town"
                    cardText="By admin | January 7th, 2020 | Categories: News" class="me-4 card-white" />
                <AppCardWhiteSecondaryVue cardImg="img/blog72x.jpg" cardTitle="Discover our new menu"
                    cardText="By admin | January 7th, 2020 | Categories: News" class="me-4 card-white" />
                <AppCardWhiteSecondaryVue cardImg="img/blog82x-1200x1375.jpg" cardTitle="We now accept Square!"
                    cardText="By admin | January 7th, 2020 | Categories: News" class="card-white" />
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../assets/scss/partials/variables' as *;

hr {
    width: 70px;
    height: 1px;
    background-color: $silver;
}

.section-4-container {
    display: flex;
    justify-content: space-between;

    .card-white {
        width: calc(100% / 3 - 30px);
    }
}
</style>