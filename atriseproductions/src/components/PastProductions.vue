<template>
  <section class="mx-4">
    <h2 class="text-center text-blue">Check out some of our past productions!</h2>
    <transition-group name="events" tag="div" class="row flex-column flex-sm-row">
      <div class="col" v-for="event in shownEvents" :key="event.id">
        <PastProductionCard :event="event"/>
      </div>
    </transition-group>
  </section>
</template>

<script>
import eventsArray from "../assets/js/events";
import PastProductionCard from "./PastProductionCard.vue";

export default {
  components: { PastProductionCard },
  name: "PastProductions",
  data() {
    return {
      events: Array.from(eventsArray),
    };
  },
  computed: {
    shownEvents() {
      return this.events.slice(0, 3);
    },
  },
  methods: {
    changeProductions() {
      const firstEvent = this.events.shift();
      this.events.push(firstEvent);
    },
  },
  mounted() {
    setInterval(this.changeProductions, 10000);
  },
};
</script>

<style scoped>
.events-move {
  transition: transform 0.8s ease;
}

.events-leave-active {
  position: absolute;
}
</style>