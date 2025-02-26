<script setup>
import ClientCards from "./ClientCards.vue";
</script>

<template>
  <article class="wrapper">
    <section class="client">
      <h3>Clients</h3>
      <section class="client__content">
        <!-- Insert Vue Component ClientCards here-->
        <ClientCards
          review="This is a great portfolio! I recommend it to all my
        colleagues."
          name="Gina G."
        />
        <ClientCards
          review="This is a fine speciman of craftmanship. I thoroughly enjoyed and appreciate it."
          name="Alison M."
        />
        <ClientCards
          review="I really like the compositions and stylistics of
        the projects. Definitely something special."
          name="Birte C."
        />
      </section>
    </section>
  </article>
</template>

<style scoped>
.client {
  min-width: 315px;
}
.client__content {
  display: grid;
  min-width: 315px;
  min-height: auto;
  gap: 2em;
}
h3 {
  font-size: var(--h3-size);
  text-align: center;
}

/** Tablet breakpoint */
@media (min-width: 700px) {
  .client__content {
    display: inline-flex !important;
    justify-content: space-evenly;
    width: 100%;
  }
}

/** Desktop breakpoint */
@media (min-width: 900px) {
  .client__content {
    display: inline-flex !important;
    justify-content: space-evenly;
  }
}
</style>
