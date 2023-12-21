<script>
export default {
    name: 'AppCardMenu',
    props: {
        cardTitle: String,
        dishes: Array,
        bgImage: String,
    },
    //if bgImage is not empty, then it's used as a background image
    computed: {
        backgroundStyle() {
            return this.bgImage
                ? {
                    background: `linear-gradient(to bottom, rgba(0, 0, 0, 1) 0%, rgba(0, 0, 0, 1) 20%, rgba(0, 0, 0, 0) 100%), url(${this.bgImage})`,
                    backgroundSize: 'cover'
                }
                : { backgroundColor: '#e8e8e8' };
        }
    }
}
</script>

<template>
    <!-- style is backgroundStyle -->
    <div class="card-menu p-5" :style="backgroundStyle">
        <h2 class="text-uppercase fw-bold"> {{ cardTitle }}</h2>
        <ul>
            <li v-for="dish in dishes">
                <div class="d-flex align-items-center justify-content-between mb-4">
                    <h3 class="text-uppercase fw-bold">{{ dish.name }}</h3>
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