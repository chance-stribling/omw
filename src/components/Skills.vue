<template>
    <div class="main3" id="skills">
        <h1 style="text-align: center; padding-top: 50px"><i>SKILLS</i></h1>
        <div style="max-width: 800px;" class="mx-auto">

            <v-row class="my-15" >
                <v-card  height="180px" width="180px"  class="card-hover mx-1 my-1" v-for="skill in skills">
                <v-card-title class="text-uppercase text-center mt-12">{{ skill.title }}</v-card-title>
                    <v-card-subtitle>
                        <v-rating
                        v-model="skill.rating"
                        readonly
                    size="x-small"
                        ></v-rating>
                    </v-card-subtitle>
            </v-card>
            </v-row>
        </div>
    </div>
  </template>
  <style scoped>

  .main3 {
    min-height: 110vh;
    width: 100vw;
    background-color: black;
    color: white;
  }
  .card-hover:hover{
    scale: 1.1;
    color: brown;
  }
  </style>
<script>
export default {
  data: () => ({
    date: null,
    skills: [
        {
            title:'css',
            rating:4,
        },
        {
            title: 'golang',
            rating: 4
        },
        {
            title: 'html',
            rating: 4
        },
        {
            title: 'java',
            rating: 4
        },
        {
            title: 'javascript',
            rating: 4
        },
        {
            title: 'php',
            rating: 3
        },
        {
            title: 'sql',
            rating: 4
        },
        {
            title: 'swift',
            rating: 4
        },
        {
            title: 'typescript',
            rating: 3
        },
        {
            title: 'agile',
            rating: 4
        },
        {
            title: 'waterfall',
            rating: 4
        },
        {
            title: 'scrum',
            rating: 4
        },
        {
            title: 'Angular JS',
            rating: 4
        },
        {
            title: 'spring boot',
            rating: 4
        },
        {
            title: 'swift ui',
            rating: 4
        }
        ,
        {
            title: 'vue js',
            rating: 4
        }
        
    ],
    
 
  })
}
</script>