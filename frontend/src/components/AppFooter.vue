<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="footer-left">
        <p>&copy; 2026 Finance Tracker. All Rights Reserved.</p>
      </div>
      <div class="footer-center">
        <ul class="social-links">
          <h4>Be happy and rich</h4>
        </ul>
      </div>
      <div class="footer-right">
        <p>Made with ❤️</p>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background-color: #2d3436;
  color: #dfe6e9;
  padding: 20px 0;
  text-align: center;
  font-size: 14px;
  margin-top: 50px;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  max-width: 1200px;
  margin: 0 auto;
}

.footer-left, .footer-right {
  flex: 1;
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
</style>
