<template>
  <header class="container-fluid d-none d-sm-flex bg-yellow p-0">
    <img src="@/assets/images/logo.png" alt="At Rise Logo" class="img-fluid">
    <div class="d-flex align-items-end">
      <h1 class="text-blue m-0 ml-2 fw-bold">At Rise Productions</h1>
    </div>
  </header>
  <TheNav />
  <main class="bg-white mx-3 p-2">
    <router-view/>
  </main>
  <footer class="fixed-bottom bg-yellow d-flex">
    <a href="https://www.facebook.com/CNYAtRise/"><i class="fab fa-facebook-f"></i></a>
    <a href="https://www.instagram.com/cnyatrise/"><i class="fab fa-instagram"></i></a>
    <p>&copy; 2020 At Rise Productions. All rights reserved.</p>
  </footer>
</template>

<script>
import TheNav from './components/TheNav.vue'
export default {
  components: { 
    TheNav 
  },
}
</script>

<style>
  @import './assets/css/custom.css'

</style>