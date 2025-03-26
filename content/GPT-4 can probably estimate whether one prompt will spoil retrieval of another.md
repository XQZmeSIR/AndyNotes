# GPT-4 can probably estimate whether one prompt will spoil retrieval of another

One low-priority challenge for orchestration of [[Spaced repetition memory system]] sessions is [[Spaced repetition memory prompts should encode ideas from multiple angles]], but often that means that practicing one prompt will “give away” the answer to another. The most trivial instances of this are “reverse” prompts (“The wave function is notated as…? $\Psi$; What does $\Psi$ denote in QM? The wave function.”) and prompts with multiple independent [[Cloze deletion]] regions. SRSs can sometimes special-case those instances. But it’s a general problem. Often it seems like it would really be best if a “cluster” of prompts about a single idea were always smeared out onto consecutive days, or at least separated by several minutes within a single session.

Some quick experiments with [[GPT-4]] suggest that it can probably classify reasonably accurately whether two prompts “conflict” in this way. We could use this to “spread out” very similar prompts.

## Related

  * [[2023-05-31 Patreon letter - Fluid practice for fluid understanding]]
    * more discussion of the problems of “clusters” of related prompts
  * Pattern matching
    * [[Spaced repetition memory prompts should be written to discourage shallow “pattern matching”]]
    * [[Is there a way to detect spaced repetition memory prompts which are likely to be answered through pattern matching?]]
