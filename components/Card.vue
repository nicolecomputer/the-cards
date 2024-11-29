<template>
  <div class="card" :class="{ animated: animated }">
    <img src="/card.svg" />
  </div>
</template>

<script setup>
defineProps({
  animated: {
    type: Boolean,
    default: false
  }
})
</script>

<style scoped>
img {
  border-radius: 10px;
  background-color: rgb(11, 9, 23);
  width: 100%;
  height: 100%;
}

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

.card {
  background: #e4e4e4;
  border-radius: 16px;
  box-shadow: 10px 10px 20px rgba(255, 254, 253, 0.3);
  height: 350px;
  width: 220px;
  padding: 10px;
  transition: all ease-in 0.3s;
}

.animated {
  animation: shake 2.2s linear infinite;
  transform-origin: center center;
}
</style>
