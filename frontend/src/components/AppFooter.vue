<template>
  <footer class="footer">
    <div class="footer-container">
      <div class="footer-left">
        <p>&copy; 2026 Finance Tracker. All Rights Reserved.</p>
      </div>
      <div class="footer-center">
        <ul class="social-links">
          <p>BE HAPPY AND RICH</p>
        </ul>
      </div>
      <div class="footer-right">
        <p>Made with ❤️</p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'AppFooter',
};
</script>

<style scoped>
.footer {
  background-color: #2d3436;
  color: #dfe6e9;
  padding: 20px 0;
  text-align: center;
  font-size: 14px;
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  z-index: 1000;
}

.footer-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.footer-left, .footer-right {
  flex: 1;
  font-size: 1rem;
}

.footer-center {
  flex: 2;
}

.social-links {
  list-style: none;
  padding: 0;
  display: flex;
  justify-content: center;
  gap: 15px;
}

.social-links li a {
  color: #dfe6e9;
  text-decoration: none;
  font-weight: bold;
  transition: color 0.3s;
}

.social-links li a:hover {
  color: #00cec9;
}

.footer-right a {
  color: #dfe6e9;
  text-decoration: none;
}

.footer-right a:hover {
  text-decoration: underline;
}

/* Адаптивность: футер для мобильных устройств (расположение в строку) */
@media (max-width: 768px) {
  .footer-container {
    flex-direction: row;
    align-items: center;
    text-align: left;
  }

  .footer-left, .footer-center, .footer-right {
    flex: 1;
    text-align: center;
  }

  .footer-center {
    margin-top: 0;
  }
}
</style>
