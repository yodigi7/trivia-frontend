<script lang="ts">
	let query: string;
	function search() {
		console.log(query);
	}
</script>

<div class="container h-full mx-auto flex justify-center items-center w-3/4 max-w-xl">
	<form class="w-full" on:submit|preventDefault={search}>
		<label for="query">Trivia Question Query</label>
		<!-- TODO: need to make the text input a more visible text -->
		<input class="w-full rounded-lg" bind:value={query} type="text" id="query" />
		<button class="btn variant-filled rounded-full">Search</button>
	</form>
</div>
