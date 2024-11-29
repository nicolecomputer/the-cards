<template>
    <div class="face-down">
        <Card size="medium" />
        <Card size="medium" />
        <Card size="medium" />
        <Card size="medium" />
        <Card size="medium" />
    </div>
</template>

<script setup>
</script>

<style scoped>
@keyframes enter {

    0% {
        transform: scale(80%);
    }

    100% {
        transform: scale(90%);
    }
}


.card {
    animation: enter 1.2s ease-in-out;
    transform-origin: center center;
    animation-fill-mode: forwards;
}

.face-down {
    display: flex;
    flex-direction: row;
    z-index: 100;
}
</style>
