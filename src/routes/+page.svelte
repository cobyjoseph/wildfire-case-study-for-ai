<script>
	import Bullet from '../lib/Bullet.svelte';
	import InnerBullet from '../lib/InnerBullet.svelte';
	import { fade } from 'svelte/transition';
</script>

<div class="content">
	<div class=" font-bold text-lg text-blue-400 text-center">
		Case study on safety standards to prevent wildfires caused by CA utilities
	</div>

	<p class=" italic">
		This case study investigates safety standards applied to investor-owned electrical companies in
		California (‘utilities’) to reduce the risk of utility equipment igniting catastrophic
		wildfires. California investor-owned utilities are regulated monopolies responsible for
		purchasing and distributing electricity across the state. Three utilities cover most of the
		state, with Pacific Gas and Electric (PG&E) being the largest.<sup id="fnref1"
			><a href="#fn1" rel="footnote">1</a></sup
		>
	</p>

	<h1>Background and overview</h1>

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

	<p>
		This case study investigates safety standards applied to investor-owned electrical companies in
		California (‘utilities’) to reduce the risk of utility equipment igniting catastrophic
		wildfires. California investor-owned utilities are regulated monopolies responsible for
		purchasing and distributing electricity across the state. Three utilities cover most of the
		state, with Pacific Gas and Electric (PG&E) being the largest.<sup id="fnref1"
			><a href="#fn1" rel="footnote">1</a></sup
		>
	</p>
	<p>
		The field has many possible parallels to the current and possible future landscape for frontier
		AI labs. Some possible similarities are listed below (though some may become dissimilarities
		depending on how the AI field evolves).
	</p>
	<ul>
		<li>
			Catastrophic risk is posed by a small number of companies (three utilities cover most of the
			state).<sup id="fnref2"><a href="#fn2" rel="footnote">2</a></sup>
		</li>
		<li>It is infeasible to fully eliminate catastrophic risk (at least in short-medium term).</li>
		<li>Risk has quickly increased in the past two decades.</li>
		<li>
			During this time, risk levels and the individual sources of risk have been highly uncertain
			(though they are better understood now).
		</li>
		<li>The cost and effectiveness of risk mitigation strategies has also been largely unclear.</li>
		<li>
			Safety standards partially resemble a licensing scheme, with approval based on a fairly
			subjective evaluation across a wide range of metrics.
		</li>
		<li>
			Safety measures can accompany economic tradeoffs for the general public (namely higher
			electricity rates).
		</li>
		<li>
			Reputational risks play an important factor for utilities, as the largest utilities are well
			known by the general public and the risk posed by such companies is widely discussed in
			California media and politics.
			<p>
				This case study aims to highlight examples of company actions and regulator successes and
				challenges in this (potentially) similar environment, to help calibrate our expectations for
				AI company behavior and the risks and opportunities for safety standard strategies.
			</p>
			<p>
				Based on my research, the following features of safety standard development on California
				utilities to prevent catastrophic wildfires should provide (further) caution for AI safety
				standard setting [link all]:
			</p>
			<ul>
				<li>
					Creating and enforcing standards while building regulator and company capacity has been a
					lengthy process (even after motivation among all parties was high).
				</li>
				<li>
					Companies and regulators did not sufficiently internalize and respond proactively to
					catastrophic risk as it rose (even when there were many indications that risk was
					growing).
				</li>
				<li>
					Events that look like warning shots in hindsight generally did not spark sufficient
					urgency around safety; only the largest and most direct disasters spurred significant
					regulation.
				</li>
				<li>
					Motives have been mixed and varied, but reputational risk and concern for public welfare
					have not alone been as influential as profit motive for all companies.
				</li>
				<li>
					Regulators were too slow to address uncertainty about the level and source of catastrophic
					risk (though sources of risk are much better understood now).
				</li>
				<li>
					It can be highly challenging for regulators to create a system with quick enough feedback
					loops that:
					<ul>
						<li>incorporates past utility performance into annual regulatory sign off, and</li>
						<li>
							allows for the regulator to update guidelines on safety best practices as evidence for
							the cost and effectiveness of various safety strategies is limited and changing.
						</li>
					</ul>
				</li>
			</ul>
		</li>
	</ul>

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
	<div class="h-[1px] w-[50%] bg-white" />

	<div class="mt-2 text-sm">
		<span id="fn1"
			>(Footnote content here. <a href="#fnref1" title="Return to the text" rel="footnote">↩</a
			>)</span
		>
	</div>
	<div class="mt-2 text-sm">
		<span id="fn2"
			>(Footnote content here. <a href="#fnref2" title="Return to the text" rel="footnote">↩</a
			>)</span
		>
	</div>
	<div class="mt-2 text-sm">
		<span id="fn3"
			>(Footnote content here. <a href="#fnref3" title="Return to the text" rel="footnote">↩</a
			>)</span
		>
	</div>
	<div class="mt-2 text-sm">
		<span id="fn4"
			>(Footnote content here. <a href="#fnref4" title="Return to the text" rel="footnote">↩</a
			>)</span
		>
	</div>
	<div class="mt-2 text-sm">
		<span id="fn5"
			>(Footnote content here. <a href="#fnref5" title="Return to the text" rel="footnote">↩</a
			>)</span
		>
	</div>
	<div class="mt-2 text-sm">
		<span id="fn6"
			>(Footnote content here. <a href="#fnref6" title="Return to the text" rel="footnote">↩</a
			>)</span
		>
	</div>
</div>

<style>
	.content {
		width: 92%;
		max-width: 700px;
		margin: 0 auto; /* center the content */
		padding: 20px;
	}

	.content h1 {
		font-size: 1.8em;
		margin-bottom: 14px;
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

	sup a {
		text-decoration: none;
		color: inherit;
	}

	sup a:hover {
		text-decoration: underline;
	}

	.footnote-ref {
		text-decoration: none;
		color: inherit;
	}

	.footnote-ref:hover {
		text-decoration: underline;
	}

	.footnote {
		font-size: 0.5em;
		margin-left: 5px;
		vertical-align: super;
	}

	.backref {
		text-decoration: none;
		font-size: 0.7em;
	}

	.backref:hover {
		text-decoration: underline;
	}
</style>
