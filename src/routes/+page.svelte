<script>
	import Bullet from '../lib/Bullet.svelte';
	import InnerBullet from '../lib/InnerBullet.svelte';
	import { fade } from 'svelte/transition';
	import ContentWithTOC from '$lib/ContentWithTOC.svelte';
</script>

<div class="grid-container">
	<div />

	<div class="content">
		<div class="mb-5">
			<div class=" font-bold text-2xl my-3 text-blue-400">
				Case study: Safety standards on California utilities to prevent wildfires
			</div>
			<div class="text-xs">
				<div class="mt-1">Coby Joseph</div>
				<div class="mt-1">October 26, 2023</div>
			</div>
		</div>

		<p class=" italic">
			<em
				>This case study was written in response to <a
					href="https://forum.effectivealtruism.org/posts/idrBxfsHkYeTtpm2q/seeking-paid-case-studies-on-standards"
					>this</a
				>
				call for proposals by Holden Karnofsky to inform possible safety standards on leading AI labs.
				It represents ~65 hours of research, interviews, and writing. I am grateful to
				<a href="https://law.stanford.edu/directory/michael-wara/">Michael Wara</a>
				(Stanford Law School Senior Research Scholar and consultant for wildfire risk to the California
				Office of Energy Infrastructure Safety),
				<a href="https://www.turn.org/tlong">Tom Long</a>
				(Director of Legal Strategy at TURN),
				<a href="http://www.adamsbroadwell.com/attorneys/marc-d-joseph1/">Marc Joseph</a> (former shareholder
				and President at
			</em>Adams, Broadwell, Joseph, & Cardozo
			<em>
				and my father), and one other expert with knowledge of the Office of Energy Infrastructure
				Safety who chose to remain anonymous to allow me to interview them for this case study.
			</em>
		</p>

		<h1 id="background">Background and overview</h1>

		<p>
			This case study investigates safety standards applied to investor-owned electrical companies
			in California (‘utilities’) to reduce the risk of utility equipment igniting catastrophic
			wildfires. California investor-owned utilities are regulated monopolies responsible for
			purchasing and distributing electricity across the state. Three utilities cover most of the
			state, with Pacific Gas and Electric (PG&E) being the largest.<sup id="fnref1"
				><a href="#fn1" rel="footnote">1</a></sup
			>
		</p>
		<p>
			The field has many possible parallels to the current and possible future landscape for
			frontier AI labs. Some possible similarities are listed below (though some may become
			dissimilarities depending on how the AI field evolves).
		</p>
		<ul>
			<li>
				Catastrophic wildfire risk is posed by a small number of companies in California (three
				utilities cover most of the state).<sup id="fnref2"><a href="#fn2" rel="footnote">2</a></sup
				>
			</li>
			<li>
				It is infeasible to fully eliminate catastrophic wildfire risk (at least in short-medium
				term).
			</li>
			<li>The risk of catastrophic wildfires has quickly increased in the past two decades.</li>
			<li>
				During this time, risk levels and the individual sources of risk have been highly uncertain
				(though they are better understood now).
			</li>
			<li>
				The cost and effectiveness of risk mitigation strategies has also been largely unclear.
			</li>
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
			</li>
		</ul>
		<p>
			This case study aims to highlight examples of company actions and regulator successes and
			challenges in this (potentially) similar environment, to help calibrate our expectations for
			AI company behavior and the risks and opportunities for safety standard strategies.
		</p>
		<p>
			Based on my research, the following features of safety standard development on California
			utilities to prevent catastrophic wildfires should provide (further) caution for AI safety
			standard setting:
		</p>
		<ul>
			<li>
				<a href="#1">
					Creating and enforcing standards while building regulator and company capacity has been a
					lengthy process (even after motivation among all parties was high).
				</a>
			</li>
			<li>
				<a href="#2">
					Companies and regulators did not sufficiently internalize and respond proactively to
					catastrophic risk as it rose (even when there were many indications that risk was
					growing).
				</a>
			</li>
			<li>
				<a href="#3">
					Events that look like warning shots in hindsight generally did not spark sufficient
					urgency around safety; only the largest and most direct disasters spurred significant
					regulation.
				</a>
			</li>
			<li>
				<a href="#4">
					Motives have been mixed and varied, but reputational risk and concern for public welfare
					have not alone been as influential as profit motive for all companies.
				</a>
			</li>
			<li>
				<a href="#5">
					Regulators were too slow to address uncertainty about the level and source of catastrophic
					risk (though sources of risk are much better understood now).
				</a>
			</li>
			<li>
				It can be highly challenging for regulators to create a system with quick enough feedback
				loops that:
				<ul>
					<li>
						<a href="#6">
							incorporates past utility performance into annual regulatory sign off, and</a
						>
					</li>

					<li>
						<a href="#7">
							allows for the regulator to update guidelines on safety best practices (while evidence
							for the cost and effectiveness of various safety strategies is limited and changing).
						</a>
					</li>
				</ul>
			</li>
		</ul>

		<p>
			This case study also explores possible benefits and challenges of several regulatory
			strategies that could be relevant for the AI field.
		</p>
		<ul>
			<li>
				<a href="#8">
					Strict, no-fault, legal liability on utilities has been hugely important in shaping
					utility incentives. Still, it hasn't forced all utilities to take sufficient safety
					precautions.
				</a>
			</li>
			<li>
				<a href="#9">
					In the face of legal liability, penalties (or their threat) do not appear to have played
					an important role in motivating utility behavior, though some suggest they could be used
					more frequently and strongly.
				</a>
			</li>
			<li>
				<a href="#10">
					California's dependence on utilities for (affordable) electricity has limited regulator
					leverage to extract safety actions.
				</a>
			</li>
			<li><a href="#11"> Tying executive pay to safety outcomes can be a replicable model. </a></li>
			<li>
				Establishing regulation of catastrophic risk in a different regulatory body from the body
				that authorizes funding has created a range of possible benefits and challenges. It may
				have:
				<ul>
					<li>
						<a href="#12">
							helped raise the competence of safety regulation and utility focus on safety
							practices,
						</a>
					</li>
					<li>
						<a href="#13">
							contributed to limiting clarity among all parties on how utilities should best handle
							safety and economic tradeoffs, and
						</a>
					</li>
					<li>
						<a href="#14">
							created bureaucratic challenges that must be navigated between various regulators.
						</a>
					</li>
				</ul>
			</li>
		</ul>
		<p>Finally, the case study highlights:</p>
		<ul>
			<li>
				<a href="#15">
					how private activists have seemingly played an important role in shaping safety standards,
					despite years of being rebuffed, and
				</a>
			</li>
			<li>
				<a href="#16">
					how voluntary safety actions by (primarily) one utility have helped inform safety policies
					and raised expectations for other utilities.
				</a>
			</li>
		</ul>

		<h2 id="contents">Contents</h2>

		<p>This case study is structured as follows:</p>
		<ul>
			<li><a href="#17"> The problem that safety standards aim to address.</a></li>
			<li><a href="#18"> Current standards.</a></li>
			<li>
				<a href="#19">
					More details on each of the key findings listed above, organized by theme (e.g. <a
						href="#20">proactivity vs reactivity</a
					>, <a href="#21">utility motives</a>, etc.).
				</a>
			</li>
		</ul>
		<p>
			<strong
				>Bullet points with arrows next to them can be clicked to reveal additional detail.</strong
			>
		</p>
		<h1 id="17">The need for safety standards</h1>

		<Bullet>
			<span slot="outer">California wildfires cause significant death and destruction. </span>
			<div slot="inner">
				<li>
					<a href="https://calmatters.org/california-wildfire-map-tracker/">Since 2008</a>,
					California wildfires have killed 225 people and damaged or destroyed more than 50,000
					structures. Since 2015, they have caused around $25 billion in “property and contents”
					loss (which does not include lost economic activity or fire suppression costs).
				</li>
			</div>
		</Bullet>
		<Bullet>
			<span slot="outer"
				>The risk of wildfires has significantly increased in recent decades, almost certainly due
				to climate change-induced droughts.</span
			>
			<div slot="inner">
				<li>
					Out of California’s <a href="https://calmatters.org/california-wildfire-map-tracker/"
						>20 largest wildfires</a
					> up to 2022, seven occurred in 2020 and 2021 alone.
				</li>
				<li>
					Climate change appears to be significantly exacerbating catastrophic wildfire risk by <a
						href="https://caseagrant.ucsd.edu/faq-droughts-californias-coastal-regions"
						>increasing drought frequency and severity</a
					>.
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
						href="https://calmatters.org/california-wildfire-map-tracker/"
						>similar number of acres</a
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
				>There is no simple and affordable solution to eliminate wildfire risk from utility
				equipment.</span
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
					> to cost more than $750 billion. Just undergrounding lines in the highest fire risk areas
					would cost substantially less, though one expert indicated it would still cost many hundreds
					of billions of dollars.
				</li>

				<!-- Add as many list items as needed -->
			</div>
		</Bullet>

		<h1 id="18">Current standards</h1>

		<ul>
			<li>
				The California Public Utilities Commission (CPUC) is the primary regulator of utilities. In
				2022, the Office of Energy Infrastructure Safety (‘Energy Safety’) was created outside of
				the CPUC to oversee utility processes related to reducing wildfire risk.
			</li>
		</ul>

		<Bullet>
			<span slot="outer"
				>Energy Safety issues “<a
					href="https://energysafety.ca.gov/what-we-do/electrical-infrastructure-safety/wildfire-mitigation-and-safety/safety-certifications/safety-certification-faqs/"
					>safety certifications</a
				>'' to qualifying utilities. Failure to receive a safety certification would significantly
				harm a utility’s financial standing.</span
			>
			<div slot="inner">
				<li>
					Receiving a safety certification increases the chances that a utility could draw on the <a
						href="https://www.cawildfirefund.com/#:~:text=The%20California%20Wildfire%20Fund%20exists,caused%20by%20the%20participating%20utility."
						>California Wildfire Fund</a
					>
					to repay victims of a wildfire caused by its equipment, for which the utility would be automatically
					liable. (<em
						>More information about legal liability facing utilities <a href="#8">here</a></em
					>). Experts stressed that failure to receive safety certification would immediately cause
					a significant stock price drop for the utility, and would likely lead to a drop in its
					credit rating.
				</li>
			</div>
		</Bullet>
		<div class="h-[0.6rem]" />

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
					</span>
				</InnerBullet>

				<ul />
			</li>

			<div class="ml-[3.35em]">
				<li>
					an <strong>approved executive compensation structure</strong> that ties compensation to
					safety performance.
					<em>This requirement is explained in more detail <a href="#11">here</a>.</em>
				</li>
				<li>
					an annually approved <strong>Wildfire Mitigation Plan</strong> (WMP).
					<a
						href="https://energysafety.ca.gov/what-we-do/electrical-infrastructure-safety/wildfire-mitigation-and-safety/wildfire-mitigation-plans/"
						>WMPs</a
					>
					“describe how the electrical corporation is constructing, maintaining, and operating its electrical
					lines and equipment in a manner that will minimize the risk of catastrophic wildfire.” WMP
					evaluation also includes an assessment for a utility’s capacity to execute the plan.
					<em>The text box below </em>
					<em> provides more details about the WMP components.</em>
				</li>
				<li>
					Demonstration of implementing its approved WMP, and board-of-director-level safety
					reporting structure.
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
							Evaluation by an independent evaluator, hired by the utility from a list approved by
							Energy Safety.
						</li>
						<li>Vegetation management (and possibly other) audits, conducted by Energy Safety.</li>
					</ul>
				</li>
				<li>See additional analysis of the auditing process <a href="#9">here</a>.</li>
			</div>
		</Bullet>

		<div class=" py-1 pr-5 pl-2 bg-slate-800 rounded-md mt-5">
			<Bullet>
				<span slot="outer"
					><div id="components" class="text-lg font-semibold pb-4">
						Wildfire Mitigation Plan components
					</div></span
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
						Safety and updated each year. WMPs are evaluated based on a range of criteria listed
						below (paraphrased from the ‘2023-2025 WMP Technical Guidelines – 12/7/22’ accessible <a
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
							resource use efficiency to achieve “the greatest risk reduction with the most
							efficient use of funds and workforce resources,”
						</li>
						<li>demonstrated year-over-year progress,</li>
						<li>
							forward-looking growth, including a long term strategy and clear action plan to
							“continue reducing utility-related ignitions and the scale, scope, and frequency of
							<a href="https://www.cpuc.ca.gov/psps/">Public Safety Power Shutoffs</a> events”
						</li>
						<li>
							use of performance metrics to evaluate wildfire risk, Public Safety Power Shutoffs,
							and other risks,
						</li>
						<li>
							and quantitative targets to track completion of initiatives in electrical
							corporation’s approved WMP.
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
						One expert indicated that the WMP requirements change fairly substantially year-to-year
						as Energy Safety learns and improves.
					</li>
				</div>
			</Bullet>
		</div>

		<h1 id="19">Key takeaways</h1>

		<h2 id="20">Proactivity vs. reactivity</h2>

		<ul>
			<li id="1">
				When starting from a low base, creating and enforcing standards can be a lengthy process –
				it took roughly 5-10+ years after it was clear that catastrophic risk was present and rising
				for standards to be created and have a meaningful impact on all utilities. <em
					>This point is summarized in the bullets below and explored in more detail in <a
						href="#evolutionTextBox">this text box.</a
					></em
				>
			</li>
			<ul>
				<li>
					Until legislation required stricter regulation (particularly starting in 2017), regulators
					lacked sufficient capacity and will to promptly impose rules in the face of opposition from most
					utilities.
				</li>
				<li>
					Following legislation, it took several years to build internal regulatory structure and expertise.
				</li>
				<li>
					For the first year or two under new regulatory structure, regulators approved substandard safety
					plans on the condition that utilities would build capacity for improving safety over time.
				</li>
			</ul>
		</ul>

		<Bullet>
			<span id="2" slot="outer"
				>Amid a changing risk landscape, utilities have appeared not to take tail risk sufficiently
				seriously until they experience it first hand, even when such risk would threaten company
				profits. More concerningly, regulators have generaly not mandated substantially stricter
				safety standards for utilities until that utility has caused a disaster. <strong>
					Some events that look like ‘warning shots’ in hindsight did not sufficiently spur urgent
					safety improvements.
				</strong>
			</span>
			<div id="3" slot="inner">
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
						to significantly increase its focus on fire prevention. The fire also increased CPUC efforts
						to increase safety standards on all utilities, but resulted in little meaningful regulatory
						change.
					</li>
					<li>
						In 2015, PG&E equipment sparked the <a
							href="https://www.fire.ca.gov/incidents/2015/9/9/butte-fire/">Butte fire</a
						>
						that killed two people. The CPUC did not not require PG&E to create a wildfire safety plan
						until mandated by legislation in 2017. By the time its first WMP was completed (2019), the
						utility had already caused devastating fires in 2017 and 2018. (<em
							>See more about the history of increasing fire risk and the evolution of safety
							standards <a href="#evolution">here)</a>
						</em>.
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
						regulation forced improvements to PG&E’s (deficient) safety culture and practices related
						to electrical equipment during this time.)
						<ul>
							<li>
								The Attorney prosecuting PG&E following the 2018 Camp Fire (which killed 85 people)
								concluded that “a nearly identical dynamic had manifested within the electric
								transmission division” as the gas division, where workers felt pressure to cut
								operating and inspection costs, leading to insufficient safety checks.<sup
									id="fnref3"><a href="#fn3" rel="footnote">3</a></sup
								>
							</li>
						</ul>
					</li>
				</ul>
				<li>
					<strong>The pattern likely extends beyond California:</strong> One expert I spoke with
					(Michael Wara) believes this pattern – whereby utilities fail to sufficiently take
					precaution (or be forced by regulators to act) until they’ve caused a catastrophic fire –
					has been playing out for utilities across the country, too. <strong />In Hawaii, for
					example,
					<a
						href="https://twitter.com/michaelwwara/status/1709717342115057841?s=48&t=jvABLpmiJy24m6BINifJrQ"
						>Hawaiian Electric</a
					>
					decided against using Public Safety Power Shutoffs to prevent catastrophic wildfire (as is
					used by California utilities) and deemed its coverage area to be less prone to catastrophic
					fires than California. Its equipment then caused the 2023
					<a href="https://www.nytimes.com/article/maui-wildfires-hawaii.html">Lahaina fire</a> that
					killed about 100 people.
				</li>
			</div>
		</Bullet>

		<div id="evolutionTextBox" class=" py-1 pr-5 pl-2 bg-slate-800 rounded-md mt-5">
			<Bullet>
				<span slot="outer"
					><div id="evolution" class="text-lg font-semibold pb-4">
						The evolution of safety standards
					</div></span
				>
				<div slot="inner" class="-mt-2 pb-3">
					<li>
						<strong>Rising risk: </strong>Wildfire risk has risen quickly and substantially over the
						past ~20 years (as indicated by many reports and all expert conversations). As one
						example, the PG&E President stated that 15 percent of PG&E service territory (which
						covers Northern and Central California) had been at high risk of fire in 2012, and that
						this amount had more than tripled by 2019.<sup id="fnref4"
							><a href="#fn4" rel="footnote">4</a></sup
						>
					</li>
					<li>
						<strong>Slow and limited regulation:</strong> In the late 2000s, the CPUC initiated
						hearings regarding wildfire safety policies, and activists pushed for stricter
						regulation. (<em
							>See more details about activist involvement and proposed policies <a href="#15"
								>here</a
							></em
						>). The process was slow, adversarial, and
						<a
							href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
							>resulted in limited regulation</a
						>
						(especially on PG&E) during the late 2000s and most of the 2010s.
						<ul>
							<li>
								<a
									href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
									>In 2012</a
								>, the CPUC required Southern California Edison (SCE) and SDG&E to create fire
								prevention plans. It did not require PG&E to create such a plan, but required that
								PG&E make a “good faith” effort to determine if such a plan was needed. PG&E
								determined a plan was not necessary, but submitted a six-page summary of a
								prevention and mitigation plan.
							</li>
							<li>
								<a
									href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
									>In 2014</a
								>, amid ongoing drought, the CPUC mandated that utilities report each fire started
								by its equipment (as opposed to only reporting fires more than 100 acres, the rule
								at the time). This policy had been proposed in CPUC hearings six years earlier.
							</li>
							<li>
								<a
									href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
									>In 2018</a
								>, after years of pushback from PG&E and SCE, the CPUC required mapping fire risks,
								though safety advocates believed the requirements to be diluted.
							</li>
						</ul>
					</li>
					<li>
						<strong>Profit motive drove opposition from utilities: </strong>Two of the three largest
						utilities (PG&E and SCE) fought most efforts to increase safety standards. PG&E in
						particular was highly
						<a
							href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
							>adversarial and effective</a
						>
						at slowing down regulation. According to a CPUC commissioner from 2011 to 2014 “On a scale
						from one to 10, where 10 is really obstructive and zero is completely cooperative, I would
						have put PG&E at a nine.”
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
						few enforcement officers and distracted by simultaneous investigations into other
						utility catastrophes, which allowed utility lawyers to dominate its proceedings.”
					</li>
					<li>
						<strong
							>Catastrophic fires caused by PG&E in 2017 sparked legislation to mandate WMPs.</strong
						>
						<ul>
							<li>
								Existing regulations were insufficient to mitigate catastrophic risk, at least in
								the PG&E service territory. In 2017, PG&E equipment started <a
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
								In 2018, before the requirement for WMPs took effect, old and insufficiently
								inspected PG&E equipment ignited the Camp Fire that killed 85 people in Paradise,
								California. PG&E later <a
									href="https://www.npr.org/2020/06/16/879008760/pg-e-pleads-guilty-on-2018-california-camp-fire-our-equipment-started-that-fire#:~:text=Hourly%20News-,PG%26E%20Pleads%20Guilty%20On%202018%20California%20Camp%20Fire%3A%20'Our%20Equipment,has%20been%20charged%20with%20homicide."
									>pleaded guilty</a
								> to 84 counts of involuntary manslaughter for the fire.
							</li>
							<li>
								Alongside the requirement for utilities to submit WMPs in 2019, the CPUC <a
									href="https://energysafety.ca.gov/wp-content/uploads/docs/strategic-roadmap/final_report_wildfiremitigationstrategy_wsd.pdf"
								>
									initiated a project</a
								> to “create a vision, strategy, and roadmap to outline its efforts to systematically
								reduce the risk of ignition of wildfires from utility infrastructure.” This included
								establishing a Wildfire Safety Division, which transitioned into the Office of Energy
								Safety in 2021.
							</li>
						</ul>
					</li>
					<li>
						Liabilities from 2017 and 2018 fires caused PG&E to declare bankruptcy
						<a
							href="https://www.nytimes.com/2020/07/01/business/energy-environment/pge-bankruptcy-ends.html"
							>in 2019</a
						>
						when facing up to $30 billion in liabilities. (<em
							>See more about legal liability for utilities <a href="#8">here</a></em
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
									href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf"
									>serious deficiencies</a
								>” in each of their WMPs. Energy Safety
								<a href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf">argued</a> that holding
								the utility to a higher standard would be unrealistic and result in denied WMPs for years.
								“Without approved plans, the utilities cannot be held accountable for the progress promised
								in those plans and denial would prevent them from implementing incremental progress over
								their prior approved plan. Instead, Energy Safety evaluates utility improvement over
								the previous year and, if sufficient, approves the WMP while providing clear direction
								on how to mature the capability going forward.”
							</li>
						</ul>
					</li>
					<li>
						<strong
							>Current oversight and standards are imperfect but hugely improved and improving:</strong
						> All experts I spoke with agree the process is significantly more effective at reducing
						wildfire risk compared to several years prior, though still a work in progress. Several suggested
						that Energy Safety is highly competent, and has built internal capacity as quickly as could
						be expected. Although wildfire risk from utility equipment is still meaningfully high, they
						indicated that it is significantly reduced and all parties involved are committed to continual
						safety improvements. (It should be noted that these experts may have bias from working with
						Energy Safety).
					</li>
				</div>
			</Bullet>
		</div>

		<h2 id="motives">Utility motives</h2>

		<ul>
			<li id="4">
				On its surface, the California utility market appears more likely than most capitalist
				markets to be one in which companies prioritize public welfare, including for the following
				reasons:
			</li>
			<ul>
				<li>Utilities have a highly regulated business model.</li>
				<li>Wildfire risk has become clear after utilities have caused deadly catastrophes.</li>
				<li>
					Utilities face significant reputational challenges. PG&E in particular has received
					significant negative publicity for many years related to wildfires. Its employees live
					among their customers, and according to one expert, employees have received death threats
					and been shot at while working.
				</li>
			</ul>
		</ul>

		<Bullet>
			<span slot="outer"
				>Still, while experts believe public welfare and reputational concerns have played a role in
				utility decisions, most decisions (especially by PG&E) would be best predicted by utilities’
				profit maximizing incentive structure, including consistent underspending on maintenance.
			</span>
			<div slot="inner">
				<li>
					California investor-owned utilities are regulated monopolies. Through a <a
						href="https://www.cpuc.ca.gov/industries-and-topics/electrical-energy/electric-rates/general-rate-case"
						>General Rate Case</a
					>
					proceeding every four years, utilities propose electric revenue based on their anticipated
					expenses.
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
								>Public reporting and experts I interviewed consistently found this business model
								to be a principal reason for consistent underspending on maintenance, which has
								(fairly directly) led to catastrophic fires.
							</strong>
						</li>
					</ul>
				</li>
				<li>
					PG&E behavior in particular has been consistently characterized by profit seeking motives.
					This point has been widely stated, including in this New York Times Article “<a
						href="https://www.nytimes.com/interactive/2019/03/18/business/pge-california-wildfires.html"
						>How PG&E Ignored Fire Risks in Favor of Profits</a
					>.” Some illustrative anecdotes include the following:
					<ul>
						<li>
							In <a
								href="https://www.nytimes.com/interactive/2019/03/18/business/pge-california-wildfires.html"
								>discussing</a
							> resistance to regulation during the 2010s, a PG&E utilities commissioner described of
							PG&E: “There was very much a focus on the bottom line over everything: ‘What are the earnings
							we can report this quarter?’” “And things really got squeezed on the maintenance side.”
						</li>
						<li>
							In describing the history of PG&E leading up to its 2019 bankruptcy, author Katherine
							Blunt described <strong>“</strong>A series of executives had sought to please
							investors and politicians, often at the expense of customers. By the time the company
							confronted the risks of its aging electric grid, the problems were staggering.”<sup
								id="fnref5"><a href="#fn5" rel="footnote">5</a></sup
							>
						</li>
						<li>
							Even following bankruptcy, PG&E’s choices for executives appear to prioritize profit
							over safety. In a letter to the company, Governor Newsom indicated he was “troubled to
							learn that PG&E is primed to reconstitute its board with hedge fund financiers,
							out-of-state executives and others with little or no experience in California and
							inadequate expertise in utility operations, regulation and safety. With this move,
							PG&E would send a clear message that it is prioritizing quick profits for Wall Street
							over public safety and reliable and affordable energy service.” The company moved
							forward with the appointments anyway.<sup id="fnref6"
								><a href="#fn6" rel="footnote">6</a></sup
							>
						</li>
					</ul>
				</li>
			</div>
		</Bullet>

		<Bullet>
			<span id="8" slot="outer">
				Experts indicated that legal liability – established by courts rather than the legislature –
				has proved substantially more influential on company behavior than public penalties.
			</span>
			<div slot="inner">
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
					if their property is damaged to serve a public purpose. A California court determined that
					the liability applied to investor-owned utilities in 1999, if their equipment sparks a
					wildfire that damages private property.<sup id="fnref7"
						><a href="#fn7" rel="footnote">7</a></sup
					>
				</li>
				<li>
					This liability (among other possible reasons), appears to have successfully motivated at
					least one utility (SDG&E) to voluntarily prioritize safety efforts (described further <a
						href="#16">here).</a
					>
					In contrast, it has not led to sufficient safety priority for PG&E, and led to the company
					declaring
					<a
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

		<Bullet>
			<span id="11" slot="outer"
				>Tying executive pay to safety outcomes may meaningfully influence utility behavior, but the
				mechanism by which this is done may make an important difference.</span
			>
			<div slot="inner">
				<li>
					Energy Safety requires utilities to submit executive payment plans, which are approved if
					they are shown to be dependent on safety outcomes (though utilities have some freedom on
					how to interpret this).<sup id="fnref8"><a href="#fn8" rel="footnote">8</a></sup>
					<ul>
						<li>
							Following bankruptcy, PG&E was given the additional requirement to base a “significant
							component of long-term incentive compensation on safety performance.”
						</li>
					</ul>
				</li>
				<li>
					One expert (Michael Wara) suggested such a program would be much more influential if
					executive pay was also required to follow a long-term (e.g. 10+ year) vesting schedule,
					such that executives would lose significant pay if the company failed to avert long-term
					catastrophic risks.
				</li>
			</div>
		</Bullet>

		<h2 id="15">Activists and third parties</h2>

		<Bullet>
			<span slot="outer"
				>Even when activists concerned about tail risks had little early success (from what I can
				tell), their proposals appeared to set the foundation for later standards.</span
			>
			<div slot="inner">
				<li>
					In 2008, the CPUC hosted public proceedings aimed at preventing wildfires caused by
					utilities (as described well in <a
						href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
						>this article</a
					>). During the proceedings,
					<strong
						>activists proposed rules that were initially rejected but later adopted in some form.</strong
					>
					Their proposals were to require that utilities:
					<ul>
						<li>
							Report each fire started by its equipment (as opposed to only reporting fires more
							than 100 acres, the rule at the time). The CPUC initially rejected the proposal amid
							pushback from PG&E and SCE, but eventually mandated it in 2014.
						</li>
						<li>
							Create detailed maps to identify fire-prone areas. The CPUC finally required such maps
							in 2018 (again, following pushback from PG&E and SCE), though not in as detailed a
							form as required in safety advocates' proposals.
						</li>
						<li>
							Create contingency plans for extreme winds that can cause catastrophic fires. This
							proposal appears to have set the foundation for requirements for fire prevention plans
							on SDG&E and SCE in 2012, and later WMPs on all utilities starting in 2019 (though I
							have not definitively confirmed this point).
						</li>
					</ul>
				</li>
				<li>
					These activists may have been motivated by a combination of factors including
					self-preservation (having previously been affected by California wildfires), public
					safety, and monetary motivations (they reportedly received significant compensation over
					many years from the CPUC <a
						href="https://www.cpuc.ca.gov/-/media/cpuc-website/divisions/administrative-law-judge-division/documents/icomp-materials/updated-icomp-program-guide-april-2017.pdf"
						>intervenor compensation program</a
					>, discussed below).
				</li>
			</div>
		</Bullet>
		<Bullet>
			<span slot="outer"
				>The <a
					href="https://www.cpuc.ca.gov/-/media/cpuc-website/divisions/administrative-law-judge-division/documents/icomp-materials/updated-icomp-program-guide-april-2017.pdf"
					>CPUC intervenor compensation program</a
				> – which pays individuals and organizations when their input has been useful to a CPUC proceeding
				– could be a replicable model to build an ecosystem of third party experts.
			</span>
			<div slot="inner">
				<li>
					The advocates described above <a
						href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
						>estimated</a
					> that they received close to $700,000 from the CPUC, as of 2020.
				</li>
				<li>
					To receive payment from the program, one must <a
						href="https://www.cpuc.ca.gov/-/media/cpuc-website/divisions/administrative-law-judge-division/documents/icomp-materials/updated-icomp-program-guide-april-2017.pdf"
						>provide</a
					> “substantial contribution” to a CPUC proceeding.
				</li>
				<li>
					My impression from speaking with Tom Long of <a href="https://www.turn.org/">TURN</a> (a legal
					advocacy organization that works with the CPUC and receives funding from the program) is that
					this program has been important to the develop the ecosystem of third party organizations providing
					expertise for the CPUC and Energy Safety (though he mentioned that Energy Safety does not currently
					have a program like the intervenor compensation program).
				</li>
			</div>
		</Bullet>
		<ul />

		<h2 id="regulation">Regulatory structure, processes, and challenges</h2>

		<Bullet>
			<span id="12" slot="outer"
				>Energy Safety was deliberately created to be a <a
					href="https://energysafety.ca.gov/who-we-are/about-energy-safety/"
					>separate regulatory body</a
				> from the CPUC to focus on regulating wildfire risk by California utilities. My impression from
				conversations with experts is that having a narrowly safety-focused organization has helped build
				significant regulatory expertise and make progress establishing a robust oversight process. One
				expert also suggested the system creates a healthy tension between Energy Safety’s focus on efficient
				risk reduction and the CPUC’s focus on spending efficiency.</span
			>
			<div slot="inner">
				<li>
					Following legislation requiring WMPs, the CPUC <a
						href="https://energysafety.ca.gov/wp-content/uploads/docs/strategic-roadmap/final_report_wildfiremitigationstrategy_wsd.pdf"
					>
						initiated a project</a
					> in 2019 to “create a vision, strategy, and roadmap to outline its efforts to systematically
					reduce the risk of ignition of wildfires from utility infrastructure.” This included establishing
					a Wildfire Safety Division, which transitioned into the office of Energy Safety in 2021.
				</li>
				<li>
					Experts indicated to me that the creation of Energy Safety as a body solely focused on
					wildfire risk from utilities was an explicit attempt to “disentangle” safety and financial
					concerns. One expert also indicated that it reflected the legislature’s lack of trust in
					the CPUC to oversee utilities regarding safety.
				</li>
				<li>
					Through <a
						href="https://www.cpuc.ca.gov/industries-and-topics/electrical-energy/electric-rates/general-rate-case"
						>General Rate Case</a
					> proceedings every four years, the CPUC authorizes utilities to collect a certain amount of
					revenue from ratepayers based on planned expenditures. As such, the CPUC has direct influence
					over whether or not utilities can recoup funds to execute their proposed WMPs.
				</li>
				<li>
					Energy Safety does not have the ability to impose penalties, rather they <a
						href="https://energysafety.ca.gov/what-we-do/electrical-infrastructure-safety/compliance/wildfire-mitigation-plan-compliance/"
						>may determine</a
					> that a utility “is not in compliance with its approved wildfire mitigation plan,” and “may
					recommend that the CPUC pursue an enforcement action against the electrical corporation for
					noncompliance with its approved plan.”
				</li>
			</div>
		</Bullet>

		<Bullet>
			<span id="13" slot="outer"
				>Still, separating the primary safety regulator from the agency that controls funding for
				safety measures has led to several challenges, too. Experts indicated that utilities may
				have insufficient clarity for how to respond to conflicting directions between the safety
				regulator and the agency that controls funding.</span
			>
			<div slot="inner">
				<li>
					Investments to reduce wildfire risk can lead to higher electricity prices for the public
					(since California utilities, as regulated monopolies, are typically allowed to pass costs
					on to customers).
				</li>
				<li>
					Since the CPUC determines (through <a
						href="https://www.cpuc.ca.gov/industries-and-topics/electrical-energy/electric-rates/general-rate-case"
						>General Rate Case</a
					> proceedings every four years) the amount that utilities can recoup from ratepayers, its decisions
					are integral to the feasibility of utility WMPs.
				</li>
				<li>
					The tension has been particularly clear during current proceedings. PG&E has put <a
						href="https://www.pgecurrents.com/articles/3858-10-000-miles-undergrounding-bold-idea-2021-significant-progress-2023"
						>significant focus</a
					>
					on undergrounding power lines to improve wildfire safety in recent years. Their 2023-2025 WMP
					proposal included
					<a href="https://www.jdsupra.com/legalnews/pg-e-and-sce-s-wildfire-mitigation-2999883/"
						>significant spending increases</a
					>
					(as did SCE’s, though my impression is that SCE is focused less on undergrounding). Experts
					indicated that the costly focus on undergrounding likely reflects PG&E’s profit incentives,
					whereby they make a regulated profit on capital expenses, but not on operating expenses (like
					cutting vegetation near power lines). They indicated to me that cheaper ‘<a
						href="https://undergroundinfrastructure.com/magazine/2010/july-2010-vol-65-no-7/features/hardening-power-lines"
						>hardening</a
					>’ techniques are likely more appropriate (despite them doing slightly less to reduce
					risk), as utility savings would result in cheaper electricity rates.
					<ul>
						<li>
							This point is also supported by an SCE study (referenced on page 25 <a
								href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf">here</a
							>) indicating that “each dollar spent replacing existing bare power lines with covered
							lines provided four times as much value in wildfire risk mitigation as a dollar spent
							on converting the bare lines to underground power lines.”
						</li>
					</ul>
				</li>
			</div>
		</Bullet>

		<Bullet>
			<span id="14" slot="outer"
				>One expert indicated to me that <strong
					>the cost and effectiveness of safety-enhancing strategies has been highly uncertain
					(though perhaps less so today than it used to be).
				</strong>The separate processes and different timelines between Energy Safety and the CPUC
				appear to risk slowing safety investments and reduce Energy Safety's flexibility to quickly
				update guidance as the cost and effectiveness of various safety strategies becomes clearer.</span
			>
			<div slot="inner">
				<li>
					Utility safety investments are largely beholden to CPUC decisions every four years
					approving the level of investment utilities can recoup from rates. There is no clear
					mechanism for updating rates between every four-year decision, which may limit Energy
					Safety’s ability to mandate continuous safety improvements on a year-to-year basis as
					evidence on best practices changes.
				</li>
				<li>
					The CPUC is currently reviewing PG&E’s General Rate Case proposal, and <a
						href="https://www.cpuc.ca.gov/news-and-updates/all-news/cpuc-releases-two-pds-in-response-to-pge-request-for-new-investments-2023"
						>has indicated</a
					>
					that it is considering two options for how PG&E should balance undergrounding and ‘hardening’
					strategies. Neither option would approve the full spending proposed by PG&E. One expert indicated
					to me that while PG&E awaits the CPUC’s decision,
					<strong
						>PG&E does not know how much it can recoup for 2023 spending, which has slowed its
						safety investments this year.</strong
					>
				</li>
			</div>
		</Bullet>

		<Bullet>
			<span id="6" slot="outer"
				>Lengthy auditing and investigation periods that reduce regulators’ ability to update
				oversight strategies appear to be particularly costly amid these uncertainties. For example,
				Energy Safety appears to have incomplete information about utilities’ compliance with the
				prior year’s WMP when evaluating its subsequent WMP.</span
			>
			<div slot="inner">
				<li>
					Especially during the 2010s, the slow regulatory process hindered safety progress. It took
					a decade for the <a
						href="https://www.sandiegouniontribune.com/business/energy-green/sd-fi-sdge-wildfirecaseruling-20171130-story.html"
						>CPUC to rule</a
					>
					that SDG&E was at fault for devastating 2007 fires. One expert indicated that this “precedent
					had huge consequences for all three of the state’s largest utilities—especially PG&E,”<sup
						id="fnref9"><a href="#fn9" rel="footnote">9</a></sup
					> and it seems possible that such a precedent could have spurred more attention to safety earlier,
					had SDG&E been found to be at fault more promptly.
				</li>
				<li id="7">
					Even in recent years, Energy Safety appears to have incomplete information about utility
					compliance with prior WMPs when evaluating subsequent WMPs. For example, Energy Safety
					only released a review of PG&E’s compliance with its 2020 WMP in February 2023.<sup
						id="fnref10"><a href="#fn10" rel="footnote">10</a></sup
					>
					(It found “that PG&E failed to substantially comply with its 2020 WMP, which “hindered its
					ability to reduce the risk of catastrophic wildfire on its system.”)
					<ul>
						<li>
							A <a href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf">2022 report</a> from the
							California State Auditor highlighted the challenges caused by this delayed evaluation.
							It stated (on page 35) “whether a utility substantially implements the projects in its
							mitigation plan has no bearing on the issuance of its safety certification as a result
							of these two factors: first, because the implementation of the plan is in progress, the
							Energy Safety Office performs only a limited review of whether a utility is implementing
							its current mitigation plan, and second, determinations of whether a utility substantially
							implemented its prior mitigation plans are not one of the criteria established in law for
							it to assess when issuing a safety certification.”
						</li>
						<li>
							In response, Energy Safety suggested that it did not believe it to be necessarily
							useful to include compliance with the most recent WMP in its subsequent WMP
							evaluation, stating the following: “Given the constantly evolving understanding of how
							best to address utility wildfire risk, any findings in the “most recently completed
							compliance assessment” may not be directly relevant or applicable to utilities’
							maturing wildfire strategies. Using the safety certification as a backward-looking,
							punitive enforcement action could undermine its value as a stabilizing incentive to
							invest in safety and, as the Report states, “support credit worthiness,” which enables
							utilities to raise capital at a lower cost to make those investments.” (available on
							page 75, <a href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf">here</a>).
						</li>
					</ul>
				</li>
			</div>
		</Bullet>

		<Bullet>
			<span id="10" slot="outer"
				>Regulation is also challenged by the state’s dependence on utilities. <strong
					>This case study highlights the risk of using a licensing scheme to regulate companies
					that become ‘too-important-to-fail.’
				</strong>Failing to issue safety certifications to utilities that insufficiently mitigate
				catastrophic risk would threaten utilities' financial standing and could lead to higher
				electricity prices.<sup id="fnref11"><a href="#fn11" rel="footnote">11</a></sup> This may make
				regulators reluctant to deny certification, thereby reducing pressure on utilities to fully comply
				with safety standards. (A similar challenge could emerge if governments and businesses become
				dependent on (updates to) AI systems).</span
			>
			<div slot="inner">
				<li>
					While experts indicated to me that Energy Safety would be highly averse to denying safety
					certification to a utility (and they have not yet done so), they do still put significant
					pressure on utilities to raise their safety capabilities. One expert indicated to me that
					the WMP evaluation process is a “negotiation, not a binary decision.” Several experts
					suggested the cost of compliance for utilities is quite high, and utilities are very
					concerned about the threat of failing to receive certification.
				</li>
				<li>
					At least in prior years, though, Energy Safety has held utilities to a lower standard.
					This appears to me to correspond with Energy Safety building its internal capacity and
					forcing utilities to continually improve safety capabilities at a rate Energy Safety feels
					is feasible.
					<ul>
						<li>
							In 2020, Energy Safety (conditionally) approved utilities’ WMPs despite identifying
							“serious deficiencies in each of their mitigation plans” (from page 35, <a
								href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf">here</a
							>).
						</li>
						<li>
							Energy Safety argued that holding the utility to a higher standard would be
							unrealistic and result in denied WMPs for years - ultimately delaying its progress.
							“Without approved plans, the utilities cannot be held accountable for the progress
							promised in those plans and denial would prevent them from implementing incremental
							progress over their prior approved plan. Instead, Energy Safety evaluates utility
							improvement over the previous year and, if sufficient, approves the WMP while
							providing clear direction on how to mature the capability going forward” (from page
							75, <a href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf">here</a>).
						</li>
					</ul>
				</li>
			</div>
		</Bullet>

		<h2 id="16">Influence of voluntary safety actions</h2>

		<Bullet>
			<span slot="outer"
				>Early voluntary safety practices by San Diego Gas and Electric (SDG&E) appear to have
				influenced subsequent safety standards applied to all large utilities. SDG&E <a
					href="https://www.nytimes.com/interactive/2019/03/18/business/pge-california-wildfires.html"
					>upgraded fire prevention efforts</a
				> after it was sued by residents for causing a devastating wildfire in 2007. Since then, it undertook
				a wide range of voluntary safety practices, and was significantly more supportive of regulation
				attempts than other utilities, especially PG&E.</span
			>
			<div slot="inner">
				<li>
					SDG&E <a
						href="https://www.psehealthyenergy.org/news/blog/preventing-wildfires-with-power-outages-2/"
						>requested approval</a
					>
					from the CPUC to use
					<a href="https://www.cpuc.ca.gov/psps/">Public Safety Power Shutoffs</a> (PSPSs) for fire prevention
					in 2008, but was denied. The CPUC allowed utilities to use PSPSs starting in 2012, and they
					have since become an important (though undesirable) fire prevention tool for utilities.
				</li>
				<li>
					‘Reclosers’ - devices that try to reclose a circuit after a fault occurs on a power line,
					are another example of a voluntary policy becoming part of safety standards (after a
					disaster, in this case). SDG&E and SCE have long <a
						href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
						>had policies</a
					>
					to block reclosers during fire season. PG&E did not have such a policy before its reclosers
					may have contributed to a 2017 fire that killed three people. This led to a
					<a
						href="https://leginfo.legislature.ca.gov/faces/billTextClient.xhtml?bill_id=201720180SB901%27"
						>bill</a
					> requiring safety policies for reclosers.
				</li>
				<li>
					More broadly, state officials <a
						href="https://www.nytimes.com/interactive/2019/03/18/business/pge-california-wildfires.html"
						>have reportedly indicated</a
					> that SDG&E could serve as a template for PG&E as it relates to safety measures. In the late
					2010s, PG&E’s vice president for community wildfire safety said PG&E often used SDG&E’s approach
					to implement safety policies.
				</li>
				<li>
					SDG&E was more supportive of policies <a
						href="https://www.pbs.org/wgbh/frontline/article/pge-california-wildfire-safety-pushback/"
						>proposed by activists in 2008</a
					> than other utilities, though it is unclear to me whether its support was influential, as
					the policies were not implemented until many years later.
				</li>
			</div>
		</Bullet>

		<Bullet>
			<span slot="outer"
				>Regulators cite peer utilities’ safety practices when evaluating WMPs. This competitive
				pressure appears to embed (sometimes voluntary) best practices into safety standards.
			</span>
			<div slot="inner">
				<li>
					One expert indicated to me that the WMP process was designed such that the period for
					public commitment could allow comparison between utilities to create a race-to-the-top
					dynamic.
				</li>
				<li>
					The following quote from Energy Safety’s Revision Notice to PG&E’s proposed 2023-2025 WMP
					provides one example of how utilities are evaluated against one another.<sup id="fnref12"
						><a href="#fn12" rel="footnote">12</a></sup
					> Energy Safety requires PG&E undertake “benchmarking with SCE and SDG&E with respect to hazard
					tree mitigation practices. PG&E then must report in its Revision Notice Response on the similarities
					and differences between the three electrical corporations’ hazard tree mitigation practices.
					Where these practices differ, PG&E must explain why its practices differ from those of its
					peers. PG&E must also describe any changes it plans to make because of this exercise and a
					timeline to implement those changes.”
				</li>
			</div>
		</Bullet>

		<h2 id="risk">Risk assessment</h2>

		<Bullet>
			<span id="5" slot="outer"
				>For many years, regulators and utilities appear to have had insufficient urgency to develop
				a robust and detailed risk identification and prioritization methodology, though risks are
				dramatically better understood and modeled today.</span
			>
			<div slot="inner">
				<li>
					As one example, it took roughly <a
						href="https://financialpost.com/pmn/business-pmn/maui-fire-lays-bare-utility-missteps-mirrored-across-the-country"
						>ten years</a
					> for maps of high risk areas to be created after regulators began such an effort in 2008.
				</li>
				<li>
					In the late 2010s, one expert described to me that the CPUC underwent a process for better
					risk identification and assessment (across all utility activities, not just wildfire
					safety). The expert indicated that the utilities were adversarial during the process,
					including strongly (but unsuccessfully) resisting the proposal for risks to be quantified.
				</li>
				<li>
					Experts indicated that risks are much better mapped and modeled today than in previous
					years. Utilities are responsible for modeling risk, and regulators rely on experts for
					detailed review of utility models.
				</li>
				<li>
					Still, a <a href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf"
						>2022 California State audit suggested</a
					> that Energy Safety didn’t require clear enough prioritization of high risk activities: “the
					office approved utilities’ 2020 and 2021 mitigation plans even though the utilities had not
					provided sufficient information on how they used risk modeling outcomes to inform decision-making
					processes, circuit prioritization for mitigation efforts, and mitigation selection.”
				</li>
				<li>
					This may have changed in the past two years, as one expert suggested that risk modeling
					now acts as an umbrella over WMP evaluation, and increased focus on risk modeling has
					become a core piece of making safety policies more proactive.
				</li>
			</div>
		</Bullet>

		<Bullet>
			<span slot="outer"
				>Still, some experts argue that risk models may focus too heavily on median wildfire risk
				rather than potential catastrophic fires.
			</span>
			<div slot="inner">
				<li>
					One expert indicated that fire risk models - while highly detailed - are still better
					suited for modeling the average type of fire, and fail to simulate extreme cases well.
					Another expert said that utilities have the choice to submit two types of analyses, one on
					tail risk and one on mean risk. The expert said they generally chose to submit an analysis
					of the mean risk (which partially covers tail risk). This expert indicated that the degree
					to which tail risk should motivate decision makers is an ongoing question.
				</li>
				<li>
					In October 2023, too, a longtime activist and wildfire safety consultant released a <a
						href="https://www.sciencedirect.com/science/article/abs/pii/S0379711223001479">paper</a
					> arguing that models “incorrectly prioritize risk drivers” and “fail to represent large fires
					due to limited run time.” It is not clear to me how widely held this belief is among experts.
				</li>
			</div>
		</Bullet>

		<h2 id="9">Audits and penalties</h2>

		<Bullet>
			<span slot="outer"
				>After causing a devastating wildfire, utilities generally face penalties from the CPUC and
				courts (if they were found to be at fault), in addition to being liable for damages caused
				to victims. Penalties from courts have generally been small relative to utility revenues.
				Some CPUC penalties have been much larger, though they are still much smaller than
				liabilities facing utilities after causing a wildfire.</span
			>
			<div slot="inner">
				<li>
					Laws that limit fine sizes appear to have kept court-issued penalties to relatively small
					totals. Despite being convicted of 84 counts of manslaughter after its old equipment
					sparked the Camp Fire, for example, PG&E was only fined
					<a
						href="https://www.nytimes.com/2020/06/16/business/energy-environment/pge-camp-fire-california-wildfires.html"
						>$3.5 million</a
					>
					by the court (PG&E had a
					<a href="https://www.macrotrends.net/stocks/charts/PCG/pacific-gas-electric/gross-profit"
						>~$17 billion</a
					>
					annual gross profit from 2022-2023). In her book <em>California Burning</em>, Katherine
					Blunt described several examples in which lawyers attempted to pursue meaningfully large
					penalties against utilities but were limited by statutory maximums.
				</li>
				<li>
					Penalties issued by the CPUC against utilities can be meaningfully large, though my
					impression is their threat is not nearly as influential on utility behavior as potential
					liabilities utilities face after causing a fire. This <a
						href="https://www.cpuc.ca.gov/news-and-updates/all-news/cpuc-staff-propose-$45-million-penalty-for-pge-over-dixie-fire"
						>partial list</a
					>
					of penalties issued against PG&E shows several over $100 million, and the largest reached
					<a
						href="https://www.utilitydive.com/news/cpuc-imposes-largest-ever-penalty-of-19b-on-pge-for-northern-california/577625/#:~:text=The%20California%20Public%20Utilities%20Commission,grim%20chapter%20in%20PG%26E's%20history%2C%E2%80%9D"
						>$1.9 billion</a
					>
					following PG&E sparking the Camp Fire that killed 85 people. Still, these pale in comparison
					to
					<a
						href="https://www.nytimes.com/2021/11/01/business/energy-environment/pge-dixie-fire.html#:~:text=PG%26E%20filed%20for%20bankruptcy%20protection,town%20of%20Paradise%20in%202018."
						>tens of billions</a
					> of dollars in liabilities that utilities have faced after causing devastating fires.
				</li>
			</div>
		</Bullet>

		<Bullet>
			<span slot="outer"
				>The CPUC does not appear to substantially use audits and penalties to punish utilities for
				failing to comply with its WMP.</span
			>
			<div slot="inner">
				<li>
					Audits are conducted by a range of actors at various (including random) times. This
					appears to <a
						href="https://energysafety.ca.gov/wp-content/uploads/2022-wmp-compliance-process.pdf"
						>include</a
					> field inspections conducted by Energy Safety, annual compliance reports conducted by the
					utility, an audit by an independent evaluator hired by the utility (from an approved list),
					and vegetation management audits conducted by Energy Safety. One expert also indicated to me
					that some individual counties also conduct their own auditing. I don’t believe this list above
					is exhaustive, as experts have mentioned other CPUC and Energy Safety audits that don’t necessarily
					fit into those categories above.
				</li>
				<li>
					Still, a <a href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf">2022 report</a> by
					the California State Auditor suggested that the CPUC audits could be more consistent and better
					targeted: “Moreover, the CPUC conducts audits to determine whether utilities are in compliance
					with rules designed to ensure that they are operating safely, but those audits could be improved
					to better ensure such compliance, thereby helping mitigate the risk of utility‑caused wildfires.
					Specifically, the CPUC does not consistently audit all areas in the utilities’ service territories,
					it did not audit several areas that include high fire-threat areas.”
				</li>
				<li>
					It also appears that the CPUC does not meaningfully issue penalties when it finds
					utilities are failing to execute their WMPs. The same <a
						href="https://www.auditor.ca.gov/pdfs/reports/2021-117.pdf">report</a
					>
					stated that the CPUC “does not use its authority to penalize utilities when its audits uncover
					violations.” The following bullet points from the same report provide examples (bolding by
					me).
					<ul>
						<li>
							“In 2014 the CPUC adopted an electric safety citation program that gave staff the
							authority to issue penalties for certain violations of law and of General Orders,
							including those identified through audits. <strong
								>However, as of November 2021, the CPUC had not issued any penalties resulting from
								violations that its safety and enforcement division found during audits.
							</strong>The safety and reliability program manager informed us that it is the CPUC’s
							practice to issue penalties for significant issues, which may be found through
							incident investigations where individuals were hurt or killed, or where buildings were
							destroyed, but that these types of immediate safety hazards are rarely found during
							audits.”
						</li>
						<li>
							“In our review of CPUC audits, we identified several instances where the CPUC
							identified violations of General Orders that were the same as those for which it
							issued penalties in incident investigations. For example, the CPUC issued a $2.5
							million penalty to a utility in 2021 for nearly 55,000 violations of a General Order
							requiring inspections of distribution poles, and we found that the CPUC had identified
							similar issues in at least two of its distribution district audits. The CPUC
							identified more than 200 violations of the same General Order in one 2020 distribution
							district audit, and about 2,400 similar violations in a second 2020 distribution
							district audit. Additionally, we found that in 2017 the CPUC issued a $50,000 penalty
							to a utility for a single violation of a General Order requiring vegetation
							management. <strong
								>Although we identified three audits that the CPUC performed in 2019 and 2020 that
								identified similar violations, it did not issue any penalties for those violations.</strong
							>”
						</li>
					</ul>
				</li>
			</div>
		</Bullet>

		<p class="mt-12">
			If you have any comments or questions about this case study, feel free to email me at <a
				href="mailto:coby.joseph@gmail.com">coby.joseph@gmail.com</a
			>.
		</p>

		<!-- You can continue adding more sections as needed -->
		<div class="h-[1px] w-[50%] bg-white mt-10" />

		<div class="mt-4 text-xs">
			<span id="fn1"
				>1: This case study focuses on safety standards on the three largest utilities and may not
				accurately represent standards applying to smaller utilities.<a
					href="#fnref1"
					title="Return to the text"
					rel="footnote">↩</a
				></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn2"
				>2: This may or may not be a parallel to the AI field in the future.<a
					href="#fnref2"
					title="Return to the text"
					rel="footnote">↩</a
				></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn3"
				>3: Katherine Blunt, California Burning, 2022. Page 268.<a
					href="#fnref3"
					title="Return to the text"
					rel="footnote">↩</a
				></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn4"
				>4: ibid. Page 230.<a href="#fnref4" title="Return to the text" rel="footnote">↩</a></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn5"
				>5: ibid. Page 211.<a href="#fnref5" title="Return to the text" rel="footnote">↩</a></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn6"
				>6: ibid. Page 211.<a href="#fnref6" title="Return to the text" rel="footnote">↩</a></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn7"
				>7: ibid. Page 100.<a href="#fnref7" title="Return to the text" rel="footnote">↩</a></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn8"
				>8: Available in the ‘Approved 2023 Executive Compensation Guidelines – 11/28/22’ accessible
				here<a href="#fnref8" title="Return to the text" rel="footnote">↩</a></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn9"
				>9: Katherine Blunt, California Burning, 2022. Page 188.<a
					href="#fnref9"
					title="Return to the text"
					rel="footnote">↩</a
				></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn10"
				>10: Available here, see Energy Safety’s 2020 Annual Reports on Compliance: PG&E – 2/24/23<a
					href="#fnref10"
					title="Return to the text"
					rel="footnote">↩</a
				></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn11"
				>11: As it would increase the utility’s risk of being unable to recover money from the
				California Wildfire Fund if it faced significant liability, likely raising its borrowing
				costs and increasing the risk of future bankruptcy, as indicated to me by experts. <a
					href="#fnref11"
					title="Return to the text"
					rel="footnote">↩</a
				></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn12"
				>12: “PG&E 2023-25 Wildfire Mitigation Plan Revision Notice – 6/22/23” available here<a
					href="#fnref12"
					title="Return to the text"
					rel="footnote">↩</a
				></span
			>
		</div>
		<div class="mt-4 text-xs">
			<span id="fn13"
				>13: Katherine Blunt, California Burning, 2022. Page 151.<a
					href="#fnref13"
					title="Return to the text"
					rel="footnote">↩</a
				></span
			>
		</div>
	</div>

	<div class="toc text-sm">
		<p class=" underline"><a href="#background">Background and overview</a></p>
		<p class="ml-5 mt-[0.5rem]"><a href="#contents">Contents</a></p>
		<p class="underline mt-3"><a href="#17">The need for safety standards</a></p>
		<p class="underline mt-3"><a href="#18">Current standards</a></p>
		<p class="ml-5 mt-[0.5rem]"><a href="#components">Wildfire Mitigation Plan components</a></p>

		<p class="underline mt-3"><a href="#19">Key takeaways</a></p>
		<p class="ml-5 mt-[0.5rem]"><a href="#20">Proactvity vs. reactivity</a></p>
		<p class="ml-10 mt-[0.5rem]"><a href="#evolution">The evolution of safety standards</a></p>
		<p class="ml-5 mt-[0.5rem]"><a href="#motives">Utility motives</a></p>

		<p class="ml-5 mt-[0.5rem]"><a href="#15">Activists and third parties</a></p>
		<p class="ml-5 mt-[0.5rem]">
			<a href="#regulation">Regulatory structure, processes, and challenges</a>
		</p>
		<p class="ml-5 mt-[0.5rem]"><a href="#16">Influence of voluntary safety actions</a></p>

		<p class="ml-5 mt-[0.5rem]"><a href="#risk">Risk assessment</a></p>
		<p class="ml-5 mt-[0.5rem]"><a href="#9">Audits and penalties</a></p>
	</div>
</div>

<style>
	a {
		color: #60a5fa;
	}

	p > a {
		color: white;
	}

	p > a:hover {
		color: #60a5fa;
	}

	.grid-container {
		display: grid;
		grid-template-columns: 1fr minmax(auto, 700px) 1fr; /* left, middle, right columns respectively */
		gap: 0px; /* This will create space between your content and the TOC */
		width: 100%;
		justify-content: center; /* This will center the entire grid layout */
	}

	.content {
		width: 100%; /* Let it occupy full width of its container (the middle column) */
		padding: 20px;
		box-sizing: border-box;
	}

	.toc {
		width: 300px;
		position: -webkit-sticky; /* For Safari */
		position: sticky;
		top: 20px;
		padding-top: 5px;
		padding-left: 10px;
		padding-right: 25px;
		box-sizing: border-box;
		max-height: calc(100vh - 40px);
		overflow-y: auto; /* Allows for scrolling inside TOC if it overflows */
	}

	/* Media Query for screens below 768px */
	@media (max-width: 900px) {
		.toc {
			display: none; /* Hide the TOC */
		}

		.grid-container {
			grid-template-columns: 1fr minmax(auto, 95%) 1fr; /* Adjust center column to 95% width */
		}
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
