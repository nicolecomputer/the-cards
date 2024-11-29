<template>
    <div class="display-area">
        <slot />
    </div>
</template>

<script setup>
</script>

<style scoped>
@keyframes fadeInAnimation {
    0% {
        opacity: 0;
    }

    100% {
        opacity: 1;
    }
}

.display-area {
    display: flex;
    flex-direction: row;
    gap: 20px;
    animation: fadeInAnimation ease 1s;
    animation-iteration-count: 1;
    animation-fill-mode: forwards;
}
</style>
