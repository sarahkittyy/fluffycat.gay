<template>
	<div class="flex-center">
		<div class="content">
			<!-- header -->
			<div class="flex-center">
				<img src="/img/banner.png" alt="tiny kitty's girl pound banner" style="width: 100%" />
			</div>
			<!-- main window -->
			<div class="window grow-in" style="width: 100%">
				<!-- title bar -->
				<div class="title-bar">
					<span>
						<icon src="/img/plush_def.png" alt="cute little plush kitty icon" />
						<span class="title-bar-text">tiny kitty's girl page</span>
					</span>
					<div class="title-bar-controls">
						<button aria-label="Minimize"></button>
						<button aria-label="Maximize"></button>
						<button aria-label="Close"></button>
					</div>
				</div>
				<!-- homepage body -->
				<div class="window-body">
					<!-- menu -->
					<menu-bar :selected="subpage" @select="onMenuSelect" />
					<div class="line-break" />
					<NuxtPage />
				</div>
			</div>
		</div>
	</div>
</template>

<script setup lang="ts">

import '98.css';

useHead({
	script: [{
		src: "/js/oneko.js",
		defer: true
	}]
})

useSeoMeta({
	title: "tiny kitty's girl pound 18+",
	ogTitle: "Tiny Kitty's Girl Pound",
	description: "Official website for the tiny kitty girl pound Team Fortress 2 server: tf2.fluffycat.gay",
	ogDescription: "Official website for the tiny kitty girl pound Team Fortress 2 server: tf2.fluffycat.gay",
	ogImage: "/img/plush_atk_big.png",
	articleTag: ['tkgp', 'tf2', 'furry'],
	twitterCard: "summary_large_image",
})

const subpage = ref('Home');
const paths: Record<string, string> = {
	'Home': '/',
	'Stats': '/stats',
	'Donate': '/donate',
};

function onMenuSelect(page: string) {
	subpage.value = page;
	return navigateTo({
		path: paths[page],
	});
}

</script>

<style lang="scss" scoped>

.flex-center {
	display: flex;
	justify-content: center;
}

.window-body {
	min-height: 800px;
}

.content {
	width: 100%;
	margin: 0 10%;

	display: flex;
	flex-wrap: wrap;
	justify-content: center;

	.window {
		margin: 2px;
	}
}

@media (max-width: $desktop-width) {
	.content {
		margin: 0 0;
	}
}

.line-break {
	width: 100%;
	border-bottom: 1px solid grey;
	margin: 12px 0;
}

</style>