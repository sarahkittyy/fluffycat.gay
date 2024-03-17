<template>
	<div id="content">
		<div id="header">
			<div id="header-text">
				<div class="rainbow-text h1">Help fund TKGP!! <icon :size="40" src="/img/plush_def.png"/></div>
				<div class="h2">Will purr for funds <icon :size="32" src="/img/plush_atk.png" /></div>
			</div>
			<a href="/donate" ><img src="/img/bigpaws.gif" /></a>
		</div>
		<div id="links">
			<paypal-donate />
			<nfoservers-donate />
			<trade-donate />
			<span class="line-break" />
			<cashapp-donate />
			<discord-donate />
		</div>
	</div>
</template>

<style lang="scss" scoped>

#links {
	display: flex;
	justify-content: center;
	align-items: center;
	flex-wrap: wrap;
	
	width: 90%;
}

.line-break {
	flex-basis: 100%;
}

#content {
	display: flex;
	justify-content: center;
	flex-wrap: wrap;
}

.h1 {
	font-size: 30pt;
}

.h2 {
	font-size: 22pt;
}

#header {
	display: flex;
	justify-content: center;
	flex-wrap: wrap;
	font-family: 'tf2build';
	align-items: center;
	width: 100%;

	img {
		max-height: 80px;
	}

	div {
		text-align: center;
	}

	#header-text {
		width: auto;
		flex-basis: auto;
	}
}

</style>