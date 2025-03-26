# Reading comprehension questions can uncover textbase holes

I was embarrassed to find ([[2023-09-11]]) that when I asked [[Large language models]] to generate reading comprehension questions to help me assess the textbase (see [[Construction-integration model]]) I’d constructed for a section in [[Linear Algebra - Hefferon]], several of the questions revealed sections of the text that I hadn’t processed at all. Even though I was trying to read somewhat carefully.

[[Reading comprehension questions are unpleasant]], and these were no exception. I added some notes there about the trouble I noticed this time:

> Unfortunately, this is _especially_ true when the question pertains to > material which I failed to process. The question just won’t seem to make > much sense. I can tell that it’s asking me to produce some particular > answer, but I can’t tell what kind of thing it’s looking for (because I > never encoded the requisite information). So the question sends me on a wild > goose chase of sorts, in which I flip back through the chapter looking for > some passage which pattern-matches to terms in the question. Then I realize > that I hadn’t really read the passage at all, and I may see what the > questions asking… but it’s an ungraceful way to get there.

It’s interesting that the mechanism here is indirect: I often don’t really understand quite what the question is asking when it uncovers a reading comprehension failure. But the confusion makes me re-read, looking for something which might help, and that process ends up filling my comprehension gap.

Presumably reading comprehension questions can also uncover holes in my situation model (see [[Construction-integration model]]), but I have less immediate experience of that. It’s more common for me to notice those holes through more elaborate tasks which require inference (i.e. [[Transfer learning]]). When failures arise in those tasks, while the textbase appears to be solid, it seems difficult to determine where the situation model has broken down.

See also, in the context of the [[Mnemonic medium]]: [[Interleaved mnemonic medium prompts uncover reading comprehension lapses, sometimes unpleasantly]]
