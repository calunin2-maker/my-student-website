
<template>
  <div class="website">
    <AppHeader />

    <main class="main-content">
      <NuxtPage />
    </main>

    <AppFooter />
  </div>
</template>

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #f1f5f9;
}

.website {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

.main-content {
  flex: 1;
}
</style>
