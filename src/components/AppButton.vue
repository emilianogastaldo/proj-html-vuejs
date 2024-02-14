<script>
export default {
    name: 'AppButton'
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
    background-color: #4145ff;
    border: 1px solid transparent;
    color: white;
    font-weight: 500;
}

.btn-large {
    width: 260px;
}

.btn-small {
    padding: 10px 15px;
    font-size: 14px;
}

.btn-transparent {
    background-color: transparent;
    color: #98939F;
    border: 1px solid currentColor;
}

.color-white {
    color: white
}

.bg-color-red {
    background-color: red;
}

.bg-color-blue {
    background-color: #4145ff;
}

button:hover,
.bg-color-red:hover {
    background-color: #FF414B;
    color: white;
}

.btn-transparent:hover {
    background-color: white;
    color: black;
}
</style>
