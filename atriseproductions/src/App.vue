<template>
  <header class="container-fluid d-none d-sm-flex bg-yellow p-0">
    <img src="@/assets/images/logo.png" alt="At Rise Logo" class="img-fluid">
    <div class="d-flex align-items-end">
      <h1 class="text-blue m-0 ml-2 fw-bold">At Rise Productions</h1>
    </div>
    <aside class="col text-right p-2">
      <a href="mailto:cnyatrise@gmail.com" class="p-1">cnyatrise@gmail.com</a><br>
      <a href="https://www.facebook.com/CNYAtRise/"><i class="fab fa-facebook-square fs-5 p-1"></i></a>
      <a href="https://www.instagram.com/cnyatrise/"><i class="fab fa-instagram fs-5 p-1"></i></a>
    </aside>
  </header>
  <TheNav :ticketsActive="ticketsActive" />
  <main class="bg-white mx-3 pb-5 p-0">
    <router-view/>
  </main>
  <footer class="fixed-bottom bg-yellow d-flex p-2">
    <a href="https://www.facebook.com/CNYAtRise/"><i class="fab fa-facebook-square fs-5 p-1"></i></a>
    <a href="https://www.instagram.com/cnyatrise/"><i class="fab fa-instagram fs-5 p-1"></i></a>
    <p class="col text-right m-0">&copy; {{ year }} At Rise Productions. All rights reserved.</p>
  </footer>
</template>

<script>
import TheNav from './components/TheNav.vue'
export default {
  components: { 
    TheNav 
  },
  data() {
    return {
      ticketsActive: false,
    }
  },
  computed: {
    year() {
      const now = new Date();
      return now.getFullYear();
    }
  }
}
</script>

<style scoped>
  @import './assets/css/custom.css';

  h1 {
    font-size: 3rem;
  }

</style>