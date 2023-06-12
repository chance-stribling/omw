<template>
    <div class="main3" id="projects">
        <h1 style="text-align: center; padding-top: 50px"><i>Projects</i></h1>
        <div style="max-width: 70vw;" class="mx-auto my-5">

            <v-row class="my-15" >
                <v-card  min-height="200px" width="70vw" color="black"  class="card-hover mx-1 my-1" v-for="project in projects">
                <v-card-title  class="text-center mt-12">{{ project.title }}</v-card-title>
                <v-card-text style="font-size: 16px;" class="px-15">

        {{project.description}}
      </v-card-text>
      <v-card-actions class="justify-center" v-if="project.action">
      <a href="https://chance-stribling.github.io/stribbles-and-bits/#/">

          <v-btn variant="outlined" color="white" >
              Link
            </v-btn>
        </a>
    </v-card-actions>
            </v-card>
            </v-row>
        </div>
    </div>
  </template>
  <style scoped>

  .main3 {
    height: 120vh;
    width: 100vw;
    background-color: white;
    color: black;
  }
  .card-hover:hover{
    scale: 1.01;
    color: brown;
  }
  </style>
<script>
export default {
  data: () => ({
    date: null,
    projects: [
        {
            title: 'i3 Verticals Developer Demo Project',
            description: 'Worked closely in a team of three to develop a smartwatch prototype. Utilized an Arduino board, 3D modeling and printing, and developed with GoLang.',
            action: true
        },
        {
            title: 'Golang Smart Watch',
            description: 'Worked closely in a team of three to develop a smartwatch prototype. Utilized an Arduino board, 3D modeling and printing, and developed with GoLang.',
        },
        {
            title:'EBR Schoolboard Campaign',
            description:'Developed and hosted a webpage for an educator running for the East Baton Rouge Parish School Board for 3 months using Wix services.',
        },
        {
            title: 'Syllabus Manager',
            description:'Worked with a team of trainees to develop a syllabus manager for future training programs. Utilized Angular for the front end and Spring Boot and MySQL were used for the back end and database respectively.',
        },
    ],
    
 
  })
}
</script>