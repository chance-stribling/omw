<template>
  <div class="cover">

        <div style="max-width: 100%;">

          <h1 class="text-uppercase" id="billboard">
            SKILLS 
          </h1>
        </div>

  </div>
  <div class="main3" id="skills">
    <h1 style="text-align: center; padding: 50px; font-size: 36px"><b>SKILLS</b></h1>
    <div style="max-width: 800px" class="mx-auto">
      <v-row class="mx-auto">
        <v-card height="180px" width="180px" class="prevent-select card mx-auto my-1" :id="'card'+ skill.id" v-for="skill in skills" @mouseover="backgroundChange(skill.title)">
          <v-card-title class="text-uppercase text-center mt-15">{{ skill.title }}</v-card-title>

        </v-card>
      </v-row>
    </div>
  </div>
</template>
<style scoped>
.cover{
  height: 140vh;
  width: 100vw;
  position: absolute;
  background-color: transparent;
  font-size: 100px;
  color: white;
  text-align: center;
  overflow: hidden;
}
#billboard{
  transform: translateY(100%);
}
@media screen and (max-width: 600px) {
  #billboard{
  transform: translateY(800%);
}
.cover{

  font-size: 20px;
}
}
.main3 {
  min-height: 100vh;
  width: 100vw;
  background-color: #607466;
  color: white;
  padding-bottom: 50px;
}
.prevent-select {

  user-select: none; /* Standard syntax */
}
.card:hover {
  scale: 1.1;
  color: #7bd389;
  opacity: 90%;
}
.card{
  
  opacity: 20%;
}

</style>
<script>
export default {
  methods:{
    backgroundChange: function(name){
        document.getElementById('billboard').innerHTML= name;   

    }
  },
  data: () => ({
    date: null,
    skills: [
      {
        title: 'golang',
        tag: 'language',
        id:1,
        shaped: false


      },
      {
        title: 'html',
        tag: 'language',
        id:2,
        shaped: false
      },
      {
        title: 'java',
        tag: 'language',
        id:3,
        shaped: false
      },
      {
        title: 'javascript',
        tag: 'language',
        id:4,
        shaped: false
      },
      {
        title:  'php 8',
        tag: 'language',
        id:5,
        shaped: false
      },
      {
        title: 'sql',
        tag: 'language',
        id:6,
        shaped: false
      },
      {
        title: 'swift',
        tag: 'language',
        id:7,
        shaped: false
      },
      {
        title: 'typescript',
        tag: 'language',
        id:8,
        shaped: false
      },
      {
        title: 'aws amplify',
        tag: 'other',
        id:16,
        shaped: false
      },
      {
        title: 'agile',
        tag: 'other',
        id:9,
        shaped: false
      },
      {
        title: 'waterfall',
        tag: 'other',
        id:10,
      
        shaped: false
      },
      {
        title: 'scrum',
        rating: 5,
        tag: 'other',
        id:11,
        shaped: false
      },
      {
        title: 'Angular JS',
        tag: 'framework',
        id:12,
        shaped: false
      },
      {
        title: 'spring boot',
        tag: 'framework',
        id:13,
        shaped: false
      },
      {
        title: 'swift ui',
        tag: 'framework',
        id:14,
        shaped: false
      },
      {
        title: 'vue js',
        tag: 'framework',
        id:15,
        shaped: false
      }
    ]
  })
}
</script>
