<template>
	<div class="right" :style="{height:rightHeight+'px'}">
		<router-link class="main" 
					v-for="i in options"
					:key="i.tit"
					tag="div"
					to="/"
		>
			<div class="main-title">{{i.tit}}</div>
			<div class="main-options"
				 v-for="k in i.options"
				 :key="k.tit"
			>
				<div class="main-options-title">{{k.tit}}</div>
			</div>
	</router-link>
	</div>
</template>

<script>
  export default {
    data(){
      return{
      	options:[
      		{tit:"HOME",options:[]},
      		{tit:"TIMELINE",options:[{tit:"Live"},{tit:"Recents"}]},
      		{tit:"EVENTS",options:[]}
      	]
      }
    },
    components:{
    },
    computed:{
    	rightHeight:function(){
    		return window.innerHeight-180
    	}
    }
  }
</script>
<style type="text/css" scoped>
#leftNav .right{
	width:100%;
	background-color:white;
	overflow-y: scroll;
}
.comEc{
  box-sizing: border-box;
  -moz-box-sizing: border-box;
}
#leftNav div{
	width:100%;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
}
.main{
	margin:15px 15px;
}
.main-title{
	text-align:center;
	font-family: "Roboto",sans-serif;
	font-size:30px;
}
.main-options-title{
	text-align:left;
	padding-left:50%;
}
</style>