<script>
export default {
    name: 'AppHeaderMenu',
    data() {
        return {
            menuItems: [
                {
                    name: 'Home',
                    link: '#'
                },
                {
                    name: 'Culinary History',
                    link: '#'
                },
                {
                    name: 'Our Team',
                    link: '#'
                },
                {
                    name: 'Our Menu',
                    link: '#'
                },
                {
                    name: 'Takeout',
                    link: '#'
                },
                {
                    name: 'Bulletin',
                    link: '#'
                },
                {
                    name: 'Reservations',
                    link: '#'
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
        margin-right: 40px;

        a {
            color: $silver;
            text-decoration: none;

            &:hover {
                text-decoration: underline;
                color: white;
            }
        }
    }
}
</style>