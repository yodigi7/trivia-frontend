<script lang="ts">
	import QuestionAnswer from '$lib/question-answer.svelte';

	let query: string;
	let showAdvanced: boolean = false;
	let count = 50;
	// TODO: need to actually send the search to api
	function search() {
		console.log(query);
		console.log(count);
	}
</script>

<div class="container h-full mx-auto flex flex-col justify-center items-center max-w-4xl">
	<form class="w-full" on:submit|preventDefault={search}>
		<label for="query" class="pb-2">Trivia Question Query:</label>
		<!-- TODO: need to make the text input a more visible text -->
		<div class="flex pb-8">
			<input required class="w-full rounded-lg" bind:value={query} type="text" id="query" />
			<button class="btn variant-filled rounded-full" type="submit">Search</button>
		</div>
		<button on:click={() => (showAdvanced = !showAdvanced)}>
			Show Advanced
			<!-- TODO: make this work and look better -->
			{#if !showAdvanced}
				v
			{:else}
				^
			{/if}
		</button>
		{#if showAdvanced}
			<div class="fadein">
				<label for="count">Results to return:</label>
				<!-- TODO: need to make the text input a more visible text -->
				<input bind:value={count} type="number" min="1" max="100" id="count" class="rounded-lg" />
			</div>
		{/if}
	</form>
	<br />

	<QuestionAnswer question="question" answer="answer" choices={['yes', 'hello']} />
</div>

<style>
	.fadein {
		opacity: 1;
		animation: 0.5s fadein;
	}

	@keyframes fadein {
		from {
			opacity: 0;
		}
	}
</style>
