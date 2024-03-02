<template>
	<div id="content">
		<div id="header">
			<span class="rainbow-text h1">Help fund TKGP!! <icon :size="40" src="/img/plush_def.png"/></span>
			<span class="h2">Will purr for funds <icon :size="32" src="/img/plush_atk.png" /></span>
		</div>
		<div id="links">
			<paypal-donate />
			<nfoservers-donate />
			<trade-donate />
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
	width: 100%;

	span {
		width: 100%;
		text-align: center;
	}
}

</style>