<template>
  <section>
    <img src="@/assets/images/cover-photo.jpg" alt="In Front of Catherine Cummings Theater" class="img-fluid">
  </section>
  <section class="mx-4">
    <h1>UPCOMING EVENTS</h1>
      <p><span class="text-blue">A Cabaret for the Environment</span> on <b>July 23, 2021 at 6pm</b> at the Fayetteville Free Library in the music pavilion. Bring a lawn chair and join us for an evening of music and environmental change. Learn about the Town of Manlius community campaign, <a href="https://www.facebook.com/sustainable.manlius/">Get Sustainable, Manlius!</a>, and hear from non-profits like HeatSmart CNY. We will be having local organizations table so you can learn all about sustainability in the area while also attending a great performance!. Click <a href="https://www.eventbrite.com/e/a-cabaret-for-the-environment-tickets-162821903697?fbclid=IwAR0BOxZNiPV4R1Ys5amazzMx0Bwfm2SNUTd_EEviwTgvh8T_Rwc1JtaogJw">here</a> to register for this free event.</p>
      <p><span class="text-blue">At Rise</span> will be participating in <a href="http://www.frontrowplayers.org">Front Row Players’</a> original production, <span class="text-blue">Let’s Go to the Movies</span>, on <b>July 29, 2021 at 7pm</b> at Fayetteville-Manlius High School. Click <a href="http://www.frontrowplayers.org/upcoming/">here</a> to register for your free ticket today!</p>
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