<template>
	<nav class="menu-bar">
		<template v-for="link in links">
			<a v-if="link.link != undefined" :href="link.link"><icon :size="32" :src="link.icon" />{{ link.name }}</a>
			<button v-else @click="$emit('select', link.name);" :active="link.name == selected"><icon :size="32" :src="link.icon" />{{ link.name }}</button>
		</template>
	</nav>
</template>
<script setup lang="ts">

interface Props {
	selected?: string
}

const props = withDefaults(defineProps<Props>(), {
	selected: 'Home',
});

const emits = defineEmits<{
	select: [value: string]
}>();

const links = [
	{
		name: 'Home',
		icon: '/img/plush_atk.png',
	},
	{
		name: 'Stats',
		icon: '/img/battlemetrics.jpg',
	},
	{
		name: 'Donate',
		icon: '/img/revolving-hearts-emoji.png',
	},
	{
		name: 'Discord',
		icon: '/img/Discord_icon.png',
		link: 'https://discord.gg/tkgp'
	},
	{
		name: 'Steam',
		icon: '/img/steam_logo.png',
		link: 'https://steamcommunity.com/groups/tinykittygirlpound'
	},
	{
		name: 'Sourcebans',
		icon: '/img/necro_smasher.png',
		link: 'https://sourcebans.fluffycat.gay'
	}
];

</script>
<style lang="scss" scoped>

.menu-bar {
	width: 100%;
	display: flex;
	justify-content: space-evenly;
	flex-wrap: wrap;

	button, a {
		display: flex;
		align-items: center;

		* {
			margin: 5px;
		}

		font-size: 32pt;
		font-family: 'tf2build';

		color: black;
		text-decoration: none;
		outline: none;
		border: none;
		box-shadow: none;

		&:hover {
			color: blue;
		}

		&:active {
			outline: none;
			box-shadow: none;
			text-shadow: none;

			color: green;
		}

	}
}

</style>