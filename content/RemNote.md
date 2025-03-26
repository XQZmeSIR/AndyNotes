# RemNote

[[RemNote]] is a web-based [[Note-writing system]] with a structured knowledge model and first- class operations for adapting notes into a [[Spaced repetition memory system]], a la [[The mnemonic medium can be extended to one’s personal notes]].

Prior to a significant redesign in September 2021, it had a somewhat oppressively formal knowledge model, but I think the design’s new approach is pretty successful. It’s an outliner in which every node may contain flashcards. To create a flashcard, you either surround text with double-curly- brackets (a la Anki’s cloze deletion syntax), or insert `>>`, `<<`, `<>`, etc to make a forward, reverse, or double-sided flashcard.

You can make multi-line flashcards by using the outliner’s hierarchical structure. If the parent ends with a flashcard symbol (e.g. `>>`), the children are rendered as the “back.” This is a graceful way to repurpose existing primitives to achieve enhanced flexibility.

It still retains notions of “concepts” and “descriptors,” which are elements of the original knowledge model, but it seems these may be deprecated at this point.

It has some [[Transclusion]] features (“portals”), so that concept hierarchies can be composed into different “documents.” Like [[Roam Research]], the model encodes the belief that text blocks, structured in this model, can be made into reusable units. I’m worried about their composability: [[Transclusion is limited by the data model’s composability]].

* * *

Original author: {Martin Schnieder}

Design-focused co-founder joined in 2021: {Moritz Wallawitsch}

They raised a $2.8M seed round in summer 2021.
