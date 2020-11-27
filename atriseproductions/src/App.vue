<template>
  <TheNav />
  <router-view/>
  <footer>
    <a href="https://www.facebook.com/CNYAtRise/" class="transparent"><i class="fab fa-facebook-f"></i></a>
    <a href="https://www.instagram.com/cnyatrise/" class="transparent"><i class="fab fa-instagram"></i></a>
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