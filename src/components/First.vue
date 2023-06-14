<template>
  <div class="main1">
    <h1>Chance Stribling</h1>
    <h3>Web Developer</h3>
    <h3>QC Analyst</h3>
    <h3>Father</h3>
    <div class="navigation">
      <v-btn variant="outlined" class="bisque" @click="scrollToExperience('experience')">Experience</v-btn>
      <v-btn variant="outlined" class="bisque" @click="scrollToExperience('skills')">Skills</v-btn>
      <v-btn variant="outlined" class="bisque" @click="scrollToExperience('projects')">Projects</v-btn>
    </div>
  </div>
</template>
<style scoped>
.bisque {
  background-color: #343e3d;
  font-size: 20px;
  width: 150px;
  color: white;
  margin-top: 5px;
}
.main1 {
  min-height: 100vh;
  width: 100vw;
  color: white;
  text-align: center;
  padding: 200px;
  background: repeating-linear-gradient(
  45deg,
  #343e3d,
  #343e3d 50px,
  #607466 50px,
  #607466 60px
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
  margin: 15px auto;
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
