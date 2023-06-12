<script setup>
import TopBar from './components/TopBar.vue'
import First from './components/First.vue'
import Experience from './components/Experience.vue'
import Skills from './components/Skills.vue'
import Projects from './components/Projects.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <v-app>
    <header>
      <TopBar />
    </header>
    <v-container fluid class="pa-0">
      <v-main>
        <First />
        <Experience />
        <Skills />
        <Projects />
        <Footer />
      </v-main>
    </v-container>
  </v-app>
</template>

<style scoped></style>
