<template>
  <div class="main1">
    <h1>Chance Stribling</h1>
    <h3>Web Developer</h3>
    <h3>QC Analyst</h3>
    <h3>Father</h3>
    <div class="navigation">
      <v-btn class="bisque" @click="scrollToExperience('experience')">Experience</v-btn>
      <v-btn class="bisque" @click="scrollToExperience('skills')">Skills</v-btn>
      <v-btn class="bisque" @click="scrollToExperience('projects')">Projects</v-btn>
    </div>
  </div>
</template>
<style scoped>
.bisque {
  background-color: bisque;
  font-size: 20px;
  width: 150px;
}
.main1 {
  max-height: 100vh;
  width: 100vw;
  color: white;
  text-align: center;
  padding: 200px;
  background: repeating-linear-gradient(
  45deg,
  rgb(74, 74, 74),
  rgb(74, 74, 74) 50px,
  black 50px,
  black 60px
);
}
.main1 h1,
h3 {
  font-weight: bold;
}

.navigation {
  margin-top: 50px;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}
@media only screen and (max-width: 600px) {
  .navigation{
    display: flex;
  flex-direction: column;
  width: 50vw;
  }
}
</style>
<script>
export default {
  data: () => ({
    title: 'CS'
  }),
  methods: {
    scrollToTop() {
      window.scrollTo(0, 0)
    },
    scrollToExperience(elementId) {
      const element = document.getElementById(elementId)

      element.scrollIntoView()
    }
  }
}
</script>
