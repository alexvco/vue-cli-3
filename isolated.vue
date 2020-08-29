<template>
	<div id="only-one-main-element">
		<h1>This file could be served independantly to prototype using: vue serve isolated.vue</h1>
		<p>Note that you need to be using vue-cli-3 and have: npm install -g @vue/cli-service-global</p>
		<p>Also note that since this file is in a directory which has a package.json file it will not work, it needs to be completely isolated</p>

		<div v-if="online">
			<p>A staff member is currently online</p>
		</div>
		<div v-if="!online">
			<p>A staff member is not currently online</p>
		</div>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				online: false
			}
		}
	}
</script>
