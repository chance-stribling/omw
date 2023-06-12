<template>
  <div class="main3" id="skills">
    <h1 style="text-align: center; padding: 50px"><i>SKILLS</i></h1>
    <div style="max-width: 800px" class="mx-auto">
      <v-row class="mx-auto">
        <v-card height="180px" width="180px" class="card-hover mx-auto my-1" v-for="skill in skills">
          <v-card-title class="text-uppercase text-center mt-12">{{ skill.title }}</v-card-title>
          <v-card-subtitle>
            <v-rating v-model="skill.rating" readonly size="x-small"></v-rating>
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
        rating: 5
      },
      {
        title: 'golang',
        rating: 4
      },
      {
        title: 'html',
        rating: 5
      },
      {
        title: 'java',
        rating: 5
      },
      {
        title: 'javascript',
        rating: 5
      },
      {
        title: 'php',
        rating: 5
      },
      {
        title: 'sql',
        rating: 5
      },
      {
        title: 'swift',
        rating: 5
      },
      {
        title: 'typescript',
        rating: 5
      },
      {
        title: 'agile',
        rating: 5
      },
      {
        title: 'waterfall',
        rating: 5
      },
      {
        title: 'scrum',
        rating: 5
      },
      {
        title: 'Angular JS',
        rating: 5
      },
      {
        title: 'spring boot',
        rating: 5
      },
      {
        title: 'swift ui',
        rating: 5
      },
      {
        title: 'vue js',
        rating: 5
      }
    ]
  })
}
</script>
