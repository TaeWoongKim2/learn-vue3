<template>
	<div class="card">
		<div class="card-body">
			<h5 class="card-title red">
				{{ title }}
			</h5>
			<p class="card-text">
				{{ contents }}
			</p>
			<a href="#" class="btn btn-primary">Read more</a>
		</div>
	</div>
</template>

<script>
import { ref, useCssModule } from 'vue';

export default {
	props: {
		title: String,
		contents: String,
	},
	setup() {
		return {};
	},
};
</script>

<style scoped>
.red {
	color: v-bind(color) !important;
}
</style>
<!-- <style module="classes">
.red {
	color: red !important;
}
</style> -->
<!-- <style scoped>
.red {
	color: red !important;
}
</style> -->
