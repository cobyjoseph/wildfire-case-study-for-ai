<script>
	import { onMount } from 'svelte';

	let headers = [];

	onMount(() => {
		// Capture all H2 and H3 tags
		headers = Array.from(document.querySelectorAll('h2, h3'));
	});
</script>

<div class="container">
	<div class="content">
		<h1>Your Main Title</h1>
		<h2>Subheading 1</h2>
		<p>Some text here...</p>
		<h3>Sub-subheading 1</h3>
		<p>Some text here...</p>
		<h2>Subheading 2</h2>
		<p>Some text here...</p>
		<!-- Add more content as needed -->
	</div>

	<div class="toc sticky">
		<strong>Table of Contents</strong>
		<ul>
			{#each headers as header (header.id)}
				<li><a href="#{header.id}">{header.innerText}</a></li>
			{/each}
		</ul>
	</div>
</div>

<style>
	.container {
		display: flex;
		justify-content: space-between;
	}

	.content {
		flex: 2;
		margin-right: 20px;
	}

	.toc {
		flex: 1;
	}

	.sticky {
		position: -webkit-sticky; /* For Safari */
		position: sticky;
		top: 10px;
	}
</style>
