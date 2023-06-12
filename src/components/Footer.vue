<template>
    <v-footer
      class="bg-brown-lighten-1 text-center d-flex flex-column"
    >
      <div class="my-5">
        
          <v-btn
          @click="gh"
          icon="mdi-github"
          class="mx-5"
          ></v-btn>
          <v-btn
          @click="li"
          icon="mdi-linkedin"
          class="mx-5"

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

    methods:{
      gh: function(){
        window.location.href = 'https://www.github.com/chance-stribling';

      },
      li: function(){
        window.location.href = 'https://linkedin.com/in/chance-stribling';

      }
    }
  }
</script>