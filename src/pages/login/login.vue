<template>
  <v-app class="d-flex">
      <v-layout justify-center align-center>
        <div class="loginform">
            <v-form  class="elevation-4 pl-4 pr-4 pt-4 pb-4" >
              <v-text-field
                label="Username"
                v-model="user.uname"
                required
              ></v-text-field>
              <v-text-field
                label="Password"
                v-model="user.psw"
                required
              ></v-text-field>
               <v-btn color="primary "  v-on:click="login">Primary</v-btn>
              <!-- {{post}} -->
            </v-form>
            {{status}}
        </div>
      </v-layout>
  </v-app>
</template>
<script>

export default {
    data () {
      return {
        user:{
          uname:'admin',
          psw:'root'
        },
        status:{}
      }
    },
    methods:{
      login:function(){
     
      }
    },
    created(){
      // console.log("enter")
          // axios.post('http://localhost:8000/login',this.user).then((response)=>{
          //     console.log(response.data,"working")
          //     // this.post=response.data
          // })
          // this.login()
    }
  }
</script>
<style>

</style>