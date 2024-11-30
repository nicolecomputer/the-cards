<template>
  <div class="card" :class="[`card--${size}`]" :style="cardStyle">
    <img src="/card.svg" />
  </div>
</template>

<script setup>
import { computed } from 'vue'

const props = defineProps({
  size: {
    type: String,
    default: 'large',
    validator: (value) => ['small', 'medium', 'large'].includes(value)
  },
  shadowColor: {
    type: String,
    default: 'rgba(255, 254, 253, 0.3)'
  }
})

const cardStyle = computed(() => ({
  boxShadow: `10px 10px 20px ${props.shadowColor}`
}))
</script>

<style scoped>
img {
  border-radius: 10px;
  background-color: rgb(9, 7, 26);
  width: 100%;
  height: 100%;
}

.card {
  background: #e4e4e4;
  border-radius: 16px;
  height: 200px;
  aspect-ratio: 220/350;
  padding: 10px;
  transition: all ease-in 0.3s;
}

.card--small {
  height: 150px;
  padding: 7px;
}

.card--medium {
  height: 250px;
  padding: 8px;
}

.card--large {
  height: 350px;
  padding: 10px;
}
</style>
