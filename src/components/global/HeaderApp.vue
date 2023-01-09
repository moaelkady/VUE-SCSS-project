<template>
  <div class="header-app">
    <div class="logo">
      <img
        src="../../assets/logo.webp"
        alt="Logo Img"
        class="my-logo"
        width="50px"
        height="50px"
      />
      <span class="primary-element">Q</span><span class="adidev">adi Dev</span>
    </div>
    <ul class="nav">
      <router-link to="/">
        <li><font-awesome-icon icon="fa-solid fa-home" /></li>
      </router-link>
      <router-link to="/about">
        <li><font-awesome-icon icon="fa-solid fa-user" /></li>
      </router-link>
      <router-link to="/skills">
        <li><font-awesome-icon icon="fa-solid fa-cogs" /></li>
      </router-link>
      <router-link to="/portfolio">
        <li><font-awesome-icon icon="fa-solid fa-eye" /></li>
      </router-link>
      <router-link to="/contact">
        <li><font-awesome-icon icon="fa-solid fa-envelope" /></li>
      </router-link>
    </ul>
    <!--Menu for mobile screens-->
    <div class="bars-menu">
      <span class="bars-menu-toggler" @click="barsMenu = !barsMenu">
        <font-awesome-icon icon="fa-solid fa-bars" />
      </span>
      <Transition name="slide-fade">
        <div class="bars-menu-container" v-if="barsMenu">
          <ul class="bars-nav">
            <router-link to="/" @click="barsMenu = false">
              <li><font-awesome-icon icon="fa-solid fa-home" /></li>
            </router-link>
            <router-link to="/about" @click="barsMenu = false">
              <li><font-awesome-icon icon="fa-solid fa-user" /></li>
            </router-link>
            <router-link to="/skills" @click="barsMenu = false">
              <li><font-awesome-icon icon="fa-solid fa-cogs" /></li>
            </router-link>
            <router-link to="/portfolio" @click="barsMenu = false">
              <li><font-awesome-icon icon="fa-solid fa-eye" /></li>
            </router-link>
            <router-link to="/contact" @click="barsMenu = false">
              <li><font-awesome-icon icon="fa-solid fa-envelope" /></li>
            </router-link>
          </ul>
        </div>
      </Transition>
    </div>
    <!--menu for mobile screens-->
  </div>
</template>

<script>
export default {
  name: "HeaderApp",
  data: function () {
    return {
      barsMenu: false,
    };
  },
};
</script>
