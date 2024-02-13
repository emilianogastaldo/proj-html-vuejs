<script>
export default {
    name: 'AppHeader',
}
</script>

<template>
    <button>
        <slot></slot>
    </button>
</template>

<style lang="scss" scoped>
button {
    padding: 17px 40px;
    border-radius: 50px;
    background-color: transparent;
    border: 1px solid currentColor;
}

button:hover {
    background-color: #FF414B;
}
</style>
