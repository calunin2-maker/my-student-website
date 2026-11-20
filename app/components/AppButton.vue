
<template>
  <button class="app-button" :style="{ backgroundColor: color }">
    {{ label }}
  </button>
</template>

<script setup>
defineProps({
  label: {
    type: String,
    default: 'Click Me'
  },
  color: {
    type: String,
    default: '#2563eb'
  }
})
</script>

<style scoped>
.app-button {
  color: white;
  border: none;
  padding: 11px 22px;
  border-radius: 7px;
  font-size: 14px;
  font-weight: bold;
  cursor: pointer;
  transition: 0.3s;
}

.app-button:hover {
  opacity: 0.8;
  transform: translateY(-2px);
}
</style>
