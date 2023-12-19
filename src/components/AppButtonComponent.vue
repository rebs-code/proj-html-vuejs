<script>
export default {
    name: 'AppButtonComponent',
    props: {
        buttonText: {
            type: String,
        },
    }
}
</script>
<template>
    <button class="app-button">
        {{ buttonText }}
    </button>
</template>
<style scoped lang="scss">
button {
    max-width: 250px;
    background-color: transparent;
    border: 1px solid white;
    padding: 15px 30px;
    font-size: 0.8rem;
    text-transform: uppercase;
    cursor: pointer;
}
</style>