<template>
	<div>
		<TheNav></TheNav>
		<TheView></TheView>
		{{ count }}
	</div>
</template>

<script>
import TheNav from './components/TheNav.vue';
import TheView from './components/TheView.vue';

export default {
	components: {
		TheNav,
		TheView,
	},
	setup() {},
};
</script>

<style lang="scss" scoped></style>
