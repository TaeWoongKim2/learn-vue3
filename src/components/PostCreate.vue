<template>
	<div>
		<input type="text" v-model="title" name="title" id="titleInput" />

		<!-- <button class="btn btn-primary" @click="$emit('createPost')">button</button> -->
		<button class="btn btn-primary" @click="createPost">button</button>
	</div>
</template>

<script>
import { ref } from 'vue';

export default {
	emits: {
		// createPost: null,
		createPost: newTitle => {
			if (!newTitle) {
				alert('제목을 입력해주세요');
				return false;
			}
			return true;
		},
	},
	setup(_, { emit }) {
		const title = ref('');

		const createPost = () => {
			emit('createPost', title.value);
		};

		return { title, createPost };
	},
};
</script>

<style lang="scss" scoped></style>
