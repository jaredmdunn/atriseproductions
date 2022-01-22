<template>
  <section>
    <img src="@/assets/images/cover-photo.jpg" alt="In Front of Catherine Cummings Theater" class="img-fluid">
  </section>
  <section class="mx-4">
    <h1 class="text-blue">Get Involved!</h1>
    <p>Pre-COVID, <span class="text-blue">At Rise Productions</span> put
          on a full musical in the spring and a cabaret of original work in the summer. 
          We are still a young company and the coming years may look different, so make
          sure you keep an eye out for any news about auditions or shows. Please email us at 
          <a href="mailto:cnyatrise@gmail.com">cnyatrise@gmail.com</a> if you wish to be 
          added to our mailing list.</p>
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
import PastProductions from "../components/PastProductions.vue";

export default {
  name: "Home",
  components: {
    PastProductions,
  },
};
</script>