<script setup>
import { defineProps } from "vue";

defineProps({
  message: String,
});
</script>

<template>
  <div>
    <p class="logo">Logo</p>
    <p id="home-message">{{ message }}</p>
    <ul>
      <li>
        <a href="" class="menuItem">About</a>
      </li>
      <li>
        <a href="" class="menuItem">Work</a>
      </li>
      <li>
        <a href="" class="menuItem">Contact</a>
      </li>
    </ul>
  </div>
</template>

<style scoped>
.logo,
#home-message {
  font-size: var(--h4-size);
  font-weight: 600;
}
a.menuItem {
  font-size: var(--h5-size);
  font-weight: 400;
}
</style>
