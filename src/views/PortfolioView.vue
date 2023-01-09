<template>
  <div class="portfolio-view view-container container">
    <div class="row gallary-row">
      <div
        class="progect-container col-6 col-sm-6 col-md-4 col-lg-3 col-xl-3"
        v-for="project in projects"
        :key="project.id"
      >
        <div class="project-cover-holder">
          <div
            class="project-cover"
            :style="{ backgroundImage: 'url(' + project.imgUrl + ')' }"
          >
            <div class="hover-content">
              <div class="content-border">
                <h4>{{ project.title }}</h4>
                <button class="btn" @click="project.status = !project.status">
                  See More
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="project-description" v-if="project.status">
          <div class="description-hold">
            <h3>{{ project.title }}</h3>
            <hr />
            <p>{{ project.description }}</p>
            <a :href="project.link" target="_blank" class="btn">
              Live Project
            </a>
            <span @click="project.status = false">X</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import projects from "../../projects.json";
export default {
  name: "portfolioView",
  data: function () {
    return {
      projects: projects,
    };
  },
};
</script>
