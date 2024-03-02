<template>
	<a id="button" href="https://discord.com/channels/1156134211581906964/shop/1171187301234258042">
		<span>Suppawter discord role <icon :size="24" src="/img/plush_def.png" /></span>
		<img src="/img/suppawter.png" alt="discord suppawter role" />
	</a>

</template>

<style lang="scss" scoped>

#button {
	outline: none;
	min-width: 200px;
	max-width: 400px;
	
	text-align: center;
	text-decoration: none;
	color: black;

	&:hover {
		text-decoration: underline;
		color: blue;
	}

	img {
		width: 100%;
		border: 1px solid #333;
		box-sizing: border-box;
		border-radius: 10px;
	}

	span {
		font-family: 'tf2';
		font-size: 14pt;
	}
}

</style>
