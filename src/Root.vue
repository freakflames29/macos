<template>
	<div class="root_container">
		<div class="root">
			<Nav />

			<div class="dock_container">
				<div class="dock">
					<div class="dock_left">
						<Icons v-for="j in js"
							:imgUrl="j.link"
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
export default {
	name: "Root",
	data() {
		return {
			js: json,
			num: 5,
		};
	},
	components: {
		Nav,
		Icons,
	},
};
</script>
