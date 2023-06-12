<template>
    <v-footer
      class="bg-brown-lighten-1 text-center d-flex flex-column"
    >
      <div>
        <v-btn
          v-for="item in icons"
          :key="item"
          class="mx-4"
          :icon="item.icon"
          variant="text"
        ></v-btn>
      </div>
  
      <div class="pt-0">
        Perseverance is not a long race; it is many short races one after the other.
      </div>
  
      <v-divider></v-divider>
  
      <div>
         <strong>- Walter Elliot</strong>
      </div>

    </v-footer>
  </template>

  <script>
  export default {
    data: () => ({
      icons: [
        {
            icon:'mdi-github',
            to:'github.com/chance-stribling',
        }
      ],
    }),
  }
</script>