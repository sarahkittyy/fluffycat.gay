<template>
	<div class="icon" :style="style"></div>
</template>

<script lang="ts">

export default defineComponent({
	props: {
		size: { type: Number, default: 16 },
		src: String,
		alt: { type: String, required: false },
	},
	computed: {
		style() {
			return `
				width: ${this.size}px;
				height: ${this.size}px;
				line-height: ${this.size}px;
				background-image: url("${this.src}");
				background-size: ${this.size}px
			`;
		}
	}
});

</script>

<style lang="scss" scoped>

.icon {
	vertical-align: middle;
	display: inline-block;
}

</style>