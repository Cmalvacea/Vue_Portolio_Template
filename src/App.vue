<script setup>
import Navigation from './components/Navigation.vue'
import FirstSection from './components/FirstSection.vue'
import SecondSection from './components/SecondSection.vue'
import ContactSection from './components/ContactSection.vue'
import Portfolio from './components/Portfolio.vue'
import Footer from './components/Footer.vue'


</script>

<template>
  <Navigation :Sections="SectionList" />
  <FirstSection :Content="TextContent1" />
  <SecondSection :Content2="TextContent2"/>
  <ContactSection :Medias="MediaList"/>
  <Portfolio :Areas="PortfolioContent"/>
  <Footer/>
</template>

<script>
export default {
  data() {
    return {
      SectionList: ['Section1', 'Section2', 'Section3', 'Section4'],
      TextContent1: {
        Title: "First Page",
        Content: "This is the content of the first page!"
      },
      TextContent2: {
        Title: "Second Page",
        Content: "Glad you're here, this is the second section",
      },
      MediaList: [
        {
          MediaName: "Github",
          Link: '#'
        },
        {
          MediaName: "Linkedin",
          Link: '#'
        },
        {
          MediaName: "Youtube",
          Link: '#'
        },
        {
          MediaName: "Upwork",
          Link: '#'
        },
      ],
      PortfolioContent: [{
                Skill_Name: "Skill Number 1",
                Projects: [{
                    Project_Name: "Project 1",
                    Project_Details: "Project Description"
                },{
                    Project_Name: "Project 2",
                    Project_Details: "Project Description" 
                }, {
                    Project_Name: "Project 3",
                    Project_Details: "Project Description"
                }]
            },{
                Skill_Name: "Skill Number 2",
                Projects: [{
                    Project_Name: "Project 1",
                    Project_Details: "Project Description"
                },{
                    Project_Name: "Project 2",
                    Project_Details: "Project Description" 
                }, {
                    Project_Name: "Project 3",
                    Project_Details: "Project Description"
                }]
            }, {
                Skill_Name: "Skill Number 3",
                Projects: [{
                    Project_Name: "Project 1",
                    Project_Details: "Project Description"
                },{
                    Project_Name: "Project 2",
                    Project_Details: "Project Description" 
                }, {
                    Project_Name: "Project 3",
                    Project_Details: "Project Description"
                }]
            }],

    }
  }
}


</script>
