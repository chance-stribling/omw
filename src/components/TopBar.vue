<template>
  <v-app-bar color="black" density="compact">
    <template v-slot:prepend>
      <v-app-bar-title class="bisque pointer" @click="scrollToTop()">{{ title }}</v-app-bar-title>
    </template>

    <template v-slot:append>
      <v-btn class="bisque" icon="mdi-dots-vertical"></v-btn>
    </template>
  </v-app-bar>
</template>
<style scoped>
.bisque {
  color: bisque;
}
.pointer {
  cursor: pointer;
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
    }
  }
}
</script>
