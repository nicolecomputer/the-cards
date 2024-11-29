<template>
    <div class="card">
        <img src="/the-computer.svg" />
        <h2>The Computer</h2>
    </div>
</template>

<script setup>
</script>

<style scoped>
img {
    padding: 5px;
}

@keyframes bob {

    0%,
    100% {
        transform: translate(0, 0) rotate(1deg);
    }

    50% {
        transform: translate(0, 12px) rotate(-1deg);
    }
}


.card {
    background: #e8e3d3ff;
    border-radius: 16px;
    box-shadow: 0px 0px 40px rgba(0, 174, 189, 0.668);
    height: 350px;
    width: 220px;

    animation: bob 5s ease-in-out infinite;
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
