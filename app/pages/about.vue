
<template>
  <div class="about-page">
    <section class="page-header">
      <h1>About StudentHub</h1>
      <p>Learn more about our student information website.</p>
    </section>

    <section class="about-content">
      <InfoCard
        title="Our Purpose"
        description="StudentHub is a simple student information website designed to organize and display student profiles in one accessible platform."
      />

      <InfoCard
        title="Our Technology"
        description="This website is developed using Nuxt and Vue.js. It demonstrates component-based development, reusable components, and props."
      />

      <InfoCard
        title="Our Goal"
        description="Our goal is to demonstrate how reusable components make website development more organized, efficient, and maintainable."
      />

      <div class="button-section">
        <NuxtLink to="/students" class="back-button">
          Explore Our Students
        </NuxtLink>
      </div>
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
}

.about-content {
  max-width: 850px;
  margin: 50px auto;
  padding: 0 20px;
  display: grid;
  gap: 25px;
}

.button-section {
  text-align: center;
  margin-top: 10px;
}

.back-button {
  display: inline-block;
  background: #2563eb;
  color: white;
  text-decoration: none;
  padding: 13px 25px;
  border-radius: 7px;
  font-weight: bold;
}

.back-button:hover {
  background: #1e40af;
}
</style>
