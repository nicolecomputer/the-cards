<template>
    <div id="overlay">
        <div class="card-slot">
            <slot name="card" class="card-slot" />
        </div>
        <div class="text-slot">
            <slot />
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped>
.card-slot {
    margin: 0 160px;
}

.text-slot {
    flex: 1
}

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
