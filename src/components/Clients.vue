<script setup>
import ClientCards from "./ClientCards.vue";
</script>

<template>
  <div class="outer">
    <div class="inner">
      <h3>Clients</h3>
      <div class="content">
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
      </div>
    </div>
  </div>
</template>

<style scoped>
.outer {
  padding: 60px 30px 90px 30px;
}
.inner {
  min-width: 315px;
}
.content {
  display: grid;
  min-width: 315px;
  min-height: auto;
  gap: 10%;
  overflow: scroll;
}
h3 {
  font-size: var(--h3-size);
  text-align: center;
}
</style>
