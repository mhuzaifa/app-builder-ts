<template>
	<div id="app">
		<TopBar />
		<Navigation />
		<div class="main">
			<AppWrapper />
		</div>
	</div>
</template>

<script lang="ts">
import Vue from 'vue';

import TopBar from '@/components/TopBar.vue';
import Navigation from '@/components/Navigation.vue';
import AppWrapper from '@/components/AppWrapper.vue';

export default Vue.extend({
	name: 'home',
	components: {
		TopBar,
		Navigation,
		AppWrapper
	},
	created () {
		document.title = "Fidelidade App Builder";
	}
});

</script>

<style lang="scss">

#app {
	display: flex;
	flex-direction: column;
	min-height: 100%;

	.main {
		min-height: 100%;
		display: flex;
		flex-direction: row;
	}
}

</style>
