
<template>
  <div class="student-card">
    <div class="avatar">
      {{ name.charAt(0) }}
    </div>

    <h2>{{ name }}</h2>
    <p class="course">{{ course }}</p>

    <div class="details">
      <p><strong>Year Level:</strong> {{ year }}</p>
      <p><strong>Email:</strong> {{ email }}</p>
    </div>

    <AppButton label="View Profile" color="#2563eb" />
  </div>
</template>

<script setup>
defineProps({
  name: String,
  course: String,
  year: String,
  email: String
})
</script>

<style scoped>
.student-card {
  background: white;
  padding: 25px;
  border-radius: 12px;
  text-align: center;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
  border: 1px solid #e2e8f0;
}

.avatar {
  width: 65px;
  height: 65px;
  background: #dbeafe;
  color: #1e40af;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 26px;
  font-weight: bold;
  margin: auto;
}

h2 {
  color: #172554;
  margin-bottom: 5px;
}

.course {
  color: #2563eb;
  font-weight: bold;
}

.details {
  color: #475569;
  text-align: left;
  margin-top: 20px;
  font-size: 14px;
  overflow-wrap: anywhere;
}
</style>
