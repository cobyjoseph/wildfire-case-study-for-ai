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
		<em
			>This case study was written in response to <a
				href="https://forum.effectivealtruism.org/posts/idrBxfsHkYeTtpm2q/seeking-paid-case-studies-on-standards"
				>this</a
			>
			call for proposals by Holden Karnofsky on safety standards to inform possible standards on leading
			AI labs. It represents ~65 hours of research, interviews, and writing. I am grateful to
			<a href="https://law.stanford.edu/directory/michael-wara/">Michael Wara</a>
			(Stanford Law School Senior Research Scholar and consultant for wildfire risk to the
			California Office of Energy Infrastructure Safety),
			<a href="https://www.turn.org/tlong">Tom Long</a>
			(Director of Legal Strategy at TURN),
			<a href="http://www.adamsbroadwell.com/attorneys/marc-d-joseph1/">Marc Joseph</a> (former shareholder
			and President at
		</em>Adams, Broadwell, Joseph, & Cardozo<em> and my father), and one other expert with knowledge of the Office of Energy Infrastructure
			Safety who chose to remain anonymous to allow me to interview them for this case study.
		</em>
	</p>

	<h1>Background and overview</h1>

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

	<p class="italic">(Click any bullet to show more)</p>

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

	<div class=" py-1 pr-5 pl-2 bg-slate-800 rounded-md mt-5">
		<Bullet>
			<span slot="outer"
				><div class="text-lg font-semibold pb-4">Wildfire Mitigation Plan components</div></span
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

	<h1>Key takeaways</h1>

	<h2>Proactvity vs. reactivity</h2>

	<ul>
		<li>
			When starting from a low base, creating and enforcing standards can be a lengthy process – it
			took roughly 5-10+ years after it was clear that catastrophic risk was present and rising for
			standards to be created and have a meaningful impact across all utilities. This point is
			summarized in the bullets below and explored in more detail in this text box. link
		</li>
		<ul>
			<li>
				Until legislation required stricter regulation in (particularly starting in 2017),
				regulators lacked sufficient capacity and will to impose rules in the face of opposition
				from most utilities.
			</li>
			<li>
				It then took several years to determine an appropriate regulatory framework and build
				internal expertise.
			</li>
			<li>
				This was followed by a year or two during which regulators approved substandard safety plans
				on the condition that utilities would build capacity for improving safety over time.
			</li>
		</ul>
	</ul>

	<Bullet>
		<span slot="outer"
			>Amid a changing risk landscape, utilities have appeared not to take tail risk sufficiently
			seriously until it experiences it first hand, even when such risk would threaten company
			profits. More concerningly in this case, regulators have not mandated stricter safety
			standards for utilities until that utility has caused a disaster. <strong>
				Some events that look like ‘warning shots’ in hindsight did not sufficiently spur urgent
				safety improvements.
			</strong>
			<i>(Click to see some examples of events that could have been viewed as warning shots)</i
			></span
		>
		<div slot="inner">
			<li>
				Events that drew attention to catastrophic threat but failed to spur significant action
				include the following:
			</li>
			<ul>
				<li>
					San Diego Gas and Electric (SDG&E) equipment <a
						href="https://www.latimes.com/business/hiltzik/la-fi-hiltzik-sdge-wildfires-20170112-story.html"
						>sparked a wildfire</a
					>
					in 2007 that killed two people and destroyed more than 1,500 homes. This prompted the utility
					to significantly increase its focus on fire prevention (<em>see more here </em>link ). The
					fire also increased CPUC efforts to increase safety standards on all utilities, but
					resulted in little meaningful regulatory change.
				</li>
				<li>
					In 2015, PG&E equipment sparked the <a
						href="https://www.fire.ca.gov/incidents/2015/9/9/butte-fire/">Butte fire</a
					>
					that killed two people. (<em
						>See more about the history of increasing fire risk here
					</em>link<em>). </em>While the CPUC did require some safety action during this period, it
					did not require PG&E to create a wildfire safety plan until mandated by legislation in
					2017. Link Its first 2019 WMP came after the company caused devastating fires in 2017 and
					2018. link
				</li>
				<li>
					PG&E was found to have deficiencies in its safety culture and practices in its gas
					department, which led to a pipeline explosion that killed six people in 2010 (for which
					the <a
						href="https://abc7news.com/pge-fine-pacific-gas-and-electric-san-bruno-fire-explosion/1722674/"
						>company was convicted</a
					>
					on six felony charges). This triggered significant efforts to improve the gas department’s
					safety practices. This could have piqued investigations into the company’s electricity safety
					culture, too. (While I’m not certain as to whether such investigations occurred, no significant
					regulation forced improvements to PG&E’s (deficient) safety culture and practices related to
					electrical equipment. link
					<ul>
						<li>
							The Attorney prosecuting PG&E following the 2018 Camp Fire (which killed 85 people)
							concluded that “a nearly identical dynamic had manifested within the electric
							transmission division” as the gas division, where workers felt pressure to cut
							operating and inspection costs, leading to insufficient safety checks.<sup id="fnref3"
								><a href="#fn3" rel="footnote">3</a></sup
							>
						</li>
					</ul>
				</li>
				<li>
					<strong>The pattern extends beyond California:</strong> One expert I spoke with (Michael
					Wara) believes this pattern – whereby utilities fail to sufficiently take precaution (or
					be forced by regulators to act) until they’ve caused a catastrophic fire – has been
					playing out for utilities across the country, too. He stated that this reactivity will
					likely lead to more disasters.<strong />In Hawaii, for example,
					<a
						href="https://twitter.com/michaelwwara/status/1709717342115057841?s=48&t=jvABLpmiJy24m6BINifJrQ"
						>Hawaiian Electric</a
					>
					decided against using Public Safety Power Shutoffs (as is used by California utilities) and
					deemed its coverage area to be less prone to catastrophic fires than California. Its equipment
					then caused the 2023
					<a href="https://www.nytimes.com/article/maui-wildfires-hawaii.html">Lahaina fire</a> that
					killed about 100 people.
				</li>
			</ul>
		</div>
	</Bullet>

	<div class=" py-1 pr-5 pl-2 bg-slate-800 rounded-md mt-5">
		<Bullet>
			<span slot="outer"
				><div class="text-lg font-semibold pb-4">The evolution of safety standards</div></span
			>
			<div slot="inner" class="-mt-2 pb-3">
				<li>
					<strong>Rising risk: </strong>Wildfire risk has risen quickly and substantially over the
					past ~20 years (as indicated by many reports and all expert conversations). As one
					example, the PG&E President stated that 15 percent of PG&E service territory (which covers
					Northern and Central California) had been at high risk of fire in 2012, and that this
					amount had more than tripled by 2019.<sup id="fnref4"
						><a href="#fn4" rel="footnote">4</a></sup
					>
				</li>
				<li>
					<strong>Slow and limited regulation:</strong> In the late 2000s, the CPUC initiated
					hearings regarding wildfire safety policies, and activists pushed for stricter regulation.
					(<em>See more details about activist involvement and proposed policies here</em>link ).
					The process was slow, adversarial, and
					<a
						href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
						>resulted in limited regulation</a
					>
					(especially on PG&E) during the late 2000s and most of the 2010s. (<em
						>Click to see more)</em
					>
					<ul>
						<li>
							<a
								href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
								>In 2012</a
							>, the CPUC required Southern California Edison and SDG&E to create fire prevention
							plans. It did not require PG&E to create such a plan, but required that PG&E make a
							“good faith” effort to determine if such a plan was needed. PG&E determined a plan was
							not necessary, but submitted a six-page summary of prevention and mitigation plan.
						</li>
						<li>
							<a
								href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
								>In 2014</a
							>, amid ongoing drought, the CPUC mandated that utilities report each fire started by
							its equipment (as opposed to only reporting fires more than 100 acres, the rule at the
							time). This policy had been proposed in CPUC hearings six years earlier.
						</li>
						<li>
							<a
								href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
								>In 2015</a
							>, after years of pushback from PG&E and SCE, the CPUC required mapping fire risks,
							though safety advocates believed the requirements to be diluted.
						</li>
					</ul>
				</li>
				<li>
					<strong>Profit motive drove opposition from utilities: </strong>Two of the three largest
					utilities (PG&E and Southern California Edison (SCE)) fought most efforts to increase
					safety standards. PG&E in particular was highly
					<a
						href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
						>adversarial and effective</a
					>
					at slowing down regulation. “On a scale from one to 10, where 10 is really obstructive and
					zero is completely cooperative, I would have put PG&E at a nine,” said Mark Ferron, a CPUC
					commissioner from 2011 to 2014.”
					<a
						href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
						>Significant</a
					>
					<a
						href="https://www.nytimes.com/interactive/2019/03/18/business/pge-california-wildfires.html"
						>reporting</a
					> suggests profit motive appeared to be the main reason for utility resistance.
				</li>
				<li>
					<strong>Regulators lacked expertise:</strong> From
					<a
						href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
						>2008 - 2018</a
					>, the CPUC “didn’t have a single staff member who specialized in wildfire prevention.
					During that period, according to three former employees, the [CPUC] was hamstrung by too
					few enforcement officers and distracted by simultaneous investigations into other utility
					catastrophes, which allowed utility lawyers to dominate its proceedings.”
				</li>
				<li>
					<strong
						>Catastrophic fires caused by PG&E in 2017 sparked legislation to mandate WMPs.</strong
					>
					(<em>Click to see more)</em>
					<ul>
						<li>
							Existing regulations were insufficient to mitigate catastrophic risk, at least in the
							PG&E service territory. In 2017, PG&E equipment started <a
								href="https://www.nytimes.com/interactive/2019/03/18/business/pge-california-wildfires.html"
								>17 of 21 major Northern California fires</a
							>, including fires that
							<a
								href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
								>killed 44 people</a
							>. For many fires, regulators
							<a
								href="https://www.nytimes.com/interactive/2019/03/18/business/pge-california-wildfires.html"
								>found</a
							> “PG&E violated state law or could have done more to make its equipment safer.”
						</li>
						<li>
							<strong>This prompted stricter regulation by the California legislature</strong>.
							Following the fires, a law was passed requiring California’s utilities to develop “a
							legally binding wildfire safety plan… or face criminal charges.” Wildfire Mitigation
							Plans (WMPs) were first required in 2019.
						</li>
						<li>
							In 2018, before the requirement for WMPs took effect, old and insufficiently inspected
							PG&E equipment ignited the Camp Fire that killed 85 people in Paradise, California.
							PG&E later <a
								href="https://www.npr.org/2020/06/16/879008760/pg-e-pleads-guilty-on-2018-california-camp-fire-our-equipment-started-that-fire#:~:text=Hourly%20News-,PG%26E%20Pleads%20Guilty%20On%202018%20California%20Camp%20Fire%3A%20'Our%20Equipment,has%20been%20charged%20with%20homicide."
								>pleaded guilty</a
							> to 84 counts of involuntary manslaughter for the fire.
						</li>
						<li>
							Alongside the requirement for utilities to submit WMPs in 2019, the CPUC<a
								href="https://energysafety.ca.gov/wp-content/uploads/docs/strategic-roadmap/final_report_wildfiremitigationstrategy_wsd.pdf"
							>
								initiated a project</a
							> to “create a vision, strategy, and roadmap to outline its efforts to systematically reduce
							the risk of ignition of wildfires from utility infrastructure.” This included establishing
							a Wildfire Safety Division, which transitioned into the office of Energy Safety in 2021.
						</li>
					</ul>
				</li>
				<li>
					<strong
						>Liabilities from 2017 and 2018 fires caused PG&E and to declare bankruptcy:
					</strong>PG&E
					<a
						href="https://www.nytimes.com/2020/07/01/business/energy-environment/pge-bankruptcy-ends.html"
						>declared bankruptcy in 2019</a
					>
					when facing up to $30 billion in liabilities. (<em
						>See more about legal liability for utilities here</em
					>)<strong />
				</li>
				<li>
					<strong
						>Following stricter regulation and bankruptcy for PG&E, utilities have taken several
						years to increase their compliance capacity.</strong
					>
					<ul>
						<li>
							Initial WMPs had significant room for improvement. Energy Safety issued safety
							certifications in 2020 even though they identified “<a
								href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf">serious deficiencies</a
							>” in each of their WMPs. Energy Safety
							<a href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf">argued</a> that holding
							the utility to a higher standard would be unrealistic and result in denied WMPs for years.
							“Without approved plans, the utilities cannot be held accountable for the progress promised
							in those plans and denial would prevent them from implementing incremental progress over
							their prior approved plan. Instead, Energy Safety evaluates utility improvement over the
							previous year and, if sufficient, approves the WMP while providing clear direction on how
							to mature the capability going forward.”
						</li>
					</ul>
				</li>
				<li>
					<strong
						>Current oversight and standards are Imperfect but hugely improved and improving:</strong
					> All experts I spoke with agree the process is hugely improved now, though still a work in
					progress. Several suggested that Energy Safety is highly competent, and has built internal
					capacity as quickly as could be expected. (It should be noted that these experts may have bias
					from working with Energy Safety). Although wildfire risk from utility equipment is still meaningfully
					high, it is significantly reduced and all parties involved are committed to continual safety
					improvements..
				</li>
			</div>
		</Bullet>
	</div>

	<h2>Utility motives</h2>

	<ul>
		<li>
			On its surface, the California utility market appears more likely than most to be one in which
			companies are motivated by public welfare, including for the following reasons:
		</li>
		<ul>
			<li>Utilities have a highly regulated business model.</li>
			<li>Wildfire risk has become clear after utilities have caused deadly catastrophes.</li>
			<li>
				Utilities face significant reputational challenges. PG&E in particular has received
				significant negative publicity for many years related to wildfires. Its employees live among
				their customers, and according to one expert, employees have received death threats and been
				shot at while working.
			</li>
		</ul>
	</ul>

	<Bullet>
		<span slot="outer"
			>Still, while experts believe public welfare and reputational concerns have played a role in
			utility decisions, most decisions (especially by PG&E) would be best predicted by utilities’
			profit maximizing incentive structure, including consistent underspending on maintenance.
			<i>(Click to see more)</i></span
		>
		<div slot="inner">
			<li>
				California investor-owned utilities are regulated monopolies. Through a <a
					href="https://www.cpuc.ca.gov/industries-and-topics/electrical-energy/electric-rates/general-rate-case"
					>General Rate Case</a
				>
				proceeding every four years, utilities propose electric revenue based on their anticipated expenses.
				<ul>
					<li>
						For approved capital investments, utilities are allowed to recover costs plus a fixed
						profit.
					</li>
					<li>
						For operating expenditures, utilities are only allowed to recover the projected
						expenditure without profit. However, if operating expenditures come in below the
						previously approved amount, these savings become utility profits.
					</li>
					<li>
						<strong
							>Public reporting and experts I interviewed consistently found this business model to
							be a principal reason for consistent underspending on maintenance, which has (fairly
							directly) led to catastrophic fires.
						</strong>
					</li>
				</ul>
			</li>
			<li>
				PG&E behavior in particular has been consistently characterized by profit seeking motives.
				This point has been widely argued, including in this New York Times Article “<a
					href="https://www.nytimes.com/interactive/2019/03/18/business/pge-california-wildfires.html"
					>How PG&E Ignored Fire Risks in Favor of Profits</a
				>.” Some illustrative anecdotes include the following:
				<ul>
					<li>
						In describing the history of PG&E leading up to its 2019 bankruptcy, author Katherine
						Blunt described <strong>“</strong>A series of executives had sought to please investors
						and politicians, often at the expense of customers. By the time the company confronted
						the risks of its aging electric grid, the problems were staggering.”<sup id="fnref5"
							><a href="#fn5" rel="footnote">5</a></sup
						>
					</li>
					<li>
						In <a
							href="https://www.nytimes.com/interactive/2019/03/18/business/pge-california-wildfires.html"
							>discussing</a
						> resistance to regulation during the 2010s, a PG&E utilities commissioner described of PG&E:
						“There was very much a focus on the bottom line over everything: ‘What are the earnings we
						can report this quarter?’” “And things really got squeezed on the maintenance side.”
					</li>
					<li>
						Even following bankruptcy, PG&E’s choices for executives appear to prioritize profit
						over safety. In a letter to the company, Governor Newsom indicated he was “troubled to
						learn that PG&E is primed to reconstitute its board with hedge fund financiers,
						out-of-state executives and others with little or no experience in California and
						inadequate expertise in utility operations, regulation and safety. With this move, PG&E
						would send a clear message that it is prioritizing quick profits for Wall Street over
						public safety and reliable and affordable energy service.” The company moved forward
						with the appointments anyway.<sup id="fnref6"><a href="#fn6" rel="footnote">6</a></sup>
					</li>
				</ul>
			</li>
		</div>
	</Bullet>

	<ul>
		<li>
			Experts indicated that legal liability – established by courts rather than the legislature –
			has proved substantially more influential on company behavior than public penalties. <i
				>(See the text box below for more information)
			</i>
		</li>
	</ul>

	<div class=" py-1 pr-5 pl-2 bg-slate-800 rounded-md mt-5">
		<Bullet>
			<span slot="outer"
				><div class="text-lg font-semibold pb-4">
					The evolution and status of utilities’ legal liability for fire damage
				</div></span
			>
			<div slot="inner" class="-mt-2 pb-3">
				<li>
					Due to a <a
						href="https://www.counties.org/sites/main/files/file-attachments/csac_issue_brief_inverse_condemnation_7-25-18.pdf"
						>California court decision</a
					>, utilities are legally required to reimburse wildfire victims for damages from fires
					started by utility equipment <em>regardless of whether the utility was at fault</em>. My
					interpretation from expert discussions is that <strong>the</strong>
					<strong
						>threat of legal liability has significantly (though not always sufficiently) motivated
						utilities to reduce wildfire threat</strong
					>, once the utility acknowledged the risk.
				</li>
				<li>
					The liability stems from “inverse condemnation,” which is a legal concept that flips the
					idea of eminent domain and establishes that property owners are entitled to compensation
					if it is damaged to serve a public purpose. A California court determined that the
					liability applied to investor-owned utilities in 1999, if their equipment sparks a
					wildfire that damages private property.<sup id="fnref7"
						><a href="#fn7" rel="footnote">7</a></sup
					>
				</li>
				<li>
					This liability (among other possible reasons), appears to have successfully motivated at
					least one utility (SDG&E) to voluntarily prioritize safety efforts (see more here). In
					contrast, it has not led to sufficient safety priority for PG&E, and led to the company
					declaring <a
						href="https://www.nytimes.com/2020/07/01/business/energy-environment/pge-bankruptcy-ends.html"
						>bankruptcy in 2019</a
					> when facing up to $30 billion in liabilities for fires started by poorly maintained equipment.
				</li>
				<li>
					Legislation in 2019 established the <a
						href="https://www.cawildfirefund.com/#:~:text=The%20California%20Wildfire%20Fund%20exists,caused%20by%20the%20participating%20utility."
						>California Wildfire Fund</a
					>, which effectively serves as insurance against very large liabilities. Utilities can
					draw from the fund for liabilities above $1 billion. Utilities are advantaged in this
					process if they have a safety certification from Energy Safety, as
					<a href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf">described in more detail</a
					>
					by the California State Auditor below.
					<ul>
						<li>
							“Participating utilities may seek payment from the Wildfire Fund to satisfy
							third-party claims for covered wildfires that exceed the greater of $1 billion in any
							year or the amount of insurance the utility must maintain. State law requires
							participating utilities to maintain reasonable insurance coverage, the amount of which
							the fund administrator must periodically review and recommend. In general, utilities
							must reimburse the fund for costs that the CPUC determines are not just and
							reasonable. By law, utilities with a valid safety certification for the period in
							which the wildfire ignited are presumed to have acted reasonably, and if the CPUC
							determines the costs for which they claim reimbursement are not just and reasonable,
							the amount the utility must reimburse the Wildfire Fund is capped. However, if the
							CPUC determines that the utility’s costs were not reasonable and it did not have a
							safety certification or the fund administrator determines that its actions or
							inactions constituted a conscious or willful disregard of the rights and safety of
							others, the utility must reimburse the Wildfire Fund in full.”
						</li>
					</ul>
				</li>
			</div>
		</Bullet>
	</div>

	<Bullet>
		<span slot="outer"
			>Tying executive pay to safety outcomes may meaningfully influence utility behavior, but the
			mechanism by which this is done may make an important difference. <i>(Click to see more)</i
			></span
		>
		<div slot="inner">
			<li>
				Energy Safety requires utilities to submit executive payment plans, which are approved if it
				is shown to be dependent on safety outcomes (though utilities have some freedom on how to
				interpret this).<sup id="fnref8"><a href="#fn8" rel="footnote">8</a></sup>
				<ul>
					<li>
						Following bankruptcy, PG&E was given the additional requirement to base a “significant
						component of long-term incentive compensation on safety performance.”
					</li>
				</ul>
			</li>
			<li>
				One expert (Michael Wara) suggested such a program would be much more influential if
				executive pay was also required to follow a long-term (e.g. 10+ year) vesting schedule, such
				that executives would lose significant pay if the company failed to avert long-term
				catastrophic risks.
			</li>
		</div>
	</Bullet>

	<h2>Activists and third parties</h2>

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
		font-size: 2.4em;
		margin-bottom: 14px;
		margin-top: 30px;
		font-weight: 600;
	}

	.content h2 {
		font-size: 1.5em;
		margin-top: 30px;
		font-weight: 600;
		margin-bottom: 20px;
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
