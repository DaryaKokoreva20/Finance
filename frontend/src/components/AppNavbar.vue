<template>
  <nav class="navbar">
    <div class="navbar-container">
      <!-- Логотип или название сайта -->
      <div class="navbar-left">
        <router-link to="/" class="navbar-logo">Finance Tracker</router-link>
      </div>

      <!-- Навигационные ссылки -->
      <div class="navbar-right">
        <ul class="navbar-links">
          <li>
            <router-link to="/" class="navbar-link">Главная</router-link>
          </li>
          <li>
            <router-link to="/expenses" class="navbar-link">Расходы</router-link>
          </li>
          <li>
            <router-link to="/income" class="navbar-link">Доходы</router-link>
          </li>
          <li>
            <router-link to="/settings" class="navbar-link">Настройки</router-link>
          </li>
          <li>
            <router-link to="/login" class="navbar-link">Вход/регистрация</router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'AppNavbar',
};
</script>

<style scoped>
.navbar {
  background-color: #2d3436;
  padding: 15px 20px;
  color: white;
  position: fixed;
  width: 100%;
  top: 0;
  left: 0;
  z-index: 1000;
}

.navbar-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
}

.navbar-left {
  font-size: 1.5rem;
  flex: auto;
}

.navbar-logo {
  color: #ffffff;
  text-decoration: none;
  font-weight: bold;
}

.navbar-right {
  display: flex;
  gap: 20px; 
  flex: 1; 
  justify-content: flex-end; 
}

.navbar-links {
  list-style: none;
  display: flex;
  gap: 20px;
}

.navbar-link {
  text-decoration: none;
  color: white;
  font-size: 1rem;
  font-weight: 500;
  transition: color 0.3s ease;
}

.navbar-link:hover {
  color: #00cec9;
}

/* Адаптивность: меню для мобильных устройств */
@media (max-width: 768px) {
  .navbar-container {
    flex-direction: column;
    align-items: flex-start;
  }

  .navbar-links {
    flex-direction: column;
    gap: 10px;
  }
}
</style>
