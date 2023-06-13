<template>
  <div class="main2" id="experience">
    <h1 style="text-align: center; padding-top: 50px"><i>EXPERIENCE</i></h1>
    <div class="panels mx-auto">
      <v-expansion-panels variant="popout">
        <v-expansion-panel v-for="job in jobs">
          <v-expansion-panel-title color="#607466" class="text-white">
            <v-row style="line-height: 50px">
              <v-col cols="4" class="d-flex justify-start font-weight-black bigger">
                {{ job.title }}
              </v-col>
              <v-col cols="3" class="d-flex justify-start font-weight-bold">
                {{ job.location }}
              </v-col>
              <v-col cols="5" class="text--secondary">
                <v-row style="width: 100%">
                  <v-col cols="6" class="d-flex justify-start">
                    Start Date: {{ job.start || 'Not set' }}
                  </v-col>
                  <v-col cols="6" class="d-flex justify-start">
                    End date: {{ job.end || 'Current' }}
                  </v-col>
                </v-row>
              </v-col>
            </v-row>
          </v-expansion-panel-title>
          <v-expansion-panel-text class="expan">
            <v-list class="pa-0">
              <v-list-item
                v-for="description in job.descriptions"
                :key="description"
                style="background-color: #343e3d; color: white; width: 100%;"
              >
            <v-list-title>{{ description }}</v-list-title>
            </v-list-item>
            </v-list>
          </v-expansion-panel-text>
        </v-expansion-panel>
      </v-expansion-panels>
    </div>
  </div>
</template>
<style scoped>


.bigger {
  font-size: 20px;
}
.expan {
  background-color: #343e3d;
  color: white;
}
.panels {
  width: 90vw;
  padding: 50px 0;
}
.main2 {
  min-height: 94vh;
  background-color: #aedcc0;
}
ul {
  line-height: 40px;
}
</style>

<script>
export default {
  data: () => ({
    date: null,

    jobs: [
      {
        title: 'Web Developer',
        location: 'i3 Verticals',
        start: 'May 2023',
        end: 'June 2023',
        descriptions: [
          'Working in an Agile Software Development lifecycle.',
          'Analyzing user and industry requirements, envisioning system features and functionality, and working with the team to bring them to life.',
          'Designing and Implementing User Interfaces and Backend Systems, including Database Design and Interfacing with 3rd Party systems.'
        ]
      },
      {
        title: 'QC Analyst',
        location: 'i3 Verticals',
        start: 'December 2023',
        end: 'Current',
        descriptions: [
          'Perform manual and automated tests to ensure the software developed by developers is fit to use.',
          'Communicate test progress, test results, and other relevant information to project managers.',
          'Analyze user stories and requirements for validity and feasibility.'
        ]
      },
      {
        title: 'Java Developer',
        location: 'CGI Federal',
        start: 'May 2022',
        end: 'July 2022',
        descriptions: [
          'Was introduced to Agile methodologies in an enterprise setting.',
          'Used Spring Boot, H2, NodeJs, and AngularJS to make a syllabus manager for future training.',
          'Studied and introduced to Mockito for software QA (unit testing).'
        ]
      },
      {
        title: 'Network Technician',
        location: 'Motion Lite Service',
        start: 'February 2022',
        end: 'May 2022',
        descriptions: [
          'Maintained and improved infrastructure for clients.',
          'Ran CAT 5e/6 cable, troubleshot network equipment, and installed software.',
          'Provided leadership in developing and implementing solutions and offering technical support and consultation.'
        ]
      },
      {
        title: 'Repair Technician',
        location: 'UBreakIFix by Asurion',
        start: 'February 2021',
        end: 'February 2022',
        descriptions: [
          'Troubleshot and repaired mobile devices, televisions, PCs, and various other devices with interchangeable parts. ',
          'Kept in constant contact with customers to inform them of the status of their repairs and walked them through the next steps.'
        ]
      },
      {
        title: 'QA Tester',
        location: 'Electronic Arts Studio',
        start: 'October 2020',
        end: 'February 2021',
        descriptions: [
          'Tasked with using Jira and TestRail to locate and validate any bugs found while testing. ',
          'Trained to follow proper beta testing procedures and how to make testing reports.',
          'Used beta testing skills from Quality Assurance Training to stress test many features of the game on several types of gaming consoles. ',
          'Successfully found and documented bugs in the software in order to make a more user-friendly gaming experience.'
        ]
      }
    ]
  })
}
</script>
