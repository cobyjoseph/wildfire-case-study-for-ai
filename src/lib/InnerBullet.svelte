<script>
	import { fade, slide } from 'svelte/transition';

	let isOpen = false;

	function toggle() {
		isOpen = !isOpen;
	}
</script>

<div class="bullet ml-[1.2em] mt-4">
	<div class="bullet-header" on:click={toggle}>
		<span class="arrow {isOpen ? 'open' : ''}">▷</span>
		<span>
			<slot name="outer" />
			<!-- Named slot for the header -->
		</span>
	</div>
	{#if isOpen}
		<div in:slide={{ y: 10 }} out:slide={{ y: 10 }} class="bullet-content ml-16 mt-3">
			<ul>
				<slot name="inner" />
				<!-- Slot for projected list items -->
			</ul>
		</div>
	{/if}
</div>

<style>
	.bullet-header {
		cursor: pointer;
		display: flex;
		align-items: flex-start;
	}

	.bullet-content ul {
		list-style-type: disc;
		padding-left: 10px; /* Adjust this value as needed to control the indent */
	}

	.arrow {
		transition: transform 0.2s ease-in-out;
		margin-right: 20px;
	}

	.arrow.open {
		transform: rotate(90deg);
	}
</style>
