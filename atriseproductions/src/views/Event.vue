<template>
  <EventTitleCard :event="event" />
</template>

<script>
import EventTitleCard from '../components/EventTitleCard.vue';
import events from '../assets/js/events';

export default {
  components: { 
    EventTitleCard 
  },
  computed: {
    event() {
      return events.find((event) => event.slug === this.$route.params.slug);
    }
  }
}
</script>

<style>

</style>