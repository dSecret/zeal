<template>
    <v-content>
      <section >
        <v-parallax src="/src/assets/hero.jpeg" :height="backgroundHeight">
          <v-layout
            column
            align-center
            justify-center
            class="white--text"
          >
            <img src="/src/assets/vuetify.png" alt="Vuetify.js" height="200">
            <h1 class="white--text mb-2 display-1 text-xs-center">Zeal '18</h1>
            <div class="subheading mb-3 text-xs-center">Annual Sports Fest of NITDelhi</div>
            <v-btn
              class="blue lighten-2 mt-2"
              dark
              large
              outline
              to="/events"
            >
              Events
            </v-btn>
          </v-layout>
        </v-parallax>
      </section>
      <section >
        <v-layout
          column
          wrap
          class="my-5"
          align-left
        >
          <v-flex xs12 >
            <v-container grid-list-xl>
              <v-layout row wrap align-center>
                <v-flex xs12 md12 >
                  <v-card class="elevation-0 transparent">
                    <v-card-title primary-title class="layout justify-left">
                      <div class="headline">About</div>
                    </v-card-title>
                    <v-card-text class="subheading justify-left layout">
                      Annual Sports Fest of  National Institute of Technology,New Delhi.
                      Every year SAC organizes this fest with help of Sports Club. 
                    </v-card-text>
                    <v-card-text>
                      <div class="layout justify-left" >
                          <v-btn outline color="teal" to="/events">Events</v-btn>
                          <v-btn outline color="teal" to="/timeline">Timeline</v-btn>
                          <div style="display:block;height:100px;width:100%;"></div>
                      </div> 
                    </v-card-text>
                  </v-card>
                </v-flex>
              </v-layout>
            </v-container>
          </v-flex>
        </v-layout>
      </section>
      <section style="background-color:lightgrey;">
        <v-layout
          column
          wrap
          class="my-5"
          align-left
        >
          <v-flex xs12>
            <v-container grid-list-xl>
              <v-layout row wrap align-center>
                <v-flex xs12 md5>
                  <v-card class="elevation-0 transparent">
                    <v-card-title primary-title class="layout justify-left">
                      <div class="headline">Address</div>
                    </v-card-title>
                    <v-card-text class="layout justify-left">
                      Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. 
                      Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. 
                      Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti. 
                    </v-card-text>
                  </v-card>
                </v-flex>
                <v-flex xs12 md5>
                  <v-card class="elevation-0 transparent">
                    <v-card-title primary-title class="layout justify-left">
                      <div class="headline text-xs-center">Contacts</div>
                    </v-card-title>
                    <v-card-text class="layout justify-left">
                      Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. 
                      Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. 
                      Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti. 
                    </v-card-text>
                  </v-card>
                </v-flex>
              </v-layout>
            </v-container>
          </v-flex>
        </v-layout>
      </section>
    </v-content>
</template>

<script>
  export default {
    data(){
      return{
        title:'Zeal 2k18',
        check:false,
        check2:false,
        backgroundHeight:window.innerHeight
      }
    },
    methods: {

    },
    toggle:function(){
      console.log("working")
          return this.check2=true
    }
  }
</script>
<style type="text/css">
  #Home{
    /*width:100vw !important;*/
    /*height:10vh !important;*/
    /*overflow:auto !important;*/
  }
</style>