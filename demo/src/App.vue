<template>
	<div id="app">
		<div>
			<skycon :condition="weather" width="40" height="40"></skycon>
			<skycon condition="clear-day" width="40" height="40"></skycon>
			<skycon condition="clear-night" width="40" height="40"></skycon>
			<skycon
				condition="partly-cloudy-day"
				width="40"
				height="40"
			></skycon>
			<skycon
				condition="partly-cloudy-night"
				width="40"
				height="40"
			></skycon>
			<skycon condition="cloudy" width="40" height="40"></skycon>
			<skycon condition="rain" width="40" height="40"></skycon>
			<skycon condition="sleet" width="40" height="40"></skycon>
			<skycon condition="snow" width="40" height="40"></skycon>
			<skycon condition="wind" width="40" height="40"></skycon>
			<skycon condition="fog" width="40" height="40"></skycon>
		</div>
	</div>
</template>

<script>
export default {
	name: "App",
	data() {
		return {
			weather: "",
		};
	},
	mounted() {
		this.weather = "rain";
	},
};
</script>

<style>
</style>
