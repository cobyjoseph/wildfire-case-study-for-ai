<script>
	import Bullet from '../lib/Bullet.svelte';
	import InnerBullet from '../lib/InnerBullet.svelte';
	import { fade } from 'svelte/transition';
</script>

<div class="content">
	<div class="mb-5">
		<div class=" font-bold text-lg text-blue-400">
			Case study: Safety standards on California utilities to prevent wildfires
		</div>
		<div class="text-xs">
			<div class="mt-1">Coby Joseph</div>
			<div class="mt-1">October 25, 2023</div>
		</div>
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

	<!-- TEMPLATE -->
	<Bullet>
		<span slot="outer">This is the outer content.</span>
		<div slot="inner">
			<li>First item of the list</li>
			<li>Second item of the list</li>
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
		</li>
	</ul>
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
			catastrophic risk as it rose (even when there were many indications that risk was growing).
		</li>
		<li>
			Events that look like warning shots in hindsight generally did not spark sufficient urgency
			around safety; only the largest and most direct disasters spurred significant regulation.
		</li>
		<li>
			Motives have been mixed and varied, but reputational risk and concern for public welfare have
			not alone been as influential as profit motive for all companies.
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
					allows for the regulator to update guidelines on safety best practices as evidence for the
					cost and effectiveness of various safety strategies is limited and changing.
				</li>
			</ul>
		</li>
	</ul>

	<p>
		This case study also explores possible benefits and challenges of several regulatory strategies
		that have been used to prevent wildfires that could be relevant for the AI safety field. [make
		this sentence more precise]
	</p>
	<ul>
		<li>
			Strict, no-fault, legal liability on utilities has been hugely important in shaping utility
			incentives. Still, it hasn't forced all utilities to take sufficient actions around safety.
		</li>
		<li>
			In the face of legal liability, penalties (or their threat) have not played an important role
			in motivating utility behavior, though some suggest they could be used more frequently and
			strongly.
		</li>
		<li>
			The State's dependence on utilities for (affordable) electricity has limited regulator
			leverage to extract safety actions.
		</li>
		<li>Tying executive pay to safety outcomes can be a replicable model.</li>
		<li>
			Establishing regulation of catastrophic risk in a different regulatory body from the body that
			authorizes funding has created a range of possible benefits and challenges. It may have:
			<ul>
				<li>
					helped raise the competence of the safety regulation and utility focus on safety
					practices,
				</li>
				<li>
					contributed to limiting clarity among all parties on how utilities should best handle
					safety and economic tradeoffs,
				</li>
				<li>created bureaucratic challenges that must be navigated between various regulators.</li>
			</ul>
		</li>
		<li>(say anything about audits)?</li>
	</ul>
	<p>Finally, the case study highlights:</p>
	<ul>
		<li>
			how private activists have seemingly played an important role in shaping safety standards,
			despite years of being rebuffed, and
		</li>
		<li>
			how voluntary safety actions by (primarily) one utility have helped inform safety policies and
			raised expectations for other utilities.
		</li>
	</ul>
	<p>This case study is structured as follows:</p>
	<ul>
		<li>The problem that safety standards aim to address link</li>
		<li>Current standards link</li>
		<li>
			More details on each of the key findings listed above, organized by theme (e.g. proactivity vs
			reactivity, utility motives, etc. link ). [ maybe organize same way as above]
		</li>
	</ul>
	<p>
		Each section contains bullet points that can be clicked to expand and reveal additional detail.
	</p>
	<h1>The need for safety standards</h1>

	<Bullet>
		<span slot="outer">California wildfires cause significant death and destruction. </span>
		<div slot="inner">
			<li>
				<a href="https://calmatters.org/california-wildfire-map-tracker/">Since 2008</a>, California
				wildfires have killed 225 people and damaged or destroyed more than 50,000 structures. Since
				2015, they have caused around $25 billion in “property and contents” loss (which does not
				include lost economic activity or fire suppression costs).
			</li>
		</div>
	</Bullet>
	<Bullet>
		<span slot="outer"
			>The risk of wildfires has significantly increased in recent decades, almost certainly due to
			climate change-induced droughts.</span
		>
		<div slot="inner">
			<li>
				Out of California’s <a href="https://calmatters.org/california-wildfire-map-tracker/"
					>20 largest wildfires</a
				> up to 2022, seven occurred in 2020 and 2021 alone.
			</li>
			<li>
				Climate change appears to be significantly exacerbating catastrophic wildfire risk by
				increasing drought frequency and severity.
			</li>
		</div>
	</Bullet>
	<Bullet>
		<span slot="outer"
			>Equipment from California’s utilities is a significant source of wildfires that have killed
			hundreds of people and caused billions of dollars in damage.</span
		>
		<div slot="inner">
			<li>
				Utility equipment caused fires that burned a <a
					href="https://calmatters.org/california-wildfire-map-tracker/">similar number of acres</a
				> as fires caused by humans or lightning in 2017, 2019, and 2021.
			</li>
			<li>
				PG&E, the state’s largest utility, <a
					href="https://www.npr.org/2020/06/16/879008760/pg-e-pleads-guilty-on-2018-california-camp-fire-our-equipment-started-that-fire#:~:text=Hourly%20News-,PG%26E%20Pleads%20Guilty%20On%202018%20California%20Camp%20Fire%3A%20'Our%20Equipment,has%20been%20charged%20with%20homicide."
					>pleaded guilty</a
				>
				to 84 counts of involuntary manslaughter following the 2018 Camp Fire, the deadliest wildfire
				in the state’s history, which was caused by old PG&E equipment. PG&E equipment was
				<a
					href="https://www.cnbc.com/2022/01/05/california-finds-pge-equipment-responsible-for-massive-dixie-fire-.html"
					>also responsible</a
				>
				for starting the Dixie Fire, the state’s second largest fire by acreage, which destroyed more
				than 1,300 homes in 2021. PG&E filed for
				<a
					href="https://www.nytimes.com/2019/01/29/business/energy-environment/pge-file-bankruptcy.html"
					>bankruptcy in 2019</a
				> after facing liability claims for dozens of fires.
			</li>
			<!-- Add as many list items as needed -->
		</div>
	</Bullet>
	<Bullet>
		<span slot="outer"
			>There is no simple and affordable solution to eliminate wildfire risk from utility equipment.</span
		>
		<div slot="inner">
			<li>
				<a
					href="https://www.pge.com/pge_global/common/pdfs/customer-service/other-services/electric-undergrounding-program/PGE-Undergrounding-Fact-Sheet.pdf"
					>Undergrounding</a
				>
				sections of overhead power lines eliminates nearly all wildfire risk from those power lines.
				However, undergrounding all existing overhead distribution and transmission lines is
				<a
					href="https://www.cpuc.ca.gov/industries-and-topics/electrical-energy/infrastructure/electric-reliability/undergrounding-program-description#:~:text=According%20to%20PG%26E%2C%20SCE%20and,to%20%246.072%20million%20per%20mile."
					>estimated</a
				> to cost more than $750 billion. Just undergrounding lines in the highest fire risk areas would
				cost substantially less, though still many hundreds of billions of dollars.
			</li>

			<!-- Add as many list items as needed -->
		</div>
	</Bullet>

	<h1>Current standards</h1>

	<p>
		The top points in this section summarize the main current safety standards. Each bullet point
		can be expanded for additional information.
	</p>
	<ul>
		<li>
			The California Public Utilities Commission (CPUC) is the primary regulator of utilities. In
			2022, the Office of Energy Infrastructure Safety (‘Energy Safety’) was created outside of the
			CPUC to oversee utility processes related to reducing wildfire risk. <em
				>See this textbox
			</em>link
			<em
				>for more information about the creation of Energy Safety and its interaction with the CPUC.</em
			>
		</li>
	</ul>

	<Bullet>
		<span slot="outer"
			>Energy Safety issues “<a
				href="https://energysafety.ca.gov/what-we-do/electrical-infrastructure-safety/wildfire-mitigation-and-safety/safety-certifications/safety-certification-faqs/"
				>safety certifications</a
			>'' to qualifying utilities. Failure to receive a safety certification would significantly
			harm a utility’s financial standing. <em>Click to show more</em></span
		>
		<div slot="inner">
			<li>
				Receiving a safety certification increases the chances that a utility could draw on the <a
					href="https://www.cawildfirefund.com/#:~:text=The%20California%20Wildfire%20Fund%20exists,caused%20by%20the%20participating%20utility."
					>California Wildfire Fund</a
				>
				to repay victims of a wildfire caused by its equipment, for which the utility would be automatically
				liable. (<em>More information about legal liability facing utilities here</em>link
				<em>.) </em>Experts stressed that failure to receive safety certification would immediately
				cause a significant stock price drop for the utility, and would likely lead to a drop in its
				credit rating.
			</li>

			<!-- Add as many list items as needed -->
		</div>
	</Bullet>
	<ul>
		<li>
			Core requirements for a safety certification <a
				href="https://energysafety.ca.gov/what-we-do/electrical-infrastructure-safety/wildfire-mitigation-and-safety/safety-certifications/safety-certification-faqs/"
				>include</a
			>:
			<InnerBullet>
				<span slot="outer">a <strong>safety culture assessment,</strong> </span>

				<span slot="inner">
					<li>
						Energy Safety conducts <a
							href="https://energysafety.ca.gov/what-we-do/electrical-infrastructure-safety/wildfire-mitigation-and-safety/safety-culture-assessments/"
							>safety culture assessments</a
						> through a third-party administrator. The assessment includes:
					</li>
					<ul>
						<li>a workforce survey,</li>
						<li>
							a self-assessment by utility management on company culture toward 22 safety culture
							elements (with supporting documentation required),
						</li>
						<li>self-reporting on lessons learned, and</li>
						<li>interviews and observational visits.</li>
					</ul>
					<li>
						To complete this requirement, the utility must have agreed to implement the findings of
						its most recent safety culture assessment.
					</li>
				</span>
			</InnerBullet>

			<ul />
		</li>

		<div class="ml-[3.35em]">
			<li>
				an <strong>approved executive compensation structure</strong> that ties compensation to
				safety performance. <em>This requirement is explained in more detail here.</em>
			</li>
			<li>
				an annually approved <strong>Wildfire Mitigation Plan</strong> (WMP).
				<a
					href="https://energysafety.ca.gov/what-we-do/electrical-infrastructure-safety/wildfire-mitigation-and-safety/wildfire-mitigation-plans/"
					>WMPs</a
				>
				“describe how the electrical corporation is constructing, maintaining, and operating its electrical
				lines and equipment in a manner that will minimize the risk of catastrophic wildfire.” WMP evaluation
				also includes an assessment for a utility’s capacity to execute the plan.
				<em>The text box below </em>link
				<em> provides more details about the WMP components.</em>
			</li>
			<li>
				Demonstration of implementing its approved WMP, and board-of-director-level safety reporting
				structure.
			</li>
		</div>
	</ul>

	<Bullet>
		<span slot="outer">
			Auditing includes field inspections, independent evaluations, and annual assessments of
			compliance with the WMP. Energy Safety can recommend to the CPUC to impose penalties on
			utilities “for noncompliance with its approved plan.”</span
		>
		<div slot="inner">
			<li>
				By statute, the compliance process must include <a
					href="https://energysafety.ca.gov/wp-content/uploads/2022-wmp-compliance-process.pdf"
					>the following components</a
				>:
				<ul>
					<li>Field inspections conducted by Energy Safety.</li>
					<li>Annual compliance reports conducted by the utility.</li>
					<li>
						An independent evaluator, hired by the utility from a list approved by Energy Safety.
					</li>
					<li>Vegetation management (and possibly other) audits, conducted by Energy Safety.</li>
				</ul>
			</li>
			<li>See herelink for additional analysis of the auditing process.</li>
		</div>
	</Bullet>

	<div class=" py-1 pr-5 bg-slate-800 rounded-md mt-5">
		<Bullet>
			<span slot="outer"
				><div class="text-lg font-semibold pb-3">Wildfire Mitigation Plan components</div></span
			>
			<div slot="inner" class="-mt-2 pb-3">
				<li>
					Wildfire Mitigation Plans (WMPs) <a
						href="https://www.kqed.org/news/11750455/what-you-need-to-know-about-pges-state-mandated-wildfire-mitigation-plan#:~:text=Wildfire%20mitigation%20plans%3A%20What%20are,Northern%20California%20in%20October%202017."
						>were mandated</a
					> by law for all utilities following devastating 2017 fires ignited by PG&E equipment. The
					first versions were required to be completed in 2019.
				</li>
				<li>
					The latest WMPs must cover utility plans for 2023-2025, and must be approved by Energy
					Safety and updated each year. WMPs are evaluated based on a range of criteria listed below
					(paraphrased from the ‘2023-2025 WMP Technical Guidelines – 12/7/22’ accessible <a
						href="https://energysafety.ca.gov/what-we-do/electrical-infrastructure-safety/wildfire-mitigation-and-safety/wildfire-mitigation-plans/2023-wildfire-mitigation-plans/"
						>here</a
					>):
				</li>
				<ul>
					<li>
						completeness with Public Utilities Code requirements and Energy Safety’s Guidelines,
					</li>
					<li>technical and programmatic feasibility and effectiveness,</li>
					<li>
						resource use efficiency to achieve “the greatest risk reduction with the most efficient
						use of funds and workforce resources,”
					</li>
					<li>demonstrated year-over-year progress,</li>
					<li>
						forward-looking growth, including a long term strategy and clear action plan to
						“continue reducing utility-related ignitions and the scale, scope, and frequency of
						Public Safety Power Shutoff (PSPS) events” (<em>PSPS are described here),</em>
					</li>
					<li>
						use of performance metrics to evaluate wildfire risk, Public Safety Power Shutoffs, and
						other risks,
					</li>
					<li>
						and quantitative targets to track completion of initiatives in electrical corporation’s
						approved WMP.
					</li>
					<li>
						WMP assessment includes input from California Department of Forestry and Fire Protection
						(CAL FIRE), public and stakeholder comments, data supplied by corporation,
					</li>
					<li>
						<em
							>Submitted WMPs can be accessed <a
								href="https://energysafety.ca.gov/what-we-do/electrical-infrastructure-safety/wildfire-mitigation-and-safety/wildfire-mitigation-plans/2023-wildfire-mitigation-plans/"
								>here</a
							>.</em
						>
					</li>
				</ul>

				<li>
					Energy Safety also uses a self-accessed <a
						href="https://energysafety.ca.gov/what-we-do/electrical-infrastructure-safety/wildfire-mitigation-and-safety/wildfire-mitigation-plans/2023-wildfire-mitigation-plans/"
						>Maturity Model</a
					> to track each utility’s WMP and its capabilities to execute the WMP. The 2023-2025 model
					examines 37 individual capabilities, each evaluated based on 20 possible sub-capabilities.
				</li>
				<li>
					Experts indicated that the WMP process is intended to encourage continuous improvement
					rather than meeting a minimum standard.
				</li>
				<li>
					One expert indicated that the WMP requirements change fairly substantially year-to-year as
					Energy Safety learns and improves.
				</li>
			</div>
		</Bullet>
	</div>

	<!-- You can continue adding more sections as needed -->
	<div class="h-[1px] w-[50%] bg-white mt-10" />

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
	a {
		color: #60a5fa;
	}

	.content {
		width: 92%;
		max-width: 700px;
		margin: 0 auto; /* center the content */
		padding: 20px;
	}

	.content h1 {
		font-size: 1.8em;
		margin-bottom: 14px;
            margin-top: 20px;
	}

	.content h2 {
		font-size: 1.5em;
		margin-top: 20px;
		margin-bottom: 10px;
	}

	.content p {
		margin-bottom: 10px;
		line-height: 1.6; /* improve readability */
	}

	.content ul {
		list-style-type: disc; /* default bullet point */
		margin-left: 35px;
		margin-bottom: 15px;
	}

	.content ul li {
		margin-top: 5px;
		margin-bottom: 10px;
		padding-left: 10px; /* added this line to push text to the right */
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
