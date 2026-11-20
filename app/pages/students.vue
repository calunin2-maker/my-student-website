
<template>
  <div class="students-page">
    <section class="page-header">
      <h1>Our Students</h1>
      <p>Meet the students of our academic community.</p>
    </section>

    <section class="students-container">
      <StudentCard
        name="Niño Calubag"
        course="BS Information Technology"
        year="3rd Year"
        email="nino@example.com"
      />

      <StudentCard
        name="Juan Dela Cruz"
        course="BS Computer Science"
        year="2nd Year"
        email="juan@example.com"
      />

      <StudentCard
        name="Maria Santos"
        course="BS Information Technology"
        year="1st Year"
        email="maria@example.com"
      />
    </section>
  </div>
</template>

<style scoped>
.page-header {
  background: #1e3a8a;
  color: white;
  text-align: center;
  padding: 55px 20px;
}

.page-header h1 {
  font-size: 36px;
  margin-bottom: 10px;
}

.page-header p {
  margin: 0;
  line-height: 1.6;
}

.students-container {
  max-width: 1100px;
  margin: 50px auto;
  padding: 0 20px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 25px;
}

@media (max-width: 750px) {
  .students-container {
    grid-template-columns: 1fr;
  }
}
</style>
