<template>
    <div class="card">
        <img src="/nature.svg" />
        <h2>Nature</h2>
    </div>
</template>

<script setup>
</script>

<style scoped>
img {
    padding: 5px;
}

@keyframes enter {

    0% {

        transform: rotate(0deg) translate(0, 300px);
    }

    50% {
        transform: rotate(-8deg) translate(0, 0);
        box-shadow: 0px 0px 40px rgba(255, 254, 253, 0.5);
    }

    100% {
        transform: rotate(-8.0deg) translate(0px, 0);
        box-shadow: 0px 0px 40px rgba(255, 254, 253, 0.5);
    }
}


.card {
    background: #e4b0b0ff;
    border-radius: 16px;
    height: 350px;
    width: 220px;

    animation: enter 1.2s ease-in-out;
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
