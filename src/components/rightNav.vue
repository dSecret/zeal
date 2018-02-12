<template>
<div class="comEc" id="#leftNav">
	<div class="top"></div>
	<div class="right"></div>
</div>
</template>

<script>
  export default {
    data(){
      return{
      }
    },
  }
</script>
<style type="text/css">
#leftNav{
  width:100%;
  height:100vh;
  z-index:100;
  /*overflow: hidden;*/
  background-color: pink;
}
#leftNav .top{
	height:25vh;
	width:100%;
	background-color:blue;
}
#leftNav .right{
	height:75vh;
	width:100%;
	background-color:white;
}
.comEc{
  box-sizing: border-box;
  -moz-box-sizing: border-box;
}
</style>