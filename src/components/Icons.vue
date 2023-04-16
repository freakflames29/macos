<template>
	<div class="dock_icons">
		<img :src="imgUrl" alt="finder" @click="runme" :title="name" />
		<!-- <h1 :id="hi">HHHHH</h1> -->
	</div>
</template>

<script>
export default {
	name: "Icons",
	props: {
		imgUrl: String,
		name: String,
	},
	data() {
		return {
			terminal: false,
			// name: name,
		};
	},
	methods: {
		runme() {
			this.terminal = !this.terminal;
			this.$emit("fun", this.terminal);
		},
	},
};
</script>
