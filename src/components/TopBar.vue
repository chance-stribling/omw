<template>
  <v-app-bar color="black" density="compact">
    <template v-slot:prepend>
      <v-app-bar-title class="bisque pointer" @click="scrollToTop">{{ title }}</v-app-bar-title>
    </template>

    <template v-slot:append>
      <v-btn>
        <v-icon class="bisque" icon="mdi-email-box" @click="copyToClip"></v-icon>
        <v-tooltip activator="parent" location="start" class="text-center"
          >Copy Email to Clipboard</v-tooltip
        >
      </v-btn>
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
    },
    copyToClip() {
      var copyText = 'cstribling1717@gmail.com'
      navigator.clipboard.writeText(copyText)
      window.alert('Copied "' + copyText + '" to clipboard')
    }
  }
}
</script>
