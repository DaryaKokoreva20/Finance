<script>
  import Navbar from './components/AppNavbar.vue'
  import Footer from './components/AppFooter.vue';

  export default {
    components: {
      Navbar,
      Footer
    }
  };
</script>

<template>
  <div id="app">
    <Navbar />
    <Footer />
  </div>
</template>
