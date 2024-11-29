<template>
    <div id="overlay">
        <img src="/curtain-top.svg" class="curtain-top" />
        <div class="curtain-left">
            <img src="/curtain.svg" />
        </div>
            <slot></slot>
        <div class="curtain-right">
            <img src="/curtain.svg" />
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped>
#overlay {
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
     display: flex;
     justify-content: center;
     align-items: center;
     color: white;
     padding-top: 80px;

     background: rgb(226,159,46);
     background: radial-gradient(circle, rgba(226,159,46,1) 0%, rgba(21,0,28,1) 45%, rgba(0,0,0,1) 96%);
    }

.curtain-top {
    position: absolute;
    top: 0;
    z-index: 1;
    filter: brightness(85%);
    padding: 5px 20px;
    height: min-content;
}

img {
    background-color: transparent;
    z-index: 1000;
}

.curtain-left {
    background-color: transparent;
    position: absolute;
    top: 0;
    left: 0;
    z-index: 2;
}

.curtain-right {
    background-color: transparent;
    position: absolute;
    top: 0;
    right: 0;
    z-index: 2;
    transform: scale(-1, 1);
}
</style>
