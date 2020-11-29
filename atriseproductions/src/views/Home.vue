<template>
  <main class="container-fluid p-0">
    <section>
      <img src="@/assets/images/cover-photo.jpg" alt="In Front of Catherine Cummings Theater" class="img-fluid">
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
  </main>
</template>

<script>

export default {
  name: 'Home',
  components: {
    
  }
}
</script>