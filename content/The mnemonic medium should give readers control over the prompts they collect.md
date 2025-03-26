# The mnemonic medium should give readers control over the prompts they collect

[[The initial mnemonic medium is implicitly authoritarian in premise]]. These mechanics:

  * discourage/prevent many valuable active modes of reading, e.g. skimming for gems, reading with a specific purpose in mind motivated by authentic use, reading non-linearly, etc: [[The best way to read is highly contextual]]
  * encourage a passive mental posture—the reader’s along for the ride, contra [[Do your own thinking]], the active choice implied by [[Spaced repetition memory systems make memory a choice]]
  * create a school-style learning aesthetic, in practical misalignment with [[Orbit - Values]], e.g. “helps you deepen your relationship with whatever you care about most … it’s for ideas and imagery that you could talk about all night … not for things you think you “should” be engaged with … not “educational” in tone”
  * create active frustration when a prompt seems poorly-written or non-meaningful; see e.g. [[Mnemonic medium readers sometimes feel impeded by authors’ wording choices]], [[Cloze deletions often create frustrations in non-technical mnemonic texts]]
  * impede fluid interaction between the medium and the rest of the reader’s knowledge work, unlike e.g. [[The mnemonic medium can be extended to one’s personal notes]]
  * create the (correct but bad) sense that the prompts aren’t “yours”, material to be deployed as you see fit; instead, you’re visiting a museum created by the author, and everything is under glass
  * make it harder to use the medium as a scaffold to learn to write your own prompts ([[The mnemonic medium may help scaffold prompt-writing through author-provided prompts]])
  * discourage [[the essential practice of iterative refactoring]] (which spaced repetition systems systematically under-value, in general)

## Forward directions

I’d like to swing the vibe aggressively more in the reader-centric direction. This will be tough to do while maintaining other important properties of the medium. Expert-authored prompts really do contribute a great deal of value ([[The mnemonic medium supplies expert-authored prompts to remove the burden of prompt-writing]]). We want to reap that value (or perhaps even enhance it!) while also providing fluidity, _malleability_.

There are some relatively simple ways we might begin: readers should be able to disable or skip prompts that don’t resonate; readers should be able to make simple edits to authors’ wording; the embedded interface shouldn’t discourage people from reviewing only part of a page. All this will generate interesting signal for authors: [[The mnemonic medium can generate interesting author analytics]]

But I think we’ll have to go deeper than this. A few directions I find promising, which of course need to be fleshed out more thoroughly:

  * You should be able to fluidly move between consuming a prompt, to editing its text, to refactoring it (one-to-many) and its adjacent author-provided prompts (many-to-one), to writing new prompts of your own inspired by those prompts.
    * Ideally, this same interaction model should extend to the review experience: as you’re reviewing, if you think of a way to improve a prompt, or you’re reminded of a new prompt you want to write, that should be just as fluid.
  * We should explore pick-and-choose modalities for ingesting prompts from the text. Imagine that as you read, some phrases are highlighted in a special way indicating that the author has provided prompts representing that idea. If you find something interesting, you can click on the highlighted text—and boom, now you’ll remember it forever.
    * We’d want the same fluid consuming-to-editing interactions for this type of prompt.
    * This type of interaction points the way to crowdsourced annotations, ML-generated prompts, etc. More generally: imagine if you could point at any idea you found interesting, anywhere, and feel assured that now you’ll remember it (and ideally deeply internalize it) for the long term.
    * [[Ozzie Kirkby]] suggests that there may be some interesting middle ground here which would encourage readers to write their own prompts representing the details they find interesting: maybe authors (or ML, or the system) can provide partial/“starter” templates for key text regions, which the user would adapt/complete as they see fit.
  * The presentation and interactions should make it very clear that your collection of prompts is _yours_ , even if you’re working with author-provided prompts. [[Taylor Rogalski]] points out a helpful analogy to making a copy of a Google Doc to scribble all over it.
  * We can start to experiment with fluid interaction between the medium and the rest of the reader’s knowledge work by fleshing out [[My implementation of a personal mnemonic medium]]. That direction is really not quite the same as what the rest of this note is talking about: I’m not sure how author-provided prompts interact with this kind of note-taking. So maybe it’s a red herring… but my instinct is that it’ll be instructive, and that all this work is intertwined.
  * I suspect this work will inform and intersect with the design of a “library view” in the Orbit app itself. One related priority for me here is to fuzz the “boundaries” between prompts; see discussion in “How to write good prompts” [[here]], grep (“revision is a holistic endeavor”). This also means fuzzing the boundaries between the author’s prompts and the user’s prompts. We should probably avoid paradigms which put those sets in separate conceptual “places”—but I expect we’ll still want some affordances showing provenance.

==TODO much of this section should be fleshed out in more elaborate separate notes==

## References

I notice that there’s a connection here with the ideas in [[Heer, J. (2019). Agency plus automation: Designing artificial intelligence into interactive systems. Proceedings of the National Academy of Sciences, 116(6), 1844–1850]]: just as a collaborative human/AI interface requires a coextensive data canvas, a collaborative human/author interface requires something similar.

See notes from [[Yusuf Ahmad]] on this tension, which he frames as a gulf between “industrial” educational architectures and social constructivist architectures: <https://www.notion.so/Placing-Cog-Sci-ideas- within-a-broader-Learning-Architecture-fa69fc15ba9e41b8a2e136f7fbe0362b>

Q. Unexpected connection between the [[Mnemonic medium]] and [[Heer, J. (2019). Agency plus automation: Designing artificial intelligence into interactive systems. Proceedings of the National Academy of Sciences, 116(6), 1844–1850]]._Agency_plus_automation%3A_Designing_artificial_intelligence_into_interactive_systems._Proceedings_of_the_National_Academy_of_Sciences%2C_116\(6\)%2C_1844%E2%80%931850)? A. Just as a collaborative human/AI interface requires a coextensive data canvas, a collaborative human/author interface requires something similar.
