<template>
	<div class="root_container">
		<div class="root">
			<Nav />
			<span v-if="terminal">
				<Terminal />
			</span>
			<div class="dock_container">
				<div class="dock">
					<div class="dock_left">
						<Icons
							v-for="j in js"
							:imgUrl="j.link"
							@fun="callme($event)"
							:name="j.name"
						/>
					</div>
					<div class="dock_right"></div>
				</div>
			</div>
		</div>
	</div>
</template>
<script>
import json from "./components/test.json";
import Nav from "./components/Nav.vue";
import Icons from "./components/Icons.vue";
import Terminal from "./components/Terminal.vue";
export default {
	name: "Root",
	data() {
		return {
			js: json,
			num: 5,
			terminal: false,
		};
	},
	components: {
		Nav,
		Icons,
		Terminal,
	},
	methods: {
		callme(value) {
			this.terminal = value;
			console.log(value);
		},
	},
};
</script>
