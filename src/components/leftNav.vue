<template>
<div class="comEc" id="leftNav">
	<top></top>
	<bottom></bottom>
</div>
</template>

<script>
import top from './top.vue'
import bottom from './bottom.vue'
export default {
	data(){
	  return{
	  	
	  }
	},
	components:{
		top,
		bottom
	},
	computed:{
		
	}
}
</script>
<style type="text/css">
#leftNav{
  width:100%;
  height:100vh;
  z-index:100;
  overflow: hidden;
}
.comEc{
  box-sizing: border-box;
  -moz-box-sizing: border-box;
}

</style>