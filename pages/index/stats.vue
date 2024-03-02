<template>
	<div class="stats-links">
		<h1 class="subheader">
			<div id="nyan-cat" />
			View kills, deaths, and other stats:
		</h1>
		<a class="statcat" href="http://stats4.fluffycat.gay">tkgp4<img src="/img/plush_def.png" alt="tkgp4's stats" /></a>
		<a class="statcat" href="http://stats5.fluffycat.gay"><img src="/img/plush_atk.png" alt="tkgp5's stats" />tkgp5</a>
	</div>
	<div class="line-break"></div>
	<div class="bm-container">
		<h1 class="subheader">Activity stats</h1>
		<battlemetrics-widget-4 />
		<battlemetrics-widget-5 />
	</div>
	<div class="gt-container">
		<gametracker-widget-4 />
		<gametracker-widget-5 />
	</div>
</template>
<style lang="scss" scoped>

.statcat {
	display: flex;
	align-items: center;
	font-size: 22pt;
	font-family: 'tf2build';
	outline: none;
}

.subheader {
	width: 100%;
	text-align: center;
	font-size: 22pt;
	font-family: 'tf2build';
	flex-basis: 100%;

	display: flex;
	align-items: center;
	justify-content: center;
	height: 60px;

	#nyan-cat {
		background-image: url('/img/cat-nyan-cat.gif');
		background-size: contain;
		background-repeat: no-repeat;
		flex-shrink: 0;
		height: 64px;
		width: 64px;
	}
}

.line-break {
	width: 100%;
	border-bottom: 1px solid grey;
	margin: 12px 0;
}

.stats-links {
	display: flex;
	flex-wrap: wrap;
	justify-content: center;
	align-items: center;
}

.bm-container, .gt-container {
	display: flex;
	justify-content: center;
	align-items: center;
	flex-wrap: wrap;
}

</style>