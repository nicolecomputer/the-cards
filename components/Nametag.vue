<template>
    <div class="nametag">
        <img src="/name-tag.svg" />
        <div class="text">
            <h2>Nicole Watts</h2>
            <h3>W1 '24</h3>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped>
.nametag {
    position: absolute;
    bottom: 40px;
    left: 40px;
    transform: rotate(2deg);
}

img {
    position: relative;
}

.text {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

h2 {
    font-size: 24px;
    line-height: 1.0em;
    color: rgb(88, 25, 85);
}

h3 {
    font-size: 14px;
    color: rgb(88, 25, 85);
}
</style>
