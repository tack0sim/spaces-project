<script setup>
import { defineProps } from "vue";

defineProps({
  message: String,
});
</script>

<template>
  <header class="wrapper">
    <div class="header">
      <p class="logo">Logo</p>
      <p id="home-message">{{ message }}</p>
    </div>
    <nav>
      <button id="btn_open" class="burger_menu">
        <svg viewBox="0 0 30 17" width="30" height="17" aria-hidden="true">
          <rect y="7" width="30" height="3"></rect>
          <rect y="14" width="30" height="3"></rect>
          <rect width="30" height="3"></rect>
        </svg>
      </button>

      <div class="nav_content">
        <button id="btn_close" class="nav_close">
          <svg viewBox="0 0 32 31" width="32" height="31" aria-hidden="true">
            <rect
              x="2.91846"
              y="0.297211"
              width="40"
              height="3"
              transform="rotate(45 2.91846 0.297211)"
            ></rect>
            <rect
              x="0.797363"
              y="28.5815"
              width="40"
              height="3"
              transform="rotate(-45 0.797363 28.5815)"
            ></rect>
          </svg>
        </button>
        <ul class="menu">
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
  </header>
</template>

<style scoped>
.header {
  display: inline-flex;
  justify-content: space-between;
  width: 50%;
}
.logo,
#home-message {
  font-size: var(--h4-size);
  font-weight: 600;
}

nav {
  button {
    background: none;
    border: none;
  }
  .nav_content {
    @media (max-width: 700px) {
      position: fixed;
      inset: 0 0 0 40%;
      background-color: gray;
    }
  }
  .nav_close {
    display: block;
    margin-left: auto;
  }
}

.burger_menu {
  display: block;
}

/** breakpoint for 700px wide and beyond */
@media (min-width: 700px) {
  nav {
    display: inline-flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
  }
  #btn_close {
    display: none;
  }
  ul,
  li {
    display: inline-flex;
    margin: 0 0 0 0.5rem;
  }
  .line {
    display: none;
  }
}
a.menuItem {
  font-size: var(--h5-size);
  font-weight: 400;
}
</style>
