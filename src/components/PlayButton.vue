<script>
export default {
    name: 'PlayButton'
}
</script>

<template>
    <a href="#" class="play-button">
        <i class="fas fa-play"></i>
    </a>
</template>

<style lang="scss" scoped>
.play-button {
    display: inline-block;
    line-height: 80px;
    text-align: center;
    height: 80px;
    width: 80px;
    color: blue;
    background-color: white;
    border-radius: 50%;
    font-size: 23px;
}

.play-button:hover {
    color: #FF414B;
}
</style>