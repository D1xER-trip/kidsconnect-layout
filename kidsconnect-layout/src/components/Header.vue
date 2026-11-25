<template>
  <header class="header">
    <div class="container header-inner">
      <router-link to="/" class="logo">
        <div class="logo-img">🐻</div>
        KidsConnect
      </router-link>
    </div>
  </header>
</template>

<style scoped>
.header {
  background-color: var(--primary);
  padding: 12px 0;
}
.header-inner {
  display: flex;
  align-items: center;
}
.logo {
  color: white;
  text-decoration: none;
  font-size: 20px;
  font-weight: 600;
  display: flex;
  align-items: center;
  gap: 12px;
}
.logo-img {
  width: 32px;
  height: 32px;
  background: #5c161e;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 16px;
}
</style>