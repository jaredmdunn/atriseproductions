<template>
  <nav class="navbar navbar-expand-sm navbar-light bg-orange sticky-top p-0">
    <div class="container-fluid">
      <button class="navbar-toggler m-auto border-0" type="button" data-toggle="collapse" data-target="#main-nav" aria-controls="main-nav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse container-fluid" id="main-nav">
        <ul class="navbar-nav d-flex justify-content-evenly col text-center">
          <li class="nav-item">
            <router-link class="nav-link" to="/">Home</router-link>
          </li>
          <li class="nav-item">
            <a v-if="ticketsActive" class="nav-link" href="https://mkt.com/atrise">Tickets</a>
            <a v-else class="nav-link" data-toggle="tooltip" title="Tickets are currently unavailable.">Tickets</a></li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" id="events-dropdown" role="button" data-toggle="dropdown" aria-expanded="false">Events</a>
            <ul class="dropdown-menu text-center text-sm-left bg-light-orange mt-0 border-0" aria-labelledby="events-dropdown">
              <li v-for="event in events" :key="event.id"><router-link class="dropdown-item" :to="'/events/' + event.slug">{{ event.title }}</router-link></li>
            </ul>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/get-involved">Get Involved</router-link>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://mkt.com/atrise2">Support</a>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">About</router-link> 
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
import eventsArray from '../assets/js/events';

export default {
  name: 'TheNav',
  props: {
    ticketsActive: Boolean
  },
  data() {
    return {
      events: eventsArray.reverse(),
    }
  }
}
</script>

<style scoped>
  /* nav li.nav-item a.nav-link {
    color: blue;
    font-weight: bold;
  }
  nav li.nav-item a.router-link-active {
    color: red;
    font-weight: bold;
  } */

</style>