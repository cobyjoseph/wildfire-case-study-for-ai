<script>
	import Bullet from '../lib/Bullet.svelte';
	import InnerBullet from '../lib/InnerBullet.svelte';
	import { fade } from 'svelte/transition';
</script>

<div class="content">
	<script>
		import Bullet from './Bullet.svelte';
	</script>

	<Bullet>
		<span slot="outer">This is the outer content.</span>
		<div slot="inner">
			<li>First item of the list</li>
			<li>Second item of the list</li>
			<!-- Add as many list items as needed -->
		</div>
	</Bullet>

	<Bullet>
		<span slot="outer">This is the outer content.</span>
		<div slot="inner">
			<li>First item of the list</li>
			<li>Second item of the list</li>
			<InnerBullet>
				<span slot="outer">testing this</span>
				<span slot="inner">
					<li>First item of the list</li>
				</span>
			</InnerBullet>
			<!-- Add as many list items as needed -->
		</div>
	</Bullet>

	<h1>Your Article Title</h1>

	<p>
		This is your introductory text. You can write a few lines or paragraphs here to introduce your
		article's main theme or subject.
	</p>

	<h2>First Header</h2>
	<p>
		This is the text that follows your first header. You can write as much as you want here,
		explaining the topic or providing more details.
	</p>

	<h2>Second Header</h2>
	<p>
		Another text section under the second header. This is just a template, so feel free to structure
		the content as you see fit.
	</p>

	<ul>
		<li>First bullet point</li>
		<li>Second bullet point</li>
		<li>Third bullet point</li>
	</ul>

	<!-- You can continue adding more sections as needed -->
</div>

<style>
	.content {
		width: 92%;
		max-width: 700px;
		margin: 0 auto; /* center the content */
		padding: 20px;
	}

	.content h1 {
		font-size: 2em;
		margin-bottom: 20px;
	}

	.content h2 {
		font-size: 1.5em;
		margin-top: 20px;
		margin-bottom: 10px;
	}

	.content p {
		margin-bottom: 20px;
		line-height: 1.6; /* improve readability */
	}

	.content ul {
		list-style-type: disc; /* default bullet point */
		margin-left: 20px; /* indent bullet points */
		margin-bottom: 20px;
	}

	.content ul li {
		margin-bottom: 10px; /* space between bullet points */
	}
</style>
