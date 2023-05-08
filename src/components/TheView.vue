<template>
	<main>
		<div class="container py-4">
			<div class="row g-3">
				<div
					class="col col-4"
					v-for="(card, index) in cards"
					:key="`${index}-${card.title}`"
				>
					<AppCard :title="card.title" :contents="card.contents" />
				</div>
			</div>
		</div>
	</main>
</template>

<script>
import AppCard from '@/components/AppCard.vue';

export default {
	components: {
		AppCard,
	},
	setup() {
		const cards = [
			{ title: 'Title 1', contents: 'Something important contents.' },
			{ title: 'Title 2', contents: '~ Something important contents ~' },
			{ title: 'Title 3', contents: '! Something important contents !' },
			{ title: 'Title 4', contents: '@ Something important contents @' },
			{ title: 'Title 5', contents: '# Something important contents #' },
			{ title: 'Title 6', contents: '$ Something important contents $' },
		];

		return { cards };
	},
};
</script>

<style scoped></style>
