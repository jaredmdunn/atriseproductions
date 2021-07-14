<template>
  <div>
  <section class="mx-4 text-center">
    <h1 class="text-blue">Who We Are</h1>
    <div class="row">
      <div class="col-md">
        <img src="@/assets/images/who-we-are.jpg" alt="Who We Are" class="img-fluid">
        <p class="fst-italic">Photo by Genevieve Fridley</p>
      </div>
      <div class="col-md d-flex flex-column justify-content-center">
        <p><span class="text-blue">At Rise Productions</span> is a Central New York based theater company dedicated to providing unique opportunities for young people to participate in all parts of putting on a theatrical production.</p>
        <p><router-link :to="{name: 'About', hash: '#mission'}" class="text-red fs-5">Read our mission!</router-link></p>
      </div>
    </div>
  </section>
  <section class="mx-4 pb-4">
    <h2 class="text-blue text-center">Some History</h2>
    <div class="row flex-column flex-md-row mx-lg-5">
      <div class="col d-flex flex-column justify-content-center text-center">
        <router-link to="/events/charlie-brown">
          <img src="@/assets/images/event-photos/charlie-brown.jpg" class="img-thumbnail" alt="You're A Good Man, Charlie Brown">
        </router-link>
      </div>
      <div class="col d-flex flex-column justify-content-center">
        <p><span class="text-blue">At Rise Productions</span> was officially started in late 2017, 
        but our first show was not until spring of 2018 when we put on 
        <em>You're A Good Man, Charlie Brown</em> with the help of 
        <a href="https://www.facebook.com/theappleseedcommunity/">Appleseed Community</a>
        and <a href="http://alcsyracuse.org/">Atonement Ministries</a>. Our team of seventeen 
        young people ranging from 12 to 18 years old made up the cast, crew, pit, and creative team for the 
        production. We had four wonderful performances, and for this production our Founding Artistic Director, 
        Jared Dunn, received a SALT (Syracuse Area Live Theater) award nomination for Best Director of a 
        Musical in community theater.</p>
      </div>
    </div>
    <div class="row flex-column-reverse flex-md-row mx-lg-5">
      <div class="col d-flex flex-column justify-content-center">
        <p>Tragedy struck when Blake Lucas, who played Linus in <em>You're A Good Man, Charlie Brown</em> passed away suddenly and unexpectedly during the summer of 2018. Blake was much loved by the entire At Rise community for his sense of humor and kind spirit. He will be forever missed.</p>
      </div>
      <div class="col d-flex flex-column justify-content-center text-center">
        <img src="@/assets/images/blake.jpg" class="img-thumbnail" alt="Blake">
      </div>
    </div>
    <div class="row flex-column flex-md-row mx-lg-5">
      <div class="col d-flex flex-column justify-content-center text-center">
        <router-link to="/events/summer-cabaret-2018">
          <img src="@/assets/images/event-photos/summer-cabaret-2018.jpg" class="img-thumbnail" alt="Summer Cabaret 2018">
        </router-link>
      </div>
      <div class="col d-flex flex-column justify-content-center">
        <p>That same summer, Jared Dunn and Nancy O'Connor had been writing songs together for an 
        <span class="text-blue">At Rise Productions</span> summer cabaret performance of original work. 
        They had just started rehearsals 
        when Blake passed away. Blake was a close friend of Jared and Nancy, 
        and with the permission of Blake's family, we turned the cabaret into a memorial for him 
        and a fundraiser for his family. We performed the cabaret after the funeral service. 
        Eighteen students, including the entire cast of <em>You're A Good Man, Charlie Brown</em>, performed eleven 
        original songs for an audience of over 300 people.</p>
      </div>
    </div>
    <div class="row flex-column-reverse flex-md-row mx-lg-5">
      <div class="col d-flex flex-column justify-content-center">
        <p>In May 2019, we produced our second spring musical <em>Band Geeks</em>. 
        We had nearly triple the number of young people working on 
        <em>Band Geeks</em> as we had for the previous year's
        production. Our cast, pit, crew, and production team included young people and adults
        hailing from seven school districts, and we sold more than 600 tickets, more than double the 
        amount of tickets we sold for <em>You're A Good Man, Charlie Brown</em>. 
        <em>Band Geeks</em> received 
        <a href="https://familytimescny.com/2019/10/17/nominees-for-2019-salt-awards-revealed/">five SALT nominations</a> in the community 
        theater category including best musical!</p>
      </div>
      <div class="col d-flex flex-column justify-content-center text-center">
        <router-link to="/events/band-geeks">
          <img src="@/assets/images/event-photos/band-geeks.jpg" class="img-thumbnail" alt="Band Geeks">
        </router-link>
      </div>
    </div>
    <div class="row flex-column flex-md-row mx-lg-5">
      <div class="col d-flex flex-column justify-content-center text-center">
        <router-link to="/events/teenage-nobodies">
          <img src="@/assets/images/event-photos/teenage-nobodies.jpg" class="img-thumbnail" alt="Teenage Nobodies">
        </router-link>
      </div>
      <div class="col d-flex flex-column justify-content-center">
        <p><em>Teenage Nobodies</em>, a cabaret of original songs
        written by O'Connor & Dunn was performed at on August 18th at the Catherine
      Cummings Theatre. We raised funds to start the Blake Lucas Memorial 
      Music/Theater Scholarship Fund.</p>
      </div>
    </div>
  </section>
  <section class="mx-4 pb-4" id="mission">
    <h2 class="text-blue text-center">Mission</h2>
    <div class="row flex-column-reverse flex-md-row">
      <div class="col d-flex flex-column justify-content-center">
        <p><span class="text-blue">At Rise Productions</span> has made it its mission to:</p>
        <ol>
          <li>Produce high-quality theater in which the majority of the cast, pit, crew, and creative team are teenagers.</li>
          <li>Create a community where young artists from the Syracuse area can connect with each other and with local adult 
            artists, acting as a bridge between the Syracuse-area theater community and local young artists.</li>
          <li>Attract young people as audience members and artists with the goal of creating lifelong theater lovers 
            and theater creators.</li>
        </ol>
      </div>
      <div class="col text-center">
        <img src="@/assets/images/mission.jpg" class="img-fluid" alt="Mission">
      </div>
    </div>
  </section>
  </div>
</template>

<style scoped>
  img {
    transform: scale(1);
    transition: transform 0.8s;
  }

  a img:hover {
    transform: scale(0.9);
    transition: transform 0.8s;
  }
</style>