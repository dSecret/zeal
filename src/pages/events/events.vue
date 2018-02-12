<template>
  <div class="Events comEc">
    <div class="comEc left" style="background-color:yellow;"><leftNav></leftNav></div>
    <div class="comEc right" style="background-color:red;"><div>ss</div></div>
  </div>
</template>

<script>
import leftNav from '../../components/leftNav.vue'
  export default {
    data(){
      return{
      
      }
    },
    components:{
      "leftNav":leftNav
    }
  }
</script>
<style type="text/css" scoped>
.Events{
  width:100vw;
  height:100vh;
  z-index:100;
  display: flex;
  justify-content: center;
  overflow: hidden;
}
.Events .left{
  width:35vw;
  height:100vh;
  overflow: hidden;
}
.Events .right{
  width:65vw;
  height:100vh;
  overflow-y: scroll;
}
.comEc{
  box-sizing: border-box;
  -moz-box-sizing: border-box;
}
@media only screen and (max-width:7in){
  .Events .left{
    width: 0;
  }
  .Events .right{
    width:100vw;
  }
}
</style>