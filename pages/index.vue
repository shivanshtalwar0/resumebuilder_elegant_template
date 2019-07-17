<template>
  <div class="bg">
    <v-layout row wrap>
      <v-flex xs4>
        <v-card width="auto" height="auto" style="height:100vh;background-color:#F5F5F5;">
          <v-layout row wrap width="auto" height="10em" class="" style="background-color: #ffffff;">
            <v-flex pt-2 xs12 text-xs-center>
              <v-avatar
                size="180px"

                color="grey lighten-4"
              >
                <img width="200" height="200" :src="myimage" alt="avatar"/>
              </v-avatar>
            </v-flex>

            <v-flex text-xs-center xs12>
              <h2 class="black--text">{{myname}}</h2>
            </v-flex>
            <v-flex text-xs-center xs12 pb-2>
              <span class="font-italic white--text">Full-Stack Web Developer</span>
            </v-flex>


          </v-layout>


          <v-layout row wrap width="auto" class="" style="background-color: #F5F5F5;">
            <v-layout mt-4 row wrap>
              <v-flex v-for="element in leftpannel" :key="element.text" xs12>
                <v-layout row wrap>

                  <v-flex xs2>

                    <v-icon class="black--text ml-2" v-html="element.icon"></v-icon>
                  </v-flex>
                  <v-flex xs10>
                    <p class=" black--text">{{element.text}}</p>
                  </v-flex>

                </v-layout>

              </v-flex>

            </v-layout>
            <v-layout row wrap>
              <v-container>
                <h2 class="text-xs-left black--text font-weight-bold">OBJECTIVE</h2>
                <p class="black--text font-weight-medium">
                  Take advantage of my technical skills and experience to become a professional
                  Developer and bring a lot value to Organisation that i will be working in, going to work in dynamic
                  working environment with challenges to develop myself.
                  From that I will Contribute to development of your Organisation.


                </p>
              </v-container>

            </v-layout>
            <v-layout row wrap>
              <v-container>
                <h2 class="text-xs-left black--text font-weight-bold">INTERPERSONAL SKILLS</h2>

                <v-layout row wrap>
                  <v-flex xs12>
                    <ul>
                      <li v-for="element in skills" :key="element.text">
                        <h4 class="black--text">{{element.text}}</h4>
                      </li>

                    </ul>

                  </v-flex>
                </v-layout>

              </v-container>

            </v-layout>

            <v-layout row wrap>
              <v-container>
                <h2 class="text-xs-left black--text font-weight-bold">CERTIFICATIONS</h2>

                <v-layout row wrap>
                  <v-flex xs12>
                    <ul>
                      <li v-for="element in certifications" :key="element.text">
                        <h4 class="black--text">{{element.text}}</h4>
                      </li>

                    </ul>

                  </v-flex>
                </v-layout>

              </v-container>

            </v-layout>


          </v-layout>

          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
          <v-layout pb-5></v-layout>
        </v-card>

      </v-flex>

      <v-flex xs8>


        <v-layout row wrap>
          <v-flex xs12>
            <v-container fluid>
              <v-layout row wrap>

                <div class="circle">
                  <v-icon large class="large text-xs-center white--text">school</v-icon>
                </div>

                <h2 class="ml-3 mt-2 font-weight-bold">EDUCATION</h2>


              </v-layout>
              <v-layout row wrap>
                <v-flex v-for="education in educations" :key="education.institutename" ma-4 xs12>

                  <v-layout row wrap>
                    <v-flex xs9>
                      <h3><b>{{education.institutename}}</b></h3>
                    </v-flex>
                    <v-flex xs3>
                      <h3><i>{{education.completiontime}}</i></h3>
                    </v-flex>
                  </v-layout>

                  <span v-if="education.type==='school'"><i>{{education.board}}</i></span>
                  <br>
                  <span v-if="education.type!=='school'"><i>{{education.major}}</i></span>
                  <br v-if="education.type!=='school'">
                  <span><i>CGPA/Percentage:</i>{{education.percentage}}</span>
                </v-flex>


              </v-layout>


            </v-container>
          </v-flex>
        </v-layout>


        <v-flex xs12>
          <v-container>

            <v-layout row wrap>

              <div class="circle">
                <v-icon large class="large text-xs-center white--text">work</v-icon>
              </div>

              <h2 class="ml-3 mt-2 font-weight-bold">WORK EXPERIENCE</h2>
            </v-layout>
            <v-container>
              <ol>
                <li v-for="(exp,key) in experience">
                  <v-layout row wrap>
                    <v-flex xs9>

                      <h3>{{exp.title}}</h3>
                    </v-flex>
                    <v-flex xs3>
                      <h3><b><i>{{exp.time}}</i></b></h3>

                    </v-flex>
                  </v-layout>
                  <v-layout>
                    <v-flex xs12><i class="grey--text darken-2">{{exp.designation}}</i></v-flex>


                  </v-layout>

                  <ul v-for="(resp,resk) in exp.responsibilities">
                    <li>{{resp}}</li>
                  </ul>


                </li>
              </ol>

            </v-container>


          </v-container>


        </v-flex>


        <v-flex xs12>
          <v-container>

            <v-layout row wrap>

              <div class="circle">
                <v-icon large class="large text-xs-center white--text">insert_chart</v-icon>
              </div>
              <h2 class="ml-3 mt-2 font-weight-bold">TECHNICAL SKILLS</h2>
            </v-layout>
            <v-container>
              <ul>
                <li style="list-style: square;" v-for="skill in technicalskills" :key="skill.technology"><h3>
                  {{skill.technology}}</h3></li>
              </ul>

            </v-container>


          </v-container>


        </v-flex>


        <v-flex xs12>
          <v-container>

            <v-layout row wrap>

              <div class="circle">
                <v-icon large class="large text-xs-center white--text">assignment_turned_in</v-icon>
              </div>

              <h2 class="ml-3 mt-2 font-weight-bold">PROJECTS</h2>
            </v-layout>

            <ol class="ma-4">
              <li class="mt-3" v-for="element in projects" :key="element.title">
                <v-layout row wrap>
                  <v-flex xs12>
                    <h3><b>{{element.title}}</b></h3>
                  </v-flex>
                  <v-flex xs12>
                    <h4 class="ml-1"><i>Description</i></h4>
                    <i><p>
                      {{element.description}}
                    </p></i>
                    <h4 class="ml-1"><i>Project URL</i></h4>
                    <h4 class="ml-1 grey--text">{{element.url}}</h4>

                  </v-flex>

                </v-layout>
              </li>

            </ol>

          </v-container>
        </v-flex>


      </v-flex>


    </v-layout>


  </div>
</template>

<script>

  import axios from 'axios'
  import rowcontainer from '../components/rowcontainer'

  export default {

    loading: false,
    loadingindicator: false,
    // fetch()

    methods: {
      settitle(response) {
        this.title = response.data.title
      }
    },

    head() {
      return {

        title: this.title,
        meta: [
          {charset: 'utf-8'},
          {name: 'viewport', content: 'width=device-width, initial-scale=1'},
          {hid: 'keywords', name: 'keywords', content: 'vuejs, nuxt, javascript, tutorials, development, software'},
          {hid: 'description', name: 'description', content: "custom description"}
        ],
        link: [
          {rel: 'icon', type: 'image/x-icon', href: '/favicon.ico'},
          {
            rel: 'stylesheet',
            href:
              'https://fonts.googleapis.com/css?family=Roboto:300,400,500,700|Material+Icons'
          }
        ]
      }
    },
    components: {},
    data() {
      return {
        myname:"Shivansh Talwar",

        myimage:"/shiv5.jpg",
        //put your image in static directory and change /shiv5.jpg to your image name
        educations:[
          {institutename:"Greenway Modern School",
          type:"school",
            completiontime:"2016",
            board:"CBSE Board",
            percentage:"76%"
          },
          {institutename:"Abdul Kalam Technical University,Lucknow",
            type:"college",
            completiontime:"2016-2020",
            board:"CBSE Board",
            percentage:"70%",
            major:"B-Tech in Computer Science"
          }

        ],

        certifications: [
          {text: 'Certificate In Java Programming'},
          {text: 'Python & its Application with IOT'},
        ],
        experience: [

          {
            title: 'Intern At Hanusha Networks Private Limited',
            time: '1 June 2019-Present',
            responsibilities: [
              'Development & Designing of SportsApp',
              'Managing SportsApp Deployment on Web Servers',
              'Debugging & Bug Fixing Of SportsApp'

            ],
            designation: 'Full-Stack Web Developer'
          },
          {
            title: 'Techsbotics Inc ,Ohio,USA',
            time: 'March 2018-Present',
            responsibilities: [
              'Development & Designing of Web-Applications',
              'Managing Web-App Deployment on Web Servers',
              'Debugging & Bug Fixing Of Web-Applications'

            ],
            designation: 'Full-Stack Web Developer'
          },


        ],

        projects: [
          {
            title: "Proxychecker",
            description: " High Performant,MultiThreaded, C Based proxy checker Tool which makes validating and checking millions of proxy in almost no time.",
            url: "https://github.com/shivanshtalwar0/proxychecker"
          },
          {
            title: "Dr. John's Nutrition Health Portal",
            description: "A Freelance Project Based on Vue.js to help Dr. John Share his Knowledge among his clients ",
            url: "https://drjohnsnutritionhealthportal.com/login"
          },
          {
            title: "Messenger clone",
            description: "A  Project Based on Nuxt.js ,having almost all features and functionality of Facebook Messenger",
            url: "http://messenger-9ea45.firebaseapp.com/signup"
          },
          {
            title: "FireNDCNPP",
            description: "A  Project Based on Nuxt.js ,used to fill petition on the political problem of Ghana",
            url: "https://firendcnpp.com"
          },


        ],
        leftpannel: [
          {icon: "calendar_today", text: "6 January 1998"},
          {icon: "email", text: "shivanshtalwar0@gmail.com"},
          {icon: "phone", text: "+918744849050"},
          {icon: "location_on", text: "B-52/A-1,Dilshad Colony,Delhi-95"},


        ],

        skills: [
          {text: "Good analytical and problem solving skills.", score: 85},
          {text: "Good Communication Skills", score: 80},

          {text: "self-confident and hard working nature.", score: 80},
          {text: "Ability to work both independently and as a team player.", score: 70},


        ],


        
        technicalskills: [
          {
            technology: 'Nuxt.js',

          },
          {
            technology: 'Vue.js',

          },
          {
            technology: 'SPA & PWA using Vue.js',

          },

          {
            technology: 'HTML5',

          },
          {
            technology: 'CSS3',

          },
          {
            technology: "Linux",

          },
          {
            technology: 'Web Scrapping using Selenium (python) ',

          },


          {
            technology: 'Google Firebase',

          },

          {
            technology: "Flutter & Dart (Cross-Platform Native Mobile Application)"

          },
          {
            technology: "Python",

          },
          {
            technology: 'Node.js & Express.js',

          },
          {
            technology: "PHP",

          },
          {
            technology: 'Mysql',

          },
          {
            technology: 'C & C++',

          },

          {
            technology: 'Java',

          },


        ]


      }


    }
  }
</script>
<style>
  .bg {
    background-image: url(/niet.png);
    background-position: 99.2% 8px;
    background-size:10em 10em;
    background-clip: content-box;


  }

  .circle {
    height: 50px;
    width: 50px;
    background-color: black;
    padding-top: 7px;
    padding-left: 7px;
    border-radius: 50%;
    display: inline-block;

  }

</style>
