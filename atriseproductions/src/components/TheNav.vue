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
            <a class="nav-link" href="https://mkt.com/atrise">Tickets</a>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/events">Events</router-link> 
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
export default {

}
</script>

<style>

</style>