<template>
  <div class="home-view view-container">
    <div class="head">
      <p>
        <span class="letter"> Hello </span>
        <br />
        <span class="letter">I'm Mohamed ElQadi </span>
      </p>
      <p>
        <span class="letter"> UI/UX </span>
        <br />
        <span class="letter"> Full Stack Developer </span>
      </p>
    </div>
    <div class="paragraph">
      <p>This Is My Personal Website</p>
      <p>You Can</p>
    </div>
    <div class="buttons">
      <router-link to="/about" class="btn">Know More About Me</router-link>
      <p>
        <span>OR</span>
      </p>
      <router-link to="/contact" class="btn">Contact Me</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeView",
};
</script>
