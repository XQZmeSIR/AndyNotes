# In prompt generation, LLMs lack prompt-writing patterns for complex conceptual material

I’ve had some success in [[Using machine learning to generate good spaced repetition prompts from explanatory text]] for simple declarative knowledge ([[GPT-4 can often generate usable spaced repetition prompts for declarative knowledge from explanatory text with guidance]]), but much less for more complex conceptual material. The problem here is not exactly that the system generates “bad” prompts (at least with [[In prompt generation, LLMs may perform better when given prompt-writing principles]]); it’s more that the resulting prompts just reinforce the surface—what is said, rather than what it _means_ or why it matters (to riff on [[How to Read a Book - Adler and van Doren]]).

To take an extremely simple example, from Hefferon’s Linear Algebra, consider definition 1.10:

> A system is in _echelon form_ if each leading variable is to the right of > the leading variable in the row above it, except for the leading variable in > the first row, and any rows with all-zero coefficients are at the bottom.

The LLM will generate questions about the _term_ , like:

  * “What properties must a linear system have to be in echelon form?”
    * (term -> definition)
  * “What do we call a system where each leading variable is to the right of the leading variable in the row above it, except for the leading variable in the first row, and any rows with all-zero coefficients are at the bottom?”
    * (definition -> term)

But these questions reinforce information, not understanding. My manually written questions would also include:

  * “Is this linear system in echelon form? Why or why not? <example>”
    * (example -> classification)
  * “Give an example of a linear system in echelon form.”
    * (classification -> example)
    * Also: “Give an example of a linear system which is _not_ in echelon form.”
  * “How can one put a linear system into echelon form (if it is possible)?”
    * (connection to other concepts)
    * In this case, Gauss’s Method had just been introduced, so the connection is only _implied_ in the book’s text)
    * And probably some light problem solving practice: “Put this system into echelon form (if possible): <example>”.
  * Lots of questions about the _purpose_ of the concept; e.g.:
    * “What does echelon form quickly show us about a linear system’s solution set?”
    * "How can echelon form show whether an equation of a linear system is redundant?”
    * “What will the echelon form of a linear system with multiple solutions look like? Explain with an example.”
    * … and so on. These details appear on the next few pages, and so one might think of them as _separate_ ideas, which could be separately highlighted and reinforced. But I guess the point I’m making here is that I wouldn’t want to add prompts about the definition _without_ adding prompts like this; as a reader, I’d have added a mental “TODO” when seeing the definition if I didn’t know how to ask these questions yet, and I’d be on the hunt for these details. But the model doesn’t know to do this, at least without further guidance.

This shouldn’t be terribly surprising. The training set isn’t going to include lots of flashcards breaking down complex conceptual topics; that’s an unusual thing to do. In my brief exercises thus far, the language model can generate these sorts of more elaborated prompts if I provide a lot of guidance, but a simple hint doesn’t suffice (as in [[In prompt generation, LLMs often need extra hints about what angle to reinforce]]). For example, I didn’t have success with just the hint that I want prompts about “applying the concept to examples”; I have to say “Generate an example linear system and ask whether it’s in echelon form.” The notion of asking about examples as a strategy to understand concepts, is apparently not highly salient to the model, at least in the context of writing spaced repetition prompts.

[[A pattern language of prompt-writing]] could probably give the models enough guidance to do a much better job.
