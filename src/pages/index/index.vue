<template>
	<view class="content">

		<ClockWeather />

	</view>
</template>
 
<script>

	import ClockWeather from '../ClockWeather/ClockWeather.vue';
	export default {

		components:{
			ClockWeather
		},
		data() {
			
			return {
				
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
.content{
	margin-top: 50vw;
	display: flex;
	justify-content: center;
	align-items: center;
}
</style>
