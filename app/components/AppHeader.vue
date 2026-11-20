
<template>
  <header class="header">
    <div class="container">
      <NuxtLink to="/" class="logo">
        StudentHub
      </NuxtLink>

      <nav>
        <NuxtLink to="/">Home</NuxtLink>
        <NuxtLink to="/students">Students</NuxtLink>
        <NuxtLink to="/about">About</NuxtLink>
      </nav>
    </div>
  </header>
</template>

<style scoped>
.header {
  background: #172554;
  padding: 20px 0;
  color: white;
}

.container {
  max-width: 1100px;
  margin: auto;
  padding: 0 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 24px;
  font-weight: bold;
  color: white;
  text-decoration: none;
}

nav {
  display: flex;
  gap: 25px;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: 500;
}

nav a:hover {
  color: #93c5fd;
}
</style>
