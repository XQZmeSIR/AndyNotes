# Framing prompt generation as a filtering problem on reinforcement targets

When I started looking into [[Using machine learning to generate good spaced repetition prompts from explanatory text]], I thought of the problem mostly in terms of how to cause the system to produce the kinds of outputs I wanted. But having now experimented with some models, I notice that something much like the question I want is often produced by the model, if I’m willing to generate and evaluate enough samples. The trouble is that it may take quite a few samples… though not a Borgesian number. Obviously any sufficiently sophisticated model contains all sentences; I’m not making the trivial point that the prompt I want is in that set. The discard count may be closer to 10 ([[2023-06-14]]: this number was with GPT-3. With GPT-4, it’s lower…)

This is very different problem than the one of causing the model to produce an acceptable output at all ([[In prompt generation, choosing reinforcement targets and writing prompts for those targets are two separate problems]]). It may be possible to develop filters on the model’s output post-generation to focus on the types of questions we want. Alternately, perhaps we can develop an interface attuned to this filtering problem.

## On automatically ranking/filtering candidate prompts

What’s the nature of the “rejected” samples? I find that they’re usually not nonsense. They’re almost always well-formed questions, and they’re usually not unreasonable. They just lack any sense of understanding what’s interesting about a passage. Some of that is subjective—one person might be interested in who/what/when or key definitions while another is interested in big-picture implications ([[In prompt generation, LLMs often need extra hints about what angle to reinforce]]; [[In prompt generation, LLMs lack prompt-writing patterns for complex conceptual material]]). But I wonder if some of it is more objective.

For instance, if we’re generating questions from a passage about a runner, and there’s a phrase saying “he laced up his sneakers,” a question asking “What did he lace up before running?” can be thought of as somewhat objectively bad. It’s bad in part because almost any other runner in any other modern story would have done the same (i.e. this information is low-entropy). More subtly, it’s bad because this detail _isn’t important_ to this particular story. His shoes aren’t significant; they’re not mentioned again. I can imagine quantifying the former, but I’m not sure about how to quantify the latter. One dumb idea: if you remove the source detail, how much is the autoencoded vector for the passage displaced? Can we use the model’s sense of entropy here?

## References

Realized this during my [[2021-09-06]] call with [[Yuval Milo]]
