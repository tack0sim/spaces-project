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
.upper {
  padding: 30px;
  background-color: #ffffd285;
}
.inner {
  display: grid;
  gap: 20%;
  min-height: fit-content;
}
.rating {
  display: flex;
  justify-content: flex-start;
}
.stars {
  display: grid;
  grid-auto-rows: auto;
  margin-left: 5%;
}
p {
  font-size: var(--text-size);
}
img {
  vertical-align: middle;
}
</style>
