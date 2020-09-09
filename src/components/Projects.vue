<template>
  <section id="projects" class="project-section">
    <v-container>
      <v-row>
        <v-col>
          <h1 class="text-center">Projects</h1>
        </v-col>
      </v-row>
      <v-row class="justify-space-around mb-8 mt-4">
        
        <v-card
          v-for="project in projects"
          :key="project.name"
          class=""
          max-width="300"
        >
          <v-img
            class="align-end"
            height="200px"
            :src="project.image"
          />
          <v-card-title>{{ project.name }}</v-card-title>

          <v-card-text class="text--primary">
            {{ truncate(project.description) }}
          </v-card-text>

          <v-card-actions>
            <v-btn
              color="orange"
              text
              :href="project.github"
            >
              Github Repo
            </v-btn>

          </v-card-actions>
        </v-card>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          name: 'Planting Website',
          github: 'https://github.com/',
          description: 'This is a great app.',
          image: 'https://assets.codepen.io/3765537/proj1.jpg'
        },
        {
          name: 'Laptop Project',
          github: 'https://github.com',
          description: 'This feels like a great app, but it is not.',
          image: 'https://assets.codepen.io/3765537/proj2.jpg'
        },
        {
          name: 'Hiking App',
          github: 'https://github.com',
          description: 'What does this feel like?',
          image: 'https://assets.codepen.io/3765537/proj3.jpg'
        }
      ]
    }
  },
  methods: {
    truncate(str) {
      if (str.length > 80) {
        return str.slice(0, 79) + '...'
      }
      return str
    }
  }
}
</script>

<style scoped>
.project-section {
  /* background-color: #f9f8f7; */
}
.v-image {
  border-bottom: 1px solid;
}
</style>