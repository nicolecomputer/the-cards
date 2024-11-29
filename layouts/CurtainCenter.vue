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
     background-color: rgb(21, 0, 28);
     display: flex;
     justify-content: center;
     align-items: center;
     color: white;
}

.curtain-top {
    position: absolute !important;
    top: -205px;
    z-index: 1;
    width: 95%;
    filter: brightness(85%);
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
#overlay::after {
    content: '';
    position: absolute;
    top: 4;
    right: 4;
    left: 4;
    bottom: 40;

    border: 2px solid #DE9B72;
   	height: 95%;
    width: 98%;
    padding: 6px;
    margin: 0 auto;

}
</style>
