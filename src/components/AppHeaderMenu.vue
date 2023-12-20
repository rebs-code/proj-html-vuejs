<script>
export default {
    name: 'AppHeaderMenu',
    data() {
        return {
            menuItems: [
                {
                    name: 'Home',
                    link: '#',
                    isNew: false
                },
                {
                    name: 'Culinary History',
                    link: '#',
                    isNew: false
                },
                {
                    name: 'Our Team',
                    link: '#',
                    isNew: false
                },
                {
                    name: 'Our Menu',
                    link: '#',
                    isNew: false
                },
                {
                    name: 'Takeout',
                    link: '#',
                    isNew: true
                },
                {
                    name: 'Bulletin',
                    link: '#',
                    isNew: false
                },
                {
                    name: 'Reservations',
                    link: '#',
                    isNew: false
                },
            ]
        }
    }
}
</script>

<template>
    <ul>
        <li v-for="item in menuItems">
            <a :href="item.link" v-html="item.name"></a>
            <span v-if="item.isNew">New</span>
        </li>
        <li> <a href="#"><font-awesome-icon icon="fa-solid fa-cart-shopping" /></a></li>
    </ul>
</template>

<style scoped lang="scss">
@use '../assets/scss/partials/variables' as *;

ul {
    display: flex;
    margin-left: auto;

    li {
        margin-right: 30px;
        display: flex;
        align-items: center;

        a {
            color: $silver;
            text-decoration: none;
            font-size: 1.2rem;

            &:hover {
                text-decoration: underline;
                color: white;
            }
        }

        span {
            color: $silver;
            font-size: 0.7rem;
            font-weight: 700;
            padding: 0.1rem;
            margin-left: 5px;
            border: 1px solid $silver;
        }
    }
}
</style>