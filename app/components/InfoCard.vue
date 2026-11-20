
<template>
  <div class="info-card">
    <h2>{{ title }}</h2>
    <p>{{ description }}</p>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  description: String
})
</script>

<style scoped>
.info-card {
  background: white;
  padding: 25px;
  border-radius: 12px;
  border-left: 5px solid #2563eb;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
}

h2 {
  color: #172554;
  margin-top: 0;
}

p {
  color: #475569;
  line-height: 1.6;
}
</style>
