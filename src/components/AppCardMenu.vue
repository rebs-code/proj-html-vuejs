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
        <h2 class="text-uppercase fw-bold"> {{ cardTitle }}</h2>
        <ul>
            <li v-for="dish in dishes">
                <div class="d-flex align-items-center justify-content-between">
                    <h3 class="text-uppercase fw-bold mb-4">{{ dish.name }}</h3>
                    <span>{{ dish.price }}</span>
                </div>
                <p class="text-size">{{ dish.description }}</p>
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