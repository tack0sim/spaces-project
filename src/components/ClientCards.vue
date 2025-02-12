<script setup>
import { defineProps } from "vue";

defineProps({
  review: String,
  name: String,
});
</script>

<template>
  <div class="upper">
    <div class="inner">
      <p>{{ review }}</p>
      <div class="rating">
        <img
          src="/src/assets/authorImages1.png"
          width="50"
          height="50"
          alt="author-image"
        />
        <div class="stars">
          <img src="/src/assets/rateStars.png" alt="stars-rating" />
          <p>{{ name }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
@media (min-width: 700px) {
  .upper {
    width: 19.5rem;
    height: auto;
  }
  .stars {
    grid-column-end: auto;
  }
}
@media (min-width: 900px) {
  .upper {
    width: 18rem;
    height: auto;
  }
}
.upper {
  padding: 30px;
  background-color: #ffffd285;
  border: solid #ffd285;
}
.inner {
  display: grid;
  align-content: center;
  justify-items: start;
  gap: 20%;
}
.rating {
  display: flex;
  justify-content: end;
  align-items: center;
}
.stars {
  display: grid;
  margin-left: 5%;
}
p {
  font-size: var(--text-size);
}
</style>
