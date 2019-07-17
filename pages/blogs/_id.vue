<template>
    <div>

      <v-layout row wrap>
        <v-flex xs2>
          <button @click="addnode">add element</button>
<!--          <h2 ref="myid" draggable="true"  @dragstart="showe" @dragend="showd" :style="styleit" > move me arround</h2>-->


          <v-select
            v-model="select"
            :hint="`${select.state}, ${select.abbr}`"
            :items="items"
            item-text="state"
            item-value="abbr"
            label="Select"
            persistent-hint
            return-object
            single-line
          ></v-select>
          {{select}}
        </v-flex>
        <v-flex  xs10 id="preview">
<!--          <v-layout draggable="true"  @dragstart="showe" @dragend="showd" :style="styleit" ><h1>rowcontainer</h1></v-layout>-->
<!--          <rowcontainer  rmargin="ma-0" rpadding="pa-0"-->
<!--          >-->
<!--            <template v-for="nod in nodes"  v-html="nod.template">-->


<!--            </template>-->



<!--          </rowcontainer>-->

            <div class="">
              <v-layout row wrap>
                <v-flex xs4>
                  <v-card width="auto" height="auto" style="background-color:#F5F5F5;" >
                    <v-layout row wrap width="auto" height="10em" class="" style="background-color: #ffffff;" >
                      <v-flex pt-2 xs12 text-xs-center>
                        <v-avatar
                          size="180px"

                          color="grey lighten-4"
                        >
                          <img width="200" height="200" src="../../static/shiv5.jpg" alt="avatar"/>
                        </v-avatar>
                      </v-flex>

                      <v-flex text-xs-center xs12>
                        <h2 class="black--text">Shivansh Talwar</h2>
                      </v-flex>
                      <v-flex text-xs-center xs12 pb-2>
                        <span class="font-italic white--text">Full-Stack Web Developer</span>
                      </v-flex>


                    </v-layout>


                    <v-layout row wrap width="auto"  class="" style="background-color: #F5F5F5;" >
                      <v-layout mt-4 row wrap>
                        <v-flex v-for="element in leftpannel" :key="element.text" xs12>
                          <v-layout row wrap>

                            <v-flex  xs2>

                              <v-icon class="black--text ml-2" v-html="element.icon" ></v-icon>
                            </v-flex>
                            <v-flex xs10 >
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
                            Developer and bring a lot value to Organisation that i will be working in, going to work in dynamic working environment with challenges to develop myself.
                            From that I will Contribute to development of your Organisation.


                          </p>
                        </v-container>

                      </v-layout>
                      <v-layout row wrap>
                        <v-container>
                          <h2 class="text-xs-left black--text font-weight-bold">INTERPERSONAL SKILLS</h2>

                          <v-layout row wrap>
                            <v-flex  xs12>
                              <ul>
                                <li v-for="element in skills" :key="element.text">
                                  <h4 class="black--text">{{element.text}}</h4>
                                </li>

                              </ul>

                              <!--                   <v-progress-linear-->
                              <!--                     background-color="blue-grey"-->
                              <!--                     color="lime"-->
                              <!--                     :value="element.score"-->
                              <!--                   ></v-progress-linear>-->
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
                          <!--                 <v-flex xs1></v-flex>-->
                          <!--                 <v-flex xs1></v-flex>-->
                          <!--                 <v-flex xs1>-->
                          <div class="circle">
                            <v-icon large  class="large text-xs-center white--text">school</v-icon>
                          </div>
                          <!--                 </v-flex>-->
                          <!--                 <v-flex xs9>-->
                          <h2 class="ml-3 mt-2 font-weight-bold">EDUCATION</h2>

                          <!--                 </v-flex>-->
                        </v-layout>
                        <v-layout row wrap>
                          <v-flex ma-4 xs12>

                            <v-layout row wrap>
                              <v-flex xs9>
                                <h3><b>Greenway Modern School</b></h3>
                              </v-flex>
                              <v-flex xs3>
                                <h3><i>2016</i></h3>
                              </v-flex>
                            </v-layout>

                            <span><i>CBSE Board</i></span><br>
                            <span><i>CGPA/Percentage:</i>76%</span>
                          </v-flex>

                          <v-flex ma-4 xs12>
                            <v-layout row wrap>
                              <v-flex xs9>
                                <h3><b>Abdul Kalam Technical University,Lucknow</b></h3>
                              </v-flex>
                              <v-flex xs3>
                                <h3><i>2016-2020</i></h3>
                              </v-flex>
                            </v-layout>
                            <span><i>B-Tech in Computer Science</i></span><br>
                            <span><i>Percentage:</i>70%</span>
                          </v-flex>


                        </v-layout>


                      </v-container>
                    </v-flex>
                  </v-layout>


                  <v-flex xs12>
                    <v-container>

                      <v-layout row wrap>
                        <!--                 <v-flex xs1></v-flex>-->
                        <!--                 <v-flex xs1></v-flex>-->
                        <!--                 <v-flex xs1>-->
                        <div class="circle">
                          <v-icon large  class="large text-xs-center white--text">insert_chart</v-icon>
                        </div>
                        <!--                 </v-flex>-->
                        <!--                 <v-flex xs9>-->
                        <h2 class="ml-3 mt-2 font-weight-bold">TECHNICAL SKILLS</h2>
                      </v-layout>


                      <v-data-table
                        hide-actions
                        :headers="headers"
                        :items="desserts"
                        class="mt-3 elevation-1"
                      >
                        <template v-slot:items="props">
                          <td class="text-xs-left">{{ props.item.technology }}</td>
                          <!--               <td class="text-xs-left">{{ props.item.experience }}</td>-->
                          <!--               <td class="text-xs-left">-->
                          <!--&lt;!&ndash;                 <v-rating half-increments&ndash;&gt;-->
                          <!--&lt;!&ndash;                                                  :value="props.item.rating" readonly></v-rating>&ndash;&gt;-->
                          <!--                 <v-progress-linear-->
                          <!--                   background-color="blue-grey"-->
                          <!--                   color="lime"-->
                          <!--                   :value="props.item.rating"-->
                          <!--                 ></v-progress-linear>-->
                          <!--               </td>-->
                        </template>
                      </v-data-table>


                    </v-container>


                  </v-flex>



                  <v-flex xs12>
                    <v-container>

                      <v-layout row wrap>
                        <!--                 <v-flex xs1></v-flex>-->
                        <!--                 <v-flex xs1></v-flex>-->
                        <!--                 <v-flex xs1>-->
                        <div class="circle">
                          <v-icon large  class="large text-xs-center white--text">assignment_turned_in</v-icon>
                        </div>
                        <!--                 </v-flex>-->
                        <!--                 <v-flex xs9>-->
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


          <script>

            import axios from 'axios'
            import Vue from 'vue'

            import rowcontainer from '../components/rowcontainer'
            let preview=new Vue({
              el:'#preview',

              loading:false,
              loadingindicator:false,
              // fetch()
              async created() {
// this.$nuxt.loadingIndicator
                console.log(this.$route.path)
                axios.get("https://jsonplaceholder.typicode.com/posts/1").then(res=>{
                  this.skills[0].text= res.data.body
                })
                axios.get("https://jsonplaceholder.typicode.com/posts/1").then((res)=>{
                  console.log(res.data.title)
                  this.settitle(res)


                })
              },
              methods:{
                settitle(response){
                  this.title=response.data.title
                }
              },

              head () {
                return {

                  title:this.title,
                  meta: [
                    { charset: 'utf-8' },
                    { name: 'viewport', content: 'width=device-width, initial-scale=1' },
                    { hid: 'keywords', name: 'keywords', content: 'vuejs, nuxt, javascript, tutorials, development, software' },
                    { hid: 'description', name: 'description', content:"custom description" }
                  ],
                  link: [
                    { rel: 'icon', type: 'image/x-icon', href: '/favicon.ico' },
                    {
                      rel: 'stylesheet',
                      href:
                        'https://fonts.googleapis.com/css?family=Roboto:300,400,500,700|Material+Icons'
                    }
                  ]
                }},
              components: {
              },
              data(){
                return{
                  title:'',

                  projects:[
                    {title:"Proxychecker",
                      description:" High Performant,MultiThreaded, C Based proxy checker Tool which makes validating and checking millions of proxy in almost no time.",
                      url:"https://github.com/shivanshtalwar0/proxychecker"
                    },
                    {title:"Dr. John's Nutrition Health Portal",
                      description:"A Freelance Project Based on Vue.js to help Dr. John Share his Knowledge among his clients ",
                      url:"https://drjohnsnutritionhealthportal.com/login"
                    },
                    {title:"Messenger clone",
                      description:"A  Project Based on Nuxt.js ,having almost all features and functionality of Facebook Messenger",
                      url:"http://messenger-9ea45.firebaseapp.com/signup"
                    },


                  ],
                  leftpannel:[
                    {icon:"calendar_today",text:"6 January 1998"},
                    {icon:"email",text:"shivanshtalwar0@gmail.com"},
                    {icon:"phone",text:"+918744849050"},
                    {icon:"location_on",text:"B-52/A-1,Dilshad Colony,Delhi-95"},



                  ],

                  skills:[
                    {text:"Good analytical and problem solving skills.",score:85},
                    {text:"Good Communication Skills",score:80},

                    {text:"self-confident and hard working nature.",score:80},
                    {text:"Ability to work both independently and as a team player.",score:70},



                  ],


                  headers: [
                    {
                      text: 'Language/Technology/Framework',
                      align: 'left',
                      sortable: false,
                      value: 'name'
                    },

                    // { text: 'Level Of Experience',   align: 'left',
                    //   sortable: false,
                    //   value: 'name'},
                    // { text: 'Rating', align: 'left',
                    //   sortable: false,
                    //   value: 'name'  }
                  ],
                  desserts: [
                    {
                      technology: 'Web Designing & Development',
                      experience:'Expert',
                      rating:99

                    },

                    {
                      technology: 'Vue.js',
                      experience:'Expert',
                      rating:99

                    },

                    {
                      technology: 'Google Firebase',
                      experience:'Intermediate',
                      rating:80

                    },

                    {
                      technology: "Python",
                      experience:'intermediate',
                      rating:90

                    },
                    {
                      technology: 'Mysql',
                      experience:'Intermediate',
                      rating:80

                    },
                    {
                      technology: 'C & C++',
                      experience:'intermediate',
                      rating:85

                    },

                    {
                      technology: 'Java',
                      experience:'Intermediate',
                      rating:75

                    },




                  ]




                }


              }
            })
          </script>
          <style>
            .bg{
              background-image: url("../../assets/professional-background-png-1.png");
              background-position: center;
              background-attachment: fixed;
              background-size:cover ;
              /*background-clip: content-box;*/


            }
            .circle {
              height: 50px;
              width: 50px;
              background-color:black;
              padding-top: 7px;
              padding-left: 7px;
              border-radius: 50%;
              display: inline-block;

            }

          </style>




        </v-flex>

      </v-layout>

    </div>
</template>

<script>
  import vm from '../../plugins/Vuejs'
  import rowcontainer from '../../components/rowcontainer'
  import uuid from 'uuid'
  import vue from 'vue'
  import colcontainer from '../../components/columncontainer'
    export default {
        name: "_id",
      computed:{


          },
      mounted(){
          // console.log(preview.$data)
        // document.getElementById('area').onmousemove= (event)=> {
        //   this.mousex=event.clientX
        //   this.mousey=event.clientX
        // }
      },

      components:{
          rowcontainer,
        colcontainer
      },
      watch:{
        nodes(v){
          console.log(v)
          this.nodes=v

        }
      },
      methods:{

          showe(e){
            this.styleit=`background-color:yellow;height:20em;width: 25em;border: dot-dot-dash 10px blue;`
            console.log(e)
          },
        showd(e){
          this.styleit=`background-color:yellow;height:20em;width: 25em;border: dot-dot-dash 4px blue;position:fixed;top:${e.clientY}px;left:${e.clientX}px`
            console.log(e)
          console.log(this.$refs.myid)


        },
          transpiler(node){
            switch (node.name) {
              case "columncontainer":
                node.template=`<columncontainer :cpadding="${node.padding}" :cmargin="${node.margin}" :arrangement="${node.arrangement}" > hello </columncontainer>`
              break;
              default:
                node.template="fail"
                    break

            }
          },
        addnode(){
            console.log(this.nodes)
            let key=uuid()
          this.nodes[key]={
              key:key,
              name:'columncontainer',
              class:'',
              style:'',
              padding:'ma-0',
              margin:'ma-0',
              arrangement:"7,6,6,6,9",





          }
          this.transpiler(this.nodes[key])
          let obj=this.nodes
          this.nodes={}
          this.nodes=obj








        }
      },

      data(){
          return{
            styleit:'background-color:yellow;height:70px;width: 160px;border: dot-dot-dash 4px blue;',
            mousex:0,
            mousey:0,
            template:"",
            nodes:{},
            select:1,
            items: [
              { state:"1 Column In Row", abbr:1 },
              { state: '2 Column In Row', abbr:2 },
              { state: '3 Column In Row', abbr: 3 },
              { state: '4 Column In Row', abbr: 4 },
              { state: '6 Column In Row', abbr: 6 },
              { state: '12 Column In Row', abbr: 12 }
            ]


          }
      }
    }
</script>

<style scoped>

</style>
