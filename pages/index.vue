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
								Join: <a class="rainbow-text" href="steam://connect/tf2.fluffycat.gay">tf2.fluffycat.gay</a>
								Alt: <a class="rainbow-text" href="steam://connect/tf3.fluffycat.gay">tf3.fluffycat.gay</a>
							</div>
							<div id="rules">
								TINY KITTY GIRL POUND&apos;S REVOLUTIONARY FEATURES INCLUDE:
								<ul>
									<li>The best map pool of all time.</li>
									<li>No random spread</li>
									<li>Crits on</li>
								</ul>
								<b><i><u>18+ ONLY! NO MINORS</u></i></b>
								<br />
								<br />
								Open to girlkissers, estrogen gulpers, tryhards, boywives, furries, women, kitty girls, tf2 players, casuals, puppyboys, and so much more!
								<br />
								<br />
								<img class="icon" src="/img/steam_logo.png" alt="steam logo" /> <b>Steam group:</b> <a class="font-tf2build rainbow-text" href="https://steamgroup.fluffycat.gay">steamgroup.fluffycat.gay</a>
								<br />
								<img class="icon" src="/img/Discord_icon.png" alt="discord logo" /> <b>Discord group:</b> <a class="font-tf2build rainbow-text" href="https://discord.gg/tkgp">discord.gg/tkgp</a>
							</div>
						</div>
						<discord-widget />
					</div>
				</div>
			</div>
			<div class="window grow-in">
				<div class="title-bar">
					<span>
						<img class="icon" src="/img/gametracker.ico" alt="gametracker logo" />
						<span class="title-bar-text">gametracker</span>
					</span>
					<div class="title-bar-controls">
						<button aria-label="Minimize"></button>
						<button aria-label="Maximize"></button>
						<button aria-label="Close"></button>
					</div>
				</div>
				<div class="window-body">
					<gametracker-widget-4 />
				</div>
			</div>
			<div class="window grow-in">
				<div class="title-bar">
					<span>
						<img class="icon" src="/img/battlemetrics.jpg" alt="sick asf kitty" />
						<span class="title-bar-text">battlemetrics</span>
					</span>
					<div class="title-bar-controls">
						<button aria-label="Minimize"></button>
						<button aria-label="Maximize"></button>
						<button aria-label="Close"></button>
					</div>
				</div>
				<div class="window-body">
					<battlemetrics-widget-4 />
				</div>
			</div>
			<div class="window grow-in">
				<div class="title-bar">
					<span>
						<img class="icon" src="/img/gametracker.ico" alt="gametracker logo" />
						<span class="title-bar-text">gametracker</span>
					</span>
					<div class="title-bar-controls">
						<button aria-label="Minimize"></button>
						<button aria-label="Maximize"></button>
						<button aria-label="Close"></button>
					</div>
				</div>
				<div class="window-body">
					<gametracker-widget-5 />
				</div>
			</div>
			<div class="window grow-in">
				<div class="title-bar">
					<span>
						<img class="icon" src="/img/battlemetrics.jpg" alt="sick asf kitty" />
						<span class="title-bar-text">battlemetrics</span>
					</span>
					<div class="title-bar-controls">
						<button aria-label="Minimize"></button>
						<button aria-label="Maximize"></button>
						<button aria-label="Close"></button>
					</div>
				</div>
				<div class="window-body">
					<battlemetrics-widget-5 />
				</div>
			</div>
		</div>
	</div>
</template>

<script setup lang="ts">

import '98.css';

useSeoMeta({
	title: "tiny kitty's girl pound 18+",
	ogTitle: "Tiny Kitty's Girl Pound",
	description: "Official website for the tiny kitty girl pound Team Fortress 2 server: tf2.fluffycat.gay",
	ogDescription: "Official website for the tiny kitty girl pound Team Fortress 2 server: tf2.fluffycat.gay",
	ogImage: "/img/plush_atk.png",
	twitterCard: "summary_large_image",
})

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
	max-width: 600px;
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

	display: flex;
	flex-wrap: wrap;
	justify-content: center;

	.window {
		margin: 2px;
	}
}

.line-break {
	width: 100%;
	border-bottom: 1px solid grey;
	margin: 12px 0;
}

</style>