<script>
export default {
    name: 'AppCardMenu',
    props: {
        cardTitle: String,
        dishes: Array
    },
}
</script>

<template>
    <div class="card-menu p-5">
        <h2 class="text-uppercase fw-bold"> Hors douvre</h2>
        <ul>
            <li>
                <div class="d-flex align-items-center justify-content-between">
                    <h3 class="text-uppercase fw-bold mb-4">Salmon nigiri</h3>
                    <span>22$</span>
                </div>
                <p class="text-size">eget vulputate vitae quis tutrim blandit sed. quasm nullam sit lacinia</p>
            </li>
            <li>
                <div class="d-flex">
                    <h3>Salmon nigiri</h3>
                    <span>22$</span>
                </div>
                <p>eget vulputate ooooo quis tutrim blandit sed. quasm nullam sit lacinia</p>
            </li>
            <li>
                <div class="d-flex">
                    <h3>Salmon nigiri</h3>
                    <span>22$</span>
                </div>
                <p>eget vulputate vitae quis tutrim blandit sed. quasm nullam sit lacinia</p>
            </li>
            <li>
                <div class="d-flex">
                    <h3>Salmon nigiri</h3>
                    <span>22$</span>
                </div>
                <p>eget vulputate vitae quis tutrim blandit sed. quasm nullam sit lacinia</p>
            </li>
        </ul>
    </div>
</template>

<style scoped lang="scss">
.card-menu {
    h2 {
        margin-bottom: 5rem;
        font-size: 2.6rem;
    }
}

ul {
    list-style: none;
    padding: 0;
    margin: 0;

    li {
        margin-bottom: 50px;
    }
}
</style>

<!-- 970 tall 570 wide -->