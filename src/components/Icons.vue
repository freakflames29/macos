<template>
	<div class="dock_icons">
		<img
			:src="imgUrl"
			alt="finder"
		/>
		<!-- <h1 :id="hi">HHHHH</h1> -->
	</div>
</template>

<script>
export default {
	name: "Icons",
	props:{
		imgUrl:String
	}
};
</script>
