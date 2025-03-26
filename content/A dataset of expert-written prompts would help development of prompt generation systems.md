# A dataset of expert-written prompts would help development of prompt generation systems

So far in my experiments with [[Using machine learning to generate good spaced repetition prompts from explanatory text]], I’ve done a lot of casual, one-off evaluations. That’s fine in the tinkering phase, but if I get more serious here, I’ll want a dataset of “known-good” prompts which can be used to evaluate various ML-driven applications.

In the past year or so, I’ve done a bunch of adaptations of sections of textbooks (e.g. from [[University Physics - Young and Freedman]]). These would make good sources, although it’s a shame the relevant textbooks are copyright encumbered. It’d be better to do this exercise with an open textbook of some kind. (e.g. maybe one of Hefferon’s?)

## Pipeline from my own prompt stream?

For that matter, now that I’m using [[Hypothes.is]] and my own prototype to do much of my prompt-writing about explanatory text, I should consider creating a pipeline which automatically attempts to generate prompts from the same highlights in the same textual context. I can evaluate them with [[GPT-4 can probably estimate whether two flashcards are functionally equivalent]] (assuming I get that to work). It’ll also help me determine how often it’s true that [[In prompt generation, LLMs often need extra hints about what angle to reinforce]], since these prompts won’t have those special annotations.
