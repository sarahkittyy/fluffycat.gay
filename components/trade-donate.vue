<template>
	<a
		id="container"
		href="https://steamcommunity.com/tradeoffer/new/?partner=125818436&token=cWUGAtJx"
	>
		<span>🔫 Donate via Steam Trade ⚒️</span>
		<div id="button" @click="">
			<div class="cap left" />
			<div class="cap right" />
			<div class="text">Send a Trade Offer</div>
		</div>
	</a>
</template>

<script setup lang="ts">

</script>

<style lang="scss" scoped>

#container {
	display: flex;
	flex-direction: column;
	text-align: center;
	cursor: pointer;

	color: black;
	text-decoration: none;
	outline: none;

	&:hover span {
		color: blue;
		text-decoration: underline;
	}

	span {
		font-family: 'tf2';
		font-size: 14pt;
	} 
}

#button {
	display: inline-block;
	position: relative;
	
	font-family: "Motiva Sans",sans-serif;
	color: #fff;

	background-image: url('/img/steam_trade_bigbutton.png');
	background-position: 0 -100px;
	background-repeat: repeat-x;
	
	padding: 0 50px;
	margin: 0 0 5px 0;
	
	height: 50px;
	line-height: 50px;

	max-width: 248px;
}

.text {
	line-height: 50px;
	font-size: 24px;
}

.cap {
	background-image: url('/img/steam_trade_bigbutton.png');
	
	position: absolute;
	width: 5px;
	height: 50px;
	top: 0;
	background-repeat: no-repeat;

	&.left {
		background-position: -10px 0;
		left: 0;
	}

	&.right {
		right: 0;
		background-position: -15px 0;
	}
}

</style>