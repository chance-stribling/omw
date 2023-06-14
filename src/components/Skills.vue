<template>
  <div class="main3" id="skills">
    <h1 style="text-align: center; padding: 50px; font-size: 36px"><b>SKILLS</b></h1>
    <div style="max-width: 800px" class="mx-auto">
      <v-row class="mx-auto">
        <v-card height="180px" width="180px" class="card-hover mx-auto my-1" v-for="skill in skills">
          <v-card-title class="text-uppercase text-center mt-12">{{ skill.title }}</v-card-title>
          <v-card-subtitle class="text-center text-uppercase">
            {{ skill.tag }}
          </v-card-subtitle>
        </v-card>
      </v-row>
    </div>
  </div>
</template>
<style scoped>

.main3 {
  min-height: 100vh;
  width: 100vw;
  background-color: #607466;
  color: white;
  padding-bottom: 50px;
}
.card-hover:hover {
  scale: 1.1;
  color: #7bd389;
}
</style>
<script>
export default {
  data: () => ({
    date: null,
    skills: [
      {
        title: 'css',
        tag: 'language'
      },
      {
        title: 'golang',
        tag: 'language'


      },
      {
        title: 'html',
        tag: 'language'
      },
      {
        title: 'java',
        tag: 'language'
      },
      {
        title: 'javascript',
        tag: 'language'
      },
      {
        title:  'php 8',
        tag: 'language'
      },
      {
        title: 'sql',
        tag: 'language'
      },
      {
        title: 'swift',
        tag: 'language'
      },
      {
        title: 'typescript',
        tag: 'language'
      },
      {
        title: 'agile',
        tag: 'other'
      },
      {
        title: 'waterfall',
        tag: 'other'
      },
      {
        title: 'scrum',
        rating: 5,
        tag: 'other'
      },
      {
        title: 'Angular JS',
        tag: 'framework'
      },
      {
        title: 'spring boot',
        tag: 'framework'
      },
      {
        title: 'swift ui',
        tag: 'framework'
      },
      {
        title: 'vue js',
        tag: 'framework'
      }
    ]
  })
}
</script>
