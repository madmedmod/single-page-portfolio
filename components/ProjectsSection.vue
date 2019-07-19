<template>
  <div id="projects" class="projects-section">
    <h2 class="projects-section-header">
      Here are my projects
    </h2>
    <div class="projects-grid">
      <div
        v-for="project in projects"
        :key="project.id"
        class="project project-title"
        target="_blank"
      >
        <img :src="`img/${project.image}`" alt="" class="project-image" />
        <a :href="project.url" target="_blank">
          <h2 class="project-title">{{ project.name }}</h2>
        </a>
        <!-- <nuxt-link :to="project.url" target="_blank">
          <h2 class="project-title">{{ project.name }}</h2>
        </nuxt-link> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          name: 'Tribute Page',
          description: 'Description here',
          image: 'tribute-page.JPG',
          url: '/tribute-page'
        },
        {
          name: 'Survey Form',
          description: 'Description here',
          image: 'survey-form.JPG',
          url: '/survey-form'
        },
        {
          name: 'CRUD App with REST',
          description: 'Description here',
          image: 'crud-app.JPG',
          url: 'https://crud-app-with-rest.herokuapp.com/'
        },
        {
          name: 'Shopping List App',
          description: 'Description here',
          image: 'shopping-list-app.JPG',
          url: '/shopping-list-app'
        },
        {
          name: 'Github Profiles',
          description: 'Description here',
          image: 'github-profiles-app.JPG',
          url: '/github-profiles-app.html'
        },
        {
          name: 'Form Validation',
          description: 'Description here',
          image: 'form-validation-app.JPG',
          url: 'https://intense-plateau-42945.herokuapp.com/index.html'
        }
      ]
    }
  }
}
</script>

<style></style>
