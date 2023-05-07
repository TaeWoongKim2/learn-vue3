<template>
	<AppReactive></AppReactive>
	<AppRef></AppRef>
	<AppRefObjectArray></AppRefObjectArray>
	<AppToRefsToRef></AppToRefsToRef>
	<AppReadonly></AppReadonly>
</template>

<script>
import AppReactive from './lectures/7/App_reactive.vue';
import AppRef from './lectures/7/App_ref.vue';
import AppRefObjectArray from './lectures/7/App_ref_object_array.vue';
import AppToRefsToRef from './lectures/7/App_toRefs_toRef.vue';
import AppReadonly from './lectures/7/App_readonly.vue';

export default {
	components: {
		AppReactive,
		AppRef,
		AppRefObjectArray,
		AppToRefsToRef,
		AppReadonly,
	},
	setup() {
		return {};
	},
};
</script>

<style lang="scss" scoped></style>
