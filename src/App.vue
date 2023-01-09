<template>
  <header-app />
  <sidebar-app />
  <footer-app />
  <router-view />
</template>

<style lang="scss">
html {
  background-image: url("./assets/bg1.webp");
  max-height: 100%;
  min-height: 100%;
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  background-attachment: fixed;
}
body {
  background-color: transparent !important;
}
</style>

<script>
import HeaderApp from "./components/global/HeaderApp.vue";
import SidebarApp from "./components/global/SidebarApp.vue";
import FooterApp from "./components/global/FooterApp.vue";

export default {
  name: "HomeView",
  components: { HeaderApp, SidebarApp, FooterApp },
};
</script>
