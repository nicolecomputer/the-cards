<template>
    <div class="container">
        <div class="fade-edge fade-left"></div>
        <div class="fade-edge fade-right"></div>

        <div v-for="(row, index) in rows" :key="index" class="row" :class="`flow-${row.direction}`"
            :style="{ '--duration': `${row.duration}s` }">
            <div class="row-content">
                <template v-for="set in 3" :key="set">
                    <Card v-for="card in cardsPerSet" :key="`${set}-${card}`" size="small"
                        shadowColor="rgba(255, 0, 0, 0.3)" />
                </template>
            </div>
        </div>
    </div>
</template>

<script setup>
const cardsPerSet = 13;

const rows = [
    { direction: 'left', duration: 45 },
    { direction: 'right', duration: 180 },
    { direction: 'left', duration: 90 }
];
</script>

<style scoped>
.container {
    width: 100%;
    overflow: hidden;
    gap: 10px;
    display: flex;
    flex-direction: column;
    /* Improve performance by creating a new stacking context */
    isolation: isolate;
}

.row {
    position: relative;
    width: 100%;
    /* Force GPU acceleration */
    transform: translateZ(0);
    will-change: transform;
}

.row-content {
    display: flex;
    flex-direction: row;
    gap: 10px;
    width: max-content;
    --duration: 60s;
}

.flow-left .row-content {
    animation: slide-left var(--duration) linear infinite;
    /* Improve animation performance */
    backface-visibility: hidden;
    perspective: 1000px;
}

.flow-right .row-content {
    animation: slide-right var(--duration) linear infinite;
    /* Improve animation performance */
    backface-visibility: hidden;
    perspective: 1000px;
}

@keyframes slide-left {
    0% {
        transform: translateX(0);
    }

    100% {
        transform: translateX(calc(-100% / 3));
    }
}

@keyframes slide-right {
    0% {
        transform: translateX(calc(-100% / 3 * 2));
    }

    100% {
        transform: translateX(calc(-100% / 3));
    }
}

.fade-edge {
    position: absolute;
    top: 0;
    bottom: 0;
    width: 300px;
    z-index: 9;
    pointer-events: none;
}

.fade-left {
    left: 0;
    background: linear-gradient(to right,
            var(--background-color, rgb(0, 0, 0)) 0%,
            transparent 100%);
}

.fade-right {
    right: 0;
    background: linear-gradient(to left,
            var(--background-color, rgb(0, 0, 0)) 0%,
            transparent 100%);
}
</style>
