<template>
  <div class="text-center">
    <h4 class="fs-6">{{ event.title }}</h4>
    <router-link :to="`/events/${event.slug}`">
      <img :src="require(`@/assets/images/event-photos/${event.slug}.jpg`)" :alt="event.title" class="img-thumbnail">
    </router-link>
    <p class="fst-italic">{{ event.date }}</p>
  </div>
</template>

<script>
export default {
  name: 'PastProductionCard',
  props: {
    event: Object
  }
}
</script>

<style scoped>
  a img {
    transform: scale(1);
    transition: transform 0.8s;
  }

  a img:hover {
    transform: scale(0.9);
    transition: transform 0.8s;
  }
</style>