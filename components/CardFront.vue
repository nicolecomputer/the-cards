<template>
    <div class="card" :style="cardStyle" :class="[`card--${kind}`]">
        <img :src="imageUrl" />
        <h2>{{ title }}</h2>
    </div>
</template>

<script setup>
import { computed } from 'vue';

const props = defineProps({
    imageUrl: {
        type: String,
        required: true,
    },
    title: {
        type: String,
        required: true,
    },
    rotationAngle: {
        type: String,
        default: "-8",
    },
    animated: {
        type: Boolean,
        default: true,
    },
    kind: {
        type: String,
        default: 'light',
        validator: (value) => ['light', 'dark', 'obstacle'].includes(value)
    }
});

const cardStyle = computed(() => ({
    '--final-rotation': `${props.rotationAngle}deg`,
    animation: props.animated ? 'enter 1.2s ease-in-out forwards' : 'none',
    'box-shadow': props.animated ? '' : '0px 0px 40px rgba(255, 0, 0, 0.3)'
}));
</script>

<style>
@keyframes enter {
    0% {
        transform: rotate(0deg) translate(0, 300px);
    }

    50% {
        transform: rotate(var(--final-rotation, -8deg)) translate(0, 0);
        box-shadow: 0px 0px 40px rgba(255, 254, 253, 0.5);
    }

    100% {
        transform: rotate(var(--final-rotation, -8deg)) translate(0px, 0);
        box-shadow: 0px 0px 40px rgba(255, 254, 253, 0.5);
    }
}
</style>

<style scoped>
img {
    padding: 5px;
}

.card--light {
    background: #e4b0b0ff;
}

.card--dark {
    background: #585867ff;
}

.card--obstacle {
    background: red;
}



.card {
    border-radius: 16px;
    height: 350px;
    width: 220px;

    animation-fill-mode: forwards;
    transform-origin: center center;
}

h2 {
    border-radius: 5px;
    background-color: rgb(234, 234, 234);
    margin: 0 10px;
    padding: 5px 0;
    color: rgb(91, 75, 91);
    text-align: center;
    font-weight: bold;
    font-size: 18px;
    position: relative;
    top: -6px;
    border: 1px solid rgb(53, 50, 53);
}
</style>
