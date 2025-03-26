# Briggs, J., Kodnani, D., Hatzius, J., & Pierdomenico, G. (2023). Large Effects of Artificial Intelligence on Economic Growth. Goldman Sachs.

[[Will generative AI cause catastrophic economic dislocation?]]

> Using data on occupational tasks in both the US and Europe, we find that > roughly two-thirds of current jobs are exposed to some degree of AI > automation, and that ==generative AI could substitute up to one-fourth of > current work==. Extrapolating our estimates globally suggests that > generative AI could expose the equivalent of 300 mn full-time jobs to > automation.

Some high level questions I have after reading this:

  * What are the personal costs of tech-induced displacement? That is, if it _eventually_ leads to re-employment in a new job, how long is the person unemployed? What losses do they experience? How might we subsidize these harms?
  * Acemoglu/Restropo claim that worker displacement from automation has been greater than creation of new roles since the 1980’s. How does this actually manifest? Do more people become homemakers as a result? Retire early?
    * It does look like unemployment roughly doubled around the 80’s. Hm.
  * How does the estimated 7% displacement relate to the displacement attributable by, say, the personal computer?
    * Eyeballing exhibit 11, it looks like the marginal impact of IT might be around 4-5% displacement.
  * At what level on these O*NET scales might GPT-4 already be at?
  * In these charts, it took 20 years to really see the economic impact of electric motors and personal computers.
    * Do we expect to see such a long period from the invention of, say, ChatGPT? What is the relevant “invention start point”? ImageNet? Transformers? Hard to say. 
    * Job displacement and new job opportunities presumably won’t occur at the same rate. What’s the lag? What was the lag historically?

## CDF of generative AI workload exposure

![](FCB7DB03-6623-49C5-B0DC-A36D3E586CCA.png)

## Impact by industry

Q. How do the authors assess the effects of generative AI on a given job? A. They get a list of “work activities” involved in the job from O*NET, and compare those to a list of activities which they believe will be automated.

Q. How do the authors account for the capability level of the generative model in their impact estimates? A. The O*NET work activities are specified at different “levels” for each occupation, and the model is assumed to be able to only perform tasks up to a certain level (4/7 for the baseline case).

Q. Give two examples of an O*NET “work activities” which the authors believe will be automated. A. e.g. getting information, monitoring processes, identifying objects/actions, estimating characteristics, processing information, evaluating information for compliance, analyzing data, updating and using relevant knowledge, scheduling work, organizing/planning/prioritizing work, documenting information, interpreting information, admin activities

Q. Give the authors’ O*NET example tasks for the “getting information” work activity, at difficulty levels 2, 4, and 6. A. 2: follow a blueprint; 4: review a budget; 6: study international tax law

One thing that seems confusing about their methodology here is that ONET says that e.g. a “market research analyst” needs to perform “getting information” at “level 5.35”. Under the authors’ assumptions, this work wouldn’t be substituted by AI. But surely not _all_ of the getting-information-work must be done at that level. Probably some big chunk of it is a lower level and _can_ be automated, right? So you’d maybe still need someone for the most important part, but a large team could perhaps become a small one. This would suggest they’re under-estimating. But it’s not to me what they mean when they say they’re taking an “importance and complexity-weighted average of essential work tasks.”

![](80914C2B-A437-4987-B5D8-61CB95F36CB5.png)

Q. Top 3 US industries estimated to be impacted by generative AI, by share of workload? A. Office/admin support (46%); legal (44%); architecture and engineering (37%)

Q. Bottom 3 US industries estimated to be impacted by generative AI, by share of workload? A. Construction/extraction (6%); installation/maintenance/repair (4%); cleaning/maintenance (1%)

Q. Analysts’ estimate for % of workload replaced by generative AI, in US / Europe? A. 25%

Q. Analysts’ estimate for % of workload replaced by generative AI, globally? A. 18%

### Within-industry breakdown by exposure level

![](7A52FE20-1E2F-44D9-B24B-9197C1143537.png)

Q. How did the analysts’ model decide whether a job would be replaced rather than complemented by generative AI? A. Substituted when 50%+ of tasks of that job can be automated (importance/complexity-weighted); complemented when 10-49% can.

Q. Top 3 US industries most likely to have jobs replaced by generative AI? A. Legal (~40%); office/admin (~35%); architecture and engineering (~10%)

Q. Analysts’ estimate for % of US legal jobs replaced by generative AI? A. ~40%

Q. Analysts’ estimate for % of US office/admin support jobs replaced by generative AI? A. ~35%

Q. Analysts’ estimate for % of US workforce _substituted_ by generative AI? A. 7% (~11M people)

Q. Roughly how many unemployed Americans are there? A. ~6M looking for a job; another ~5M not looking but report wanting a job (March, 2023 [[USBLS]])

Q. Analysts’ estimate for % of US workforce _complemented_ by generative AI? A. 63%

Q. Analysts’ estimate for % of US workforce _unaffected_ by generative AI? A. 30%

Q. Summarize analysts’ assessment of the high-level impact of generative AI on the US labor market? A. Substantial majority of jobs complemented by generative AI (63%); relatively small share (7%) likely to be substituted.

I’m really interested in some model of: how might each occupational workload _evolve_ in response to partial labor savings?

## Sensitivity to generative AI capacity

“Much less powerful”: 2/7; “much more powerful”: 6/7 on O*NET scale (compared to baseline 4). ![](8D7AAE16-A2A6-43D6-B322-5AB8394B664F.png)

Q. Analysts’ estimated change in employment exposure as generative AI becomes more powerful? A. Little impact with increased capability until integrated with robotics, then big jump (25% -> 27% -> 35%)

Q. Analysts’ estimated change in employment exposure if generative AI is weaker than predicted? A. Impact may be roughly halved if generative AI is much less powerful than imagined (25% -> 14%)

## Impact on productivity growth

![](B1C620C8-7197-4F28-8D66-2A1E1863EB34.png)

I don’t think I follow this. If 30% of a worker’s complexity/importance- weighted tasks are replaced by AI, how is it that their productivity growth is only a few pp? Are they working fewer hours?

I’ll need to dig into the cited papers to understand, I guess.

Q. When did the labor productivity boom caused by electricity and personal computing occur, relative to their invention? A. ~20 years later, when ~half of business had adopted.

![](74B6B898-6CB8-4A50-8C54-E97F2E233DED.png)

Q. Analysts’ “baseline” estimate of the effect of generative AI adoption on annual US labor productivity growth, over a 10-year adoption period? A. 1.3%

Q. Analysts’ range of estimates of the effect of generative AI adoption on annual US labor productivity growth, over a 10-year adoption period? A. 0.3% (much less powerful AI) - 2.9% (much more powerful AI)

Q. Analysts’ estimate of the effect of generative AI adoption on annual _global_ labor productivity growth, over a 10-year adoption period? A. 1.4%

Q. Analysts’ estimate of the effect of generative AI adoption on annual global GDP? A. 7% increase over 10 years

## Re-employment

The authors anticipate that “many workers that are displaced by AI automation will eventually become reemployed—and therefore boost total output—in new occupations that emerge either directly from AI adoption or in response to the higher level of aggregate and labor demand generated by the productivity boost from non-displaced workers.” Let’s hope so! How should we reason about this?

Q. The authors argue that IT automation-driven job displacement was compensated by reemployment in what two ways? A. New occupations (web designers, digital marketers); and more service sector job demand (health care, education, food service) due to increased aggregate income.

Q. Argument from Autor et al (2022) that technological innovation drives long- term employment growth? A. Census data suggest that 60% of workers today are employed in occupations that didn’t exist in 1940.

Q. Big-picture finding from Acemoglu and Restrepo (2019) on technology-driven job displacement? A. Technological change displaced workers faster than it created new jobs since the 1980s (roughly the IT automation boom). Those rates were roughly equal from 1950 until then.
