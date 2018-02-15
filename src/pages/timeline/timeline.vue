<template>
	<v-app id="timelineWrap">
		<div id="timeline">
			<v-card v-for="i in 10" :key="i" class="mb-3">
			    <v-card-title primary-title>
			      <div>
			        <span class="headline mb-0">Cricket</span>
			        <span class="mb-0 ml-2 grey--text">12:00PM 15/2/2018</span>
			        <span class="subheading mb-0 ml-2">Live</span>
			      </div>
			    </v-card-title>
			    <v-card-text>
 					<div>
 						<div class="mb-2" align="center">
 								<span class="mr-3 title">CSE</span>
 								<span class="grey--text">vs</span>
 								<span class="ml-3 title">ECE</span>
 						</div>
 						<div class="mt-3">
 							<span class="subheading mr-2 mt-3">Venue:</span>
 							<span>FootBall Ground, NITD</span><br>
 							<span class="subheading mr-2 mt-3">Timing:</span>
 							<span>11PM | 12 Aug'18 Onwards</span>
 						</div>
 					</div>
			    </v-card-text>
		  	</v-card>
		</div>
	</v-app>
</template>
<style scoped>
#timelineWrap{
	background-color: #08AEEA !important;
background-image: linear-gradient(0deg, #08AEEA 0%, #2AF598 100%) !important;
}
#timeline{
	width:40vw;
	margin:0 auto;
	margin-top:10vh;
	margin-bottom:15vh;
}
@media only screen and (max-width:8in){
	#timeline{
		width:97vw;
	}
}
</style>