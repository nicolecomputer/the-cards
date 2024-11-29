<template>
  <div class="perspective">
    <div class="card-container spread" :class="{ 'spread': isSpread }" @click="toggleSpread">
      <div class="card card-1">
        <img src="/card.svg" />
      </div>
      <div class="card card-2">
        <img src="/card.svg" />
      </div>
      <div class="card card-3">
        <img src="/card.svg" />
      </div>
      <div class="card card-4">
        <img src="/card.svg" />
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const isSpread = ref(false)
const toggleSpread = () => {
  console.log('click', isSpread.value) // Add this to debug
  isSpread.value = !isSpread.value
}
</script>

<style scoped>
.perspective {
  height: 100vh;
  perspective: 2000px;
  position: absolute;
  width: 100vw;
}

.card-container {
  cursor: pointer;
  left: 50%;
  position: absolute;
  top: 50%;
  transform: rotateX(35deg) translate(-50%, -50%);
  height: 350px;
  width: 220px;
}

img {
  border-radius: 10px;
  background-color: rgb(9, 0, 77);
  width: 100%;
  height: 100%;
}

.card {
  background: #e4e4e4;
  border-radius: 16px;
  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.4);
  height: 350px;
  width: 220px;
  padding: 10px;
  position: absolute;
  transition: all ease-in 0.3s;
}

/* Initial stacked positions */
.card-1 {
  transform: rotate(-31deg) translate(-50%, -10%);
  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.4),
    0 4px 12px 0 rgba(0, 0, 0, 0.4);
}

.card-2 {
  transform: rotate(-31deg) translate(-49.5%, -10.5%);
}

.card-3 {
  transform: rotate(-31deg) translate(-49%, -11%);
}

.card-4 {
  transform: rotate(-31deg) translate(-48.5%, -11.5%);
}

/* Spread positions */
.card-container.spread .card-1 {
  transform: rotate(-31deg) translate(-50%, -10%);
}

.card-container.spread .card-2 {
  transform: rotate(-4.5deg) translateX(-22%);
}

.card-container.spread .card-3 {
  transform: rotate(5.8deg) translateX(10%);
}

.card-container.spread .card-4 {
  transform: rotate(22.5deg) translate(40%, -5%);
}
</style>
