<script>
import AppCardMenu from './AppCardMenu.vue';
export default {
    name: 'AppSectionMenu',
    data() {
        return {
            menuItems: [
                {
                    cardTitle: 'Hors d\'ouvres',
                    dishes: [
                        {
                            name: 'Ahi salmon nigiri',
                            description: 'Eget vulputate vitae quis rutrum blandit sed. Quam nulla sit lacinia.',
                            price: '$48'
                        },
                        {
                            name: 'Umi masu salad',
                            description: 'Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.',
                            price: '$21'
                        },
                        {
                            name: 'Temaki with crab',
                            description: 'Ac vel, risus orrnare senectus placerat duis amet dictumst tellus.',
                            price: '$22'
                        },
                        {
                            name: 'California Roll',
                            description: 'Ac vel, risus orrnare senectus placerat duis amet dictumst tellus.',
                            price: '$22'
                        },
                    ]
                },
                {
                    cardTitle: 'Main course',
                    dishes: [
                        {
                            name: 'Braised Abalone',
                            description: 'Eget vulputate vitae quis rutrum blandit sed. Quam nulla sit lacinia.',
                            price: '$52'
                        },
                        {
                            name: 'Twice cooked pork',
                            description: 'Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.',
                            price: '$21'
                        },
                        {
                            name: 'Kung pao chicken',
                            description: 'Ac vel, risus orrnare senectus placerat duis amet dictumst tellus.',
                            price: '$32'
                        },
                        {
                            name: 'Char sui & sushis',
                            description: 'Ac vel, risus orrnare senectus placerat duis amet dictumst tellus.',
                            price: '$48'
                        },
                    ]
                },
                {
                    cardTitle: 'Desserts',
                    dishes: [
                        {
                            name: 'Chocolate ball cake',
                            description: 'Eget vulputate vitae quis rutrum blandit sed. Quam nulla sit lacinia.',
                            price: '$13'
                        },
                        {
                            name: 'Lime pie with crust',
                            description: 'Mollis ornare sit sapien, sodales. Cursus duis proin semper quisque.',
                            price: '$14'
                        },
                        {
                            name: 'Raspberry pear cake',
                            description: 'Ac vel, risus orrnare senectus placerat duis amet dictumst tellus.',
                            price: '$32'
                        },
                        {
                            name: 'Café au lait',
                            description: 'Ac vel, risus orrnare senectus placerat duis amet dictumst tellus.',
                            price: '$6'
                        },
                    ]
                },

            ],
        }
    },
    components: {
        AppCardMenu,
    },
}
</script>

<template>
    <div class="menu-container">
        <AppCardMenu class="col-3" :cardTitle="menuItems[0].cardTitle" :dishes="menuItems[0].dishes" />
        <AppCardMenu class="col-3" :cardTitle="menuItems[1].cardTitle" :dishes="menuItems[1].dishes" />
        <AppCardMenu class="col-3" :cardTitle="menuItems[2].cardTitle" :dishes="menuItems[2].dishes" />
    </div>
</template>

<style scoped lang="scss">
.menu-container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 1200px;
}
</style>