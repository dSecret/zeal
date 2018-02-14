<template>
<v-app style="background-color:lightgrey;">
    <div class="upperDiv">
      <img src="/src/assets/zeal.jpg"/>
    </div>
    <div class="lowerDiv">
            <v-card color="blue-grey darken-2 mb-2" class="white--text" flat>
              <v-card-title primary-title>
                <span class="display-1">Events</span><br>
                
              </v-card-title>
              <v-card-text>
                <span class="heading">
                      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Harum maiores modi quidem veniam, expedita quis laboriosam, ullam facere adipisci, iusto, voluptate sapiente corrupti asperiores rem nemo numquam fuga ab at.
                </span><br>
                <span class="mt-3 d-block subheading">
                    Checkout Live updates!!
                </span>
              </v-card-text>
              <v-card-actions class="mt-0">
                <v-btn flat dark outline to="/">Home</v-btn>
                <v-btn flat dark outline to='/timeline'>Timeline</v-btn>
              </v-card-actions>
            </v-card>
            <v-container grid-list-md>
              <v-layout row wrap>
                <v-flex xs12 md6 v-for="i in 10" :key="i">
                <v-card class=" mr-1 ml-1" >
                  <v-card-media
                    class="white--text"
                    height="200px"
                    src="/src/assets/zeal.jpg"
                  >
                    <v-container class="d-block pr-0 pl-0 pt-0 "fill-height fluid 
                                  style="display:block;"
                    >
                          <div  style="background-color:rgba(0,0,0,0.5);width:100%;"
                                class="headline pl-3 pt-3 pb-3"
                          >Cricket<br>
                            <span class="subheading grey--text">
                              Are you ready to switch your Game mode!!
                            </span>
                          </div>
                    </v-container>
                    <!-- <div>Class</div> -->
                  </v-card-media>
                  <v-card-actions>
                      <v-btn flat>Explore</v-btn>
                  </v-card-actions>
                </v-card>
                </v-flex>
              </v-layout>
            </v-container>
    </div>
</v-app>
</template>
<style>
  .card--flex-toolbar {
    margin-top: -64px;
  }
  .upperDiv{
      width:100vw;
      background-color:grey;
      height:50vh;
      overflow: hidden;
  }
  .lowerDiv{
      width:70vw;
      margin:0 auto;
      background-color:white;
      margin-top:-28vh;
      margin-bottom:15vh;
      padding-bottom:20px;
      /*height:200vh;*/
  }
  .upperDiv img{
    width:100%;
  }
@media only screen and (max-width:8in){
  .lowerDiv{
    width:96vw;
  }
}
</style>