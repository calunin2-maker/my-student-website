
<template>
  <div class="home">
    <section class="hero">
      <h1>Welcome to StudentHub</h1>

      <p>
        Your simple and reliable student information portal.
        Explore student profiles and learn more about our community.
      </p>

      <NuxtLink to="/students" class="explore-button">
        Explore Students
      </NuxtLink>
    </section>

    <section class="content">
      <h2>What We Offer</h2>

      <div class="info-grid">
        <InfoCard
          title="Student Profiles"
          description="View student names, courses, year levels, and contact information."
        />

        <InfoCard
          title="Easy Navigation"
          description="Explore our website through a simple and user-friendly navigation system."
        />

        <InfoCard
          title="Reusable Components"
          description="Our website uses reusable Vue components to create consistent layouts."
        />
      </div>
    </section>
  </div>
</template>

<style scoped>
.hero {
  background: #1e3a8a;
  color: white;
  text-align: center;
  padding: 90px 20px;
}

.hero h1 {
  font-size: 42px;
  margin-bottom: 15px;
}

.hero p {
  max-width: 650px;
  margin: 0 auto 30px;
  line-height: 1.7;
}

.explore-button {
  display: inline-block;
  background: white;
  color: #1e3a8a;
  padding: 13px 25px;
  border-radius: 7px;
  text-decoration: none;
  font-weight: bold;
}

.explore-button:hover {
  background: #dbeafe;
}

.content {
  max-width: 1100px;
  margin: 50px auto;
  padding: 0 20px;
}

.content h2 {
  color: #172554;
  text-align: center;
  margin-bottom: 30px;
}

.info-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

@media (max-width: 700px) {
  .info-grid {
    grid-template-columns: 1fr;
  }

  .hero h1 {
    font-size: 30px;
  }
}
</style>
