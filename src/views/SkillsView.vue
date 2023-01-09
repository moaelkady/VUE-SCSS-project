<template>
  <div class="skills-view view-container">
    <p class="skills-head primary-element">Skills & Experiences</p>
    <p class="quote">
      My main area of my expertise is front end development <br />(Client side
      of the web).
      <br />
      <br />
      UI, UX, Photoshop, HTML, CSS, JS, JQuery, Bootstrap, SCSS, SASS,
      Responsive Web Pages, Media Queries, Json, VueJS, Custom plugins, hosting,
      Features, Animations and conding interactive dynamic layouts.
      <br />
      <br />
      You can See Some of my<br />
      <span class="view-link">
        <router-link to="/portfolio"> WORK</router-link>
      </span>

      or
      <span class="view-link">
        <router-link to="/contact"> CONTACT</router-link>
      </span>
      <br />
      me.
    </p>
    <br />
    <a
      class="btn my-resume"
      :href="require('../assets/gallary/myResume.webp')"
      download
    >
      Download My Resume
    </a>
  </div>
</template>
