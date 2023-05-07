<template>
	<ClassBinding></ClassBinding>
	<br />
	<hr />
	<br />
	<StyleBinding></StyleBinding>
</template>

<script>
import ClassBinding from './lectures/9/App_class_binding.vue';
import StyleBinding from './lectures/9/App_style_binding.vue';

export default {
	components: {
		ClassBinding,
		StyleBinding,
	},
	setup() {
		return {};
	},
};
</script>

<style lang="scss" scoped></style>
