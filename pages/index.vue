<template>
	<div class="flex-center">
		<div class="content">
			<div class="flex-center">
				<img src="/img/banner.png" alt="tiny kitty's girl pound banner" style="width: 100%" />
			</div>
			<div class="window grow-in">
				<div class="title-bar">
					<span>
						<img class="icon" src="/img/plush_def.png" alt="sick asf kitty" />
						<span class="title-bar-text">tiny kitty's introduction</span>
					</span>
					<div class="title-bar-controls">
						<button aria-label="Minimize"></button>
						<button aria-label="Maximize"></button>
						<button aria-label="Close"></button>
					</div>
				</div>
				<div class="window-body">
					<div class="body-header">
						<div id="intro">
							<span id="welcome" class="font-tf2build">haiiiii ^_^ hi!! hiiiiii &lt;3 haiiiiii hii :3 </span>
							<div id="join" class="font-tf2build">
								Join: <a class="rainbow-text" href="steam://connect/tf2.fluffycat.gay:19990">tf2.fluffycat.gay:19990</a>
							</div>
							<div id="rules">
								TINY KITTY GIRL POUND&apos;S REVOLUTIONARY FEATURES INCLUDE:
								<ul>
									<li>The best map pool of all time.</li>
									<li>No random spread</li>
									<li>Crits on</li>
								</ul>
								Open to girlkissers, estrogen gulpers, tryhards, boywives, furries, women, kitty girls, tf2 players, casuals, puppyboys, and so much more!
							</div>
									
						</div>
						<discord-widget />
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script setup lang="ts">

import '98.css';

</script>

<style lang="scss">

#welcome {
	font-size: 24pt;
	font-family: 'tf2build'
}

#join {
	text-align: center;
	width: 100%;
	font-size: 18pt;
	font-family: 'tf2build';
	margin-bottom: 12px;
}

#intro {
	width: 600px;
}

#rules {
	font-size: 14pt;
	font-family: 'tf2';
}

.flex-center {
	display: flex;
	justify-content: center;
}

.body-header {
	display: flex;
	align-items: flex-start;
	justify-content: space-around;
	flex-wrap: wrap;
}

.content {
	width: 100%;
	max-width: 1000px;
}

</style>