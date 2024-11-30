<template>
    <div class="card" :class="[
        `card--large`,
        {
            animated: !isFlipped,
            flip: isFlipped
        }
    ]">
        <div class="card-inner">
            <div class="front" :style="cardStyle">
                <div class="front-content">
                    <img src="/card.svg" />
                </div>
            </div>
            <div class="back" :style="cardStyle">
                <img src="/the-hero.png" />
            </div>
        </div>
    </div>
</template>

<script setup>
import { computed } from 'vue'

const isFlipped = computed(() => $slidev.nav.clicks >= 1)
</script>

<style scoped>
@keyframes shake {

    0%,
    100% {
        transform: rotate(0deg) translate(0, 0);
    }

    15% {
        transform: rotate(2deg) translate(-2px, -2px);
    }

    30% {
        transform: rotate(-1.5deg) translate(2px, 1px);
    }

    45% {
        transform: rotate(1deg) translate(-1px, -1px);
    }

    60% {
        transform: rotate(-3deg) translate(2px, 2px);
    }

    75% {
        transform: rotate(1.5deg) translate(-2px, 1px);
    }

    90% {
        transform: rotate(-1deg) translate(1px, -1px);
    }
}

.front-content {
    width: 100%;
    height: 100%;
    transform-style: preserve-3d;
}

img {
    border-radius: 10px;
    background-color: rgb(9, 7, 26);
    width: 100%;
    height: 100%;
    transform: translateZ(1px);
}

.card {
    perspective: 1000px;
    background: transparent;
    border-radius: 16px;
    height: 200px;
    aspect-ratio: 220/350;
    height: 350px;
}

.card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    transition: transform 0.6s;
    transform-style: preserve-3d;
}

.front,
.back {
    position: absolute;
    width: 100%;
    height: 100%;
    backface-visibility: hidden;
    border-radius: 16px;
    background: #e4e4e4;
    transform-style: preserve-3d;
}

.back img {
    background-color: transparent;
}

.front {
    padding: 10px;
}

.back {
    transform: rotateY(180deg);
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 20px;
    color: black;
}

.flip .card-inner {
    transform: rotateY(180deg);
    box-shadow: none;
}

.animated {
    animation: shake 2.2s linear infinite;
    transform-origin: center center;
}
</style>
