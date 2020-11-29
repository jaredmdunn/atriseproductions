<template>
  <section class="pb-2 mx-4">
    <div class="row">
      <div class="col">
        <h1 class="text-blue text-center">{{ event.title }}</h1>
        <p v-if="event.by" class="text-center fst-italic">by {{ event.by }}</p>
      </div>
    </div>
    <div class="row m-auto justify-content-center">
      <div class="col-md col-lg-5 text-center">
        <img :src="require(`@/assets/images/event-photos/${event.slug}.jpg`)" :alt="event.title" class="img-fluid">
        <p v-if="event.eventPhotoCredit" class="fst-italic">Photo by {{ event.eventPhotoCredit }}</p>
      </div>
      <div class="col-md col-lg-5 text-center">
        <blockquote v-if="event.quote" class="bg-yellow border border-red rounded p-2 lh-1">
          <p v-html="event.quote"></p> -- <cite>{{ event.quoteBy }}</cite>
        </blockquote>
        <article class="lh-2" v-html="event.description"></article>
        <p v-if="event.program"><a :href="`/programs/${event.slug}.pdf`">Click here</a> to see the program.</p>
        <p v-if="event.video"><a :href="event.video">Click here</a> to watch <em>{{ event.title }}</em>.</p>
      </div>
    </div>
  </section>
</template>

<script>

export default {
  name: 'EventTitleCard',
  props: {
    event: Object
  },
}
</script>

<style>

</style>