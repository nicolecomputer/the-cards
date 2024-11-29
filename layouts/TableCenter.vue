<template>
    <div id="overlay">
        <slot></slot>
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
    flex-direction: column;
    color: white;
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
