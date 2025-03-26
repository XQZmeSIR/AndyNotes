# In prompt generation, LLMs often need extra hints about what angle to reinforce

In the problem of [[Using machine learning to generate good spaced repetition prompts from explanatory text]], it’s often not enough to give a model a text passage and a highlighted range. There are often so many things one _could_ reinforce about a phrase of explanatory text: a declarative detail, why it’s true, its implications, its contrast to an earlier statement, etc. Many very different good prompts _could_ be written. The model doesn’t know which you want ([[In prompt generation, choosing reinforcement targets and writing prompts for those targets are two separate problems]]).

But I get much better results if I give the model a word or two hinting at what _aspect_ of the phrase I want to reinforce. Interface-wise, this might look a bit like: highlighting something you find important, then scribbling “why” above it. Or a little note to yourself: “this is much higher than I thought.”

For example, reading Griffiths’ Introduction to Quantum Mechanics, I was surprised by the usage of $V$ as notation for potential energy—I’m used to $U$. I wanted a prompt about that. But if I just highlight the $V$ in the phrase “the force can be expressed as the derivative of a potential energy function, 1 F = −∂ V /∂ x”, I get “What is the relationship between force and potential energy in conservative systems?”. This isn’t terribly surprising. How could it know that my issue was that the notation was surprising to me? By contrast, if I ask the model to emphasize “notation”, I get “In the context of classical mechanics, what does the symbol “V” represent?”

So far, I’ve found that hints are only consistently unnecessary when reinforcing simple statements of fact. (“Carbon’s atomic number is 6.”)

## Personal connection; personal notes

One fundamental issue here is that the best prompts often involve making the material personally meaningful—connecting some abstract information to a goal you have, or honing in on a detail or angle you find particularly striking, but which the author doesn’t emphasize. A model can’t easily know these things.

One approach that might help is to also generate prompts from one’s notes about a text.
