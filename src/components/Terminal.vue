<template>
	<div class="terminal_container">
		<div class="terminal">
			<div class="terminal_bar">
				<span class="headlight red"
					><i class="fa-solid fa-circle"></i
				></span>
				<span class="headlight yellow"
					><i class="fa-solid fa-circle"></i
				></span>
				<span class="headlight green"
					><i class="fa-solid fa-circle"></i
				></span>
				<p class="terminal_title bold">sourav--Zsh-- 80x24</p>
			</div>
			<div class="terminal_body">
				<p class="bold">Sourav@macmini ~ %</p>
			</div>
		</div>
	</div>
</template>
<script>
export default {
	name: "Terminal",
};
</script>
<style type="text/css">
.terminal_body {
	padding-top: 10px;
}
</style>
