<template>
  <section>
    <img src="@/assets/images/cover-photo.jpg" alt="In Front of Catherine Cummings Theater" class="img-fluid">
  </section>
  <section class="mx-4">
    <h1 class=text-blue">UPCOMING EVENTS!</h1>
      <p><b>July 23, 2021 at 6pm</b> - <em>A Cabaret for the Environment</em>: <span class="text-blue">At Rise</span>, <a href="https://https://movementsthroughmu.wixsite.com/elenaandkira/director-s-note">Movements Through Music</a>, and <a href="https://www.facebook.com/sustainable.manlius/">Sustainable Manlius</a> are organizing an evening of live music and environmental change at the <a href="https://https://fflib.org/">Fayetteville Free Library</a> in the music pavilion. Bring a lawn chair and join us for a great night of performances, learn about the Town of Manlius community campaign, <em>Get Sustainable, Manlius!</em> and the local sustainability efforts being taken by local organizations, such as <a href="https://heatsmartcny.org/">HeatSmart CNY</a>. Click <a href="https://www.eventbrite.com/e/a-cabaret-for-the-environment-tickets-162821903697?fbclid=IwAR0BOxZNiPV4R1Ys5amazzMx0Bwfm2SNUTd_EEviwTgvh8T_Rwc1JtaogJw">here</a> to register for this free event.</p>
      <p><b>July 29, 2021 at 7pm</b> - <em>Let’s Go to the Movies</em>: <span class="text-blue">At Rise</span> will be participating in <a href="http://www.frontrowplayers.org">Front Row Players’</a> original production, <em>Let’s Go to the Movies</em> at <a href="https://www.fmschools.org/fayetteville-manlius-high-school/">Fayetteville-Manlius High School</a>. Click <a href="http://www.frontrowplayers.org/upcoming/">here</a> to register for your free ticket today!</p>
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