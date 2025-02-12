<script setup>
import { defineProps } from "vue";

defineProps({
  message: String,
});
</script>

<template>
  <div class="wrapper">
    <nav>
      <p class="logo">Logo</p>
      <p id="home-message">{{ message }}</p>
      <div class="menu">
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
    </nav>
  </div>
</template>

<style scoped>
.logo,
#home-message {
  font-size: var(--h4-size);
  font-weight: 600;
}
@media (min-width: 700px) {
  nav {
    display: inline-flex;
    justify-content: space-between;
    align-items: baseline;
    width: 100%;
  }
  ul,
  li {
    display: inline-flex;
    margin: 0 0 0 0.5rem;
  }
}
a.menuItem {
  font-size: var(--h5-size);
  font-weight: 400;
}
</style>
