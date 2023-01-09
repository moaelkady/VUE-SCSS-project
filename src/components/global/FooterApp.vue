<template>
  <div class="footer-app">
    <ul>
      <router-link to="/about">
        <li><font-awesome-icon icon="fa-solid fa-user" /></li>
        <span class="description">About Me</span>
      </router-link>
      <router-link to="/portfolio">
        <li><font-awesome-icon icon="fa-solid fa-eye" /></li>
        <span class="description">My Portfolio</span>
      </router-link>
      <router-link to="/contact">
        <li><font-awesome-icon icon="fa-solid fa-envelope" /></li>
        <span class="description">Contact Me</span>
      </router-link>
    </ul>
  </div>
</template>

<script>
export default {
  name: "FooterApp",
};
</script>
