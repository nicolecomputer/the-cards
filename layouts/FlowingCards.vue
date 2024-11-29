<template>
    <div id="overlay">
        <div class="row">
            <Card size="small" />
            <Card size="medium" />
            <Card size="large" />
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
    flex-direction: column;
    color: white;
}

.row {
    display: flex;
    flex-direction: row;
    gap: 10px;
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
