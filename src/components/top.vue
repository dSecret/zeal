<template>
	<div class="top">          
		<v-avatar
              :size="logoSize1"
              class="white lighten-5 mr-3"
        >
              <img src="/src/assets/logo.png" alt="avatar">
       </v-avatar>
		<v-avatar
              :size="logoSize2"
              class="grey lighten-5"
        >
              <img src="/src/assets/logo.png" alt="avatar">
       </v-avatar>
   </div>
</template>

<script>
  export default {
    data(){
      return{
      	logoSize1:"100px",
      	logoSize2:"80px"
      }
    },
    computed:{
    	rightHeight:function(){
    		return window.innerHeight-180
    	}
    }
  }
</script>
<style type="text/css" scoped>
 .top{
	height:180px;
	width:100%;
	display: flex;
	justify-content:center;
	align-items: center;
	background-color:blue;
}
.comEc{
  box-sizing: border-box;
  -moz-box-sizing: border-box;
}

</style>