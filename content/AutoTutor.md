# AutoTutor

A family of natural dialogue-based [[Intelligent tutoring system]] initially developed by Arthur Graessler but later expanded into many variations by other researchers. These systems frame their ambition as attempting to simulate a human tutor; the initial designs were created to imitate conversational forms and moves observed in a pool of human tutors. Unlike [[John Anderson]]’s systems, which emphasize problem-solving, these dialogues mostly focus on explanation, implication, inference, and so on.

In most implementations of AutoTutor, each task includes a main question, a glossary of related concepts, a set of expected response elements, anticipated misconceptions, and “a space of discourse moves needed during the conversation (e.g., corrections for misconceptions, answers for definitional questions, hints, hint completions, prompts, prompt completions, a summary).” The conversation is guided by LSA: students’ responses are checked against the expectations; when elements are missing, a cycle of pumping, hinting, prompting, and asserting is triggered.

Q. What’s the 5-step tutoring frame used by AutoTutor? A. 1. tutor poses question; 2. student attempts; 3. tutor provides feedback; 4. collaborative improvement of response; 5. final check for understanding

![](FF2A1CC9-470F-413D-8FCA-39E9F89FEE5C.png) ![](E29FF6A0-3A0F-4D8B-97F0-ED85D7801CDF.png)

![](F3BFD630-9077-4A3E-8359-6A07C81F145C.png)

  * [[Video of 2008-era computer literacy AutoTutor]]
  * [[Video of 2015-era CSAL AutoTutor used for adult literacy, which adds multiple choice input and trialogues to AutoTutor’s traditional free input dialogues]]
  * [[Video for 2020-era “AutoTutor Read” for adult literacy]] (quite similar to 2015 tool)
  * [[Index of live demos]]
    * [[Live demo of adult literacy AutoTutor]]

## Impressions

My sense is that the explicit systems around detecting and choosing conversational moves will mostly give way to prompt engineering in an era of [[Large language models]]. AutoTutor implementations have mostly used pre-deep-learning strategies for modeling students; responses are mostly canned. Yet there are important structural insights captured in the tutoring methods specified by the architecture here. It’s interesting to consider how the tutoring insights represented by AutoTutor’s approach might be translated to a more versatile LLM-based implementation.

For example, one strategy “encouraged students to generate questions for the tutor to answer, which correlates with learning and can improve meta-cognitive skills. Unfortunately, AutoTutor was not capable of answering all student questions so this strategy was not feasible.” (Nye, 2014). Presumably student questions can now be answered with some reliability.

My subjective impression, at the visceral experience level, is one of repulsion: the sluggish synthesized voices and 3D faces are appalling; the scripts are condescending and unmotivated (“I am happy you have decided to join me in learning to be a better reader”); the UI is unskillfully executed. These systems are mostly developed by people in psych departments, not HCI, to be fair. But the underlying edpsych ideas seem well-grounded. Maybe an experience-centric approach could generate something interesting here.

## References

  * Graesser, A. C., Lu, S., Jackson, G. T., Mitchell, H. H., Ventura, M., Olney, A., & Louwerse, M. M. (2004). AutoTutor: A tutor with dialogue in natural language. Behavior Research Methods, Instruments, & Computers, 36(2), 180–192. <https://doi.org/10.3758/BF03195563>
  * Nye, B. D., Graesser, A. C., & Hu, X. (2014). AutoTutor and Family: A Review of 17 Years of Natural Language Tutoring. International Journal of Artificial Intelligence in Education, 24(4), 427–469. <https://doi.org/10.1007/s40593-014-0029-5>
