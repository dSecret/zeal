<template>
<v-app light v-scroll="onScroll">
    <v-toolbar class="white" v-if="check2" fixed style="z-index:2000;"  height="60px" >
      <v-toolbar-items style="margin:0;padding:0;">
              <v-btn   flat style="height:100%;margin:0 0 0 0;padding:0;width:10px;" to='/'exact >
                <v-icon color="teal" style="margin:0 0 0 0;padding:0">home</v-icon>
              </v-btn>
              <v-btn   flat style="height:100%;margin:0;padding:0"to='/events'>
                <v-icon color="teal" style="margin:0 0 0 0;padding:0" >event</v-icon>
              </v-btn>
              <v-btn   flat style="height:100%;margin:0;padding:0"to='/timeline'>
                <v-icon color="teal" style="margin:0 0 0 0;padding:0" >timeline</v-icon>
              </v-btn>
      </v-toolbar-items>  
      <v-spacer></v-spacer>    
      <v-btn icon @click="check2=!check2">
        <v-icon>clear</v-icon>
      </v-btn>
    </v-toolbar>
    <v-toolbar class="transparent" v-if="check" flat fixed  height="60px">
      <!-- <v-toolbar-title v-text="title"></v-toolbar-title> -->
      <v-avatar
        :tile="false"
        size="15"
        class="black lighten-10"
      >
        <img src="/src/assets/nitdd.png" alt="avatar" style="height:50px;">
      </v-avatar>
      <v-spacer></v-spacer>
      <v-btn icon @click="check2=!check2">
        <v-icon>menu</v-icon>
      </v-btn>
    </v-toolbar>
    <router-view></router-view>
</v-app>
</template>

<script>
  export default {
    data(){
      return{
        title:'Zeal 2k18',
        check:false,
        check2:false,
        route:this.$route.path,
        backgroundHeight:window.innerHeight
      }
    },
    computed:{
       handleToolbar:function(){
           let foo=this.route;
           this.onScroll()
           return 'Zeal'
       }
    },
    methods: {
      onScroll (e) {
        this.offsetTop = window.pageYOffset || document.documentElement.scrollTop
        let path=this.$route.path
          if(path=='/'){
              if(this.offsetTop>window.innerHeight){
                return this.check=true;
              }
              else 
                return this.check=false
          }
          else{
             return this.check=true;
          }
      },

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