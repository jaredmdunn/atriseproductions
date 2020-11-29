<template>
  <section>
    <img src="@/assets/images/cover-photo.jpg" alt="In Front of Catherine Cummings Theater" class="img-fluid">
  </section>
  <section class="mx-4">
    <h1>COVID-19</h1>
    <p>Due to the coronavirus pandemic, our Spring 2020 production of <em>Calvin Burger</em> has been canceled. We hope that everyone is staying safe and healthy through this insane period of history. We will be back producing theater when it is safe to do so. Best wishes from everyone at <span class="text-blue">At Rise</span>.</p>
  </section>
  <aside class="bg-orange text-center row mx-4 justify-content-center">
    <div class="col col-md-9 col-lg-6">
      <h2 class="text-blue">At Rise Productions</h2>
      <p>is a Central New York based theater company dedicated to providing 
        unique opportunities for young people to participate in all parts 
        of putting on a theatrical production.</p>
      <p><router-link to="/about">Read our story!</router-link></p>
    </div>
  </aside>
  <PastProductions />
</template>

<script>
import PastProductions from '../components/PastProductions.vue'

export default {
  name: 'Home',
  components: {
    PastProductions
  }
}
</script>