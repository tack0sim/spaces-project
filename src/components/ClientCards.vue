<script setup>
import { defineProps } from "vue";

defineProps({
  review: String,
  name: String,
});
</script>

<template>
  <article class="review">
    <div class="review__inner">
      <!-- Review -->
      <p>{{ review }}</p>

      <!-- Author Image -->
      <section class="review__author">
        <img
          src="/src/assets/authorImages1.png"
          width="50"
          height="50"
          alt="author-image"
        />

        <!-- Star rating -->
        <section class="review__stars">
          <img src="/src/assets/rateStars.png" alt="stars-rating" />
          <p>{{ name }}</p>
        </section>
      </section>
    </div>
  </article>
</template>

<style scoped>
.review {
  padding: 30px;
  background-color: #ffffd285;
  border: solid #ffd285;
}
.review__inner {
  display: grid;
  align-content: center;
  justify-items: start;
  gap: 20%;
}
.review__author {
  display: flex;
  justify-content: end;
  align-items: center;
}
.review__stars {
  display: grid;
  margin-left: 5%;
}
p {
  font-size: var(--text-size);
}

/** Tablet breakpoint */
@media (min-width: 700px) {
  .review {
    width: 19.5rem;
    height: auto;
  }
  .review__stars {
    grid-column-end: auto;
  }
}

/** Desktop breakpoint */
@media (min-width: 900px) {
  .review {
    width: 18rem;
    height: auto;
  }
}
</style>
