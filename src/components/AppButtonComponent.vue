<script>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faCar } from '@fortawesome/free-solid-svg-icons'
export default {
    name: 'AppButtonComponent',
    props: {
        buttonText: {
            type: String,
        },
        buttonIcon: {
            type: Object,
        },
    },
    components: {
        FontAwesomeIcon,
    },
    data() {
        return {
            faCar: faCar
        }
    },
}
</script>
<template>
    <button class="app-button">
        <font-awesome-icon :icon="buttonIcon" />
        {{ buttonText }}
    </button>
</template>
<style scoped lang="scss">
button {
    max-width: 250px;
    background-color: transparent;
    border: 1px solid;
    padding: 15px 30px;
    font-size: 0.8rem;
    text-transform: uppercase;
    cursor: pointer;
}
</style>