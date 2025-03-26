# Idea-centric memory system

In a [[Spaced repetition memory system]], the central noun is the prompt—a task constructed to promote [[Retrieval practice]] or to produce the [[Testing effect]]. But I’m interested in exploring an alternative formulation in which _ideas_ are the core noun, or at least exist alongside prompts. To put this another way: to put something into a memory system right now, you encode it into prompts and tasks. What if, instead, you could put _the thing itself_ into the memory system? And then, when you show up for your daily review sessions, you’d be presented with activities which reinforce and deepen those things?

This notion is typically discussed in the context of _automation_ : good memory prompts are hard to write; it takes too long; wouldn’t it be nice if you could make the computer do that work? But let’s leave efficiency and convenience aside for a moment; I think there are more central reasons to consider “the thing itself” as the natural primitive:

  *  **Avoid pattern matching:** One problem for memory system prompts is that often we learn to pattern match responses to prompts based on shallow surface features ([[Spaced repetition memory prompts should be written to discourage shallow “pattern matching”]]). It’s hard to escape from this within the static nature of a prompt.
    * [[GPT-3 can generate shallow variations of spaced repetition prompt questions]], but variations generated from a specific prompt might be narrower than those generated from the idea which gave rise to the prompt.
    * Pattern matching is also bad emotionally; it damages my faith in the system, makes me feel like I’m doing busywork, and puts me into a rote state of mind.
  *  **Multi-angle encodings:** Surface-level variation aside, prompts tend to produce a narrow kind of reinforcement. When I try to work with information I reinforce with memory systems, it often feels like I have to “search my mind” in just the right way—find a very specific key to unlock that knowledge. By contrast, I understand important ideas in programming from a hundred different angles, so I rarely feel like I have to find the right key; the ideas always feel ready at hand in any given situation.
    * All this is why we advise that [[Spaced repetition memory prompts should encode ideas from multiple angles]]. But in practice, this often feels like an abuse of the system:
    * The prompts representing the different angles are totally independent, so you get asked about the same idea from many different angles in the same session. For the latter angles, you won’t have to retrieve the information from long term memory, and this likely diminishes reinforcement.
      * Also, answering half a dozen questions which are all really about the same idea back to back often feels obnoxious or boring.
      * I’d rather smear highly related questions out over several days, so that they unfold in time.
    * If I mark a prompt about one of the angles as difficult, shouldn’t that affect the schedules of the other angles?
    * Organizationally, it’s annoying that these prompts are presented as separate entities within the library; they’re really just many sides of the same coin, but (especially if you write them at different times) there’s no way to view them as a group.
    * [[Pan, S. C., & Rickard, T. C. (2018). Transfer of test-enhanced learning: Meta-analytic review and synthesis. Psychological Bulletin, 144(7), 710–756]] find that transfer is much more likely when “response congruency” is present—that is, the answer to the transfer question substantially overlaps with the answer which was practiced. This suggests that, to get good coverage for transfer, we also want multiple angles on the _answers_ , not just on the questions.
    * Hm. Not sure this belongs here, or that I trust it. Practically speaking, high response congruency studies were mostly those about rote recall; low response congruency studies were mostly about problem solving practice, application, and inference questions. So their response congruency codes might “really” correspond to, say, increased complexity, or to more distant transfer.
  *  **Pointing at the thing itself:** My concrete emotional experience is: I hear or read or think something that excites me. I think, “ah! I want to bring this into my practice!” But I can’t quite bring “this” into my memory practice; I have to find a way to transform it into some other object which I can bring into my practice. Sometimes, that transformation task is a welcome exercise—bringing me closer to the idea that stimulated me, helping me pick it apart and understand it better. But the vast majority of the time, it just feels like a burden.
    * (see [[2022-10-14 Patreon letter - Lessons from summer 2022’s mnemonic medium prototype]] for more)
    * I want to emphasize that this impulse is _not_ about efficiency or “lowering the floor.” It’s about making the core verb _feel_ better—making it more naturally aligned with my internal intent and my emotional interest. Removing a friction which often alienates me from the process.
    * Related: [[Deciding to remember something with a spaced repetition system is (aspirationally) a lightweight gesture]]
    * It seems pretty obvious to me that this is the conceptual model we’d have used from the start if it were possible… the trouble is that _it doesn’t work!_ [[Readwise]]-like systems which just resurface the idea itself as the practice session don’t produce a [[Testing effect]], and few people seem to stick with it. I haven’t used [[Kawara]] much, or interviewed its users, but I suspect it would have the same problem.
    * Notice that this is also closer to what’s happening in the places where memory systems find themselves most pervasively and naturally used: language learning and medical school.
    * i.e. in language learning, prompts usually are _words themselves_ —the raw thing you’re trying to learn. In medicine, a common prompt would be an anatomy diagram with one label blanked out. Again, the prompt is the thing itself. The task is implicit. If you see a flashcard with an Italian word on it, you know you’re supposed to give its English translation. If you see a diagram with a blanked-out label, you know you’re supposed to provide it.
    * I think this also explains some of the attraction of [[Cloze deletion]].
    * This is a more natural way to implement something like [[The mnemonic medium can be extended to one’s personal notes]]. In practice, I find that I’ll often make a note of something I find interesting in a paper, then I’ll repeat that idea in a couple of differently-phrased prompts, then I’ll continue with the prose note. This feels disjointed and repetitive, and it makes for notes which are unpleasant to read. Maybe the solution is better folding affordances; but it feels to me that the more natural conceptual design would be to let the insight itself be the object of practice.
    * “bringing ideas into your Orbit”—not “awkwardly transforming ideas into tasks and bringing those into your Orbit”
  *  **Deepening over time:** present-day memory systems let me save a lossy snapshot of my understanding at the time I wrote some prompts about a particular topic. It’s about preservation, maintenance. But a more powerful frame is connection and depth, rather than mere preservation, as [[Michael Nielsen]] has pointed out (e.g. in [[Building a better memory system - Michael Nielsen]]). It would be much more interesting and much more valuable to use that review session time to think new thoughts about the material, to push it further, to notice new connections, to reconnect with it emotionally.
    * It’s possible to do this with prompts ([[Spaced repetition memory systems can be used to prompt application, synthesis, and creation]]), but it’s often difficult or awkward to write such prompts for yourself. You want to give yourself new tasks each time, to push yourself to think new thoughts. Practically speaking, you’re forced to write highly general prompts (“Think of a new way to apply advice X in your life…”). I often find these sorts of prompts pretty difficult to emotionally connect to during review. I think it would be better to work with a large variety of more concrete tasks, but it’s tough to execute that practically with a prompt-centric conceptual design.
    * Static prompts can’t naturally specify an arc or progression. As a motivating example: If I’m learning about some new concepts in physics, I’d probably like to start with basic reading comprehension checks, and by making sure I know their definitions and notations; then once those are solid, I’d like to practice applying them in simple ways individually; then in combination; then perhaps using them to make longer inferences.
    * Another more classic recall-centric example: if I’m trying to remember a poem, I might begin by completing couplets, then once those are solid, progressing to stanzas, and so on.
    * Another way to look at this is that I’d like to find systematic ways to use my practice sessions to increase my chunk size.
  *  **Emphasizing problem-solving practice:** another way to look at the last point is that I’m interested in finding ways to use my practice time for problem-solving practice. The problems should vary; they should become more complex over time.
    * Ideally, these tasks could be done without pen and paper, so that I could integrate them into my normal smartphone review sessions. Maybe it’s enough to just “set up” problems?
    * A good early “step” might be to complete steps of worked examples (see [[Worked example effect]] literature… presumably people have looked at the effects of this as a task?)
  *  **Easier shared language for mnemonic medium reader preferences?** as described in [[2022-10-14 Patreon letter - Lessons from summer 2022’s mnemonic medium prototype]], people don’t really want to evaluate prompts—i.e. “should I save this one?”; they want to point to passages of the text which seemed most important.
    * The mnemonic medium needs an affordance for expressing the desired level of depth to be learned. It makes more sense to specify or control this on an idea level than on a per-prompt level.
    * (But it likely makes more sense to control this on a chapter / section level than an idea level)
    * If a reader doesn’t like a prompt they’re being asked to answer, they’d probably like the ability to defer/delete all related prompts about that idea.

## How to implement this?

In its most general form, we’re talking about a system which can facilitate practice sessions by selecting the most appropriate ideas to practice and providing appropriate activities.

In the case of the [[Mnemonic medium]], this might mean a static library of activities or activity templates provided by the author. In the case of a more general system, this task probably requires some kind of generative AI (i.e. [[Large language models]]); see [[Using machine learning to generate good spaced repetition prompts from explanatory text]]. Challenges abound there.

I guess I’m proposing something like:

  * a high-level language for specifying material to be reviewed
    * … which may approach straightforward natural language, given [[Large language models]]
  * a pattern language of practice/review/reinforcement activities
    * … which may take the form of fine-tuning or prompt engineering

## What’s the chunk size?

One thing that’s good about prompts-as-tasks is that they have a relatively clear natural chunk size. Novices do have trouble learning what that chunk size should be, but I think one can get a sense of it relatively quickly. Not so for ideas as the natural primitive. How complex should the idea be? Hm.

I notice that in practice, when I look at, say, [[University Physics - Young and Freedman]], and try to pull out “an idea” which might be converted into prompts, I’m pretty dissatisfied. For example, consider: “Two positive charges or two negative charges repel each other. A positive charge and a negative charge attract each other.” OK… this is part of the idea of charge. There are two kinds of charge. What distinguishes the two kinds is exactly this property. And, in fact, nothing else distinguishes them. So… what kinds of questions might one ask about this idea?

  * (predicate -> consequence) Two negatively charged particles are placed near each other. What will happen?
  * (consequence -> predicate) When will a pair of charges repel each other? Attract each other?
  * (application) If you place a proton next to an electron, how will they affect each other?
  * (application) If you want to attract positive charges to a particular point, what kind of charge should you place there?

These questions are sort of fine, as a starting point… but they’re too isolated, I think. You want this idea to interact with the idea of “proton” and “electron” and “conductor” and so on, in increasingly complicated ways.

## Finding a better word than “idea”

“Idea” doesn’t _quite_ capture what I mean. Some things which I might want to bring into my daily sessions which don’t quite fall under the term “idea”:

  * a beautiful piece of poetry
  * a striking dish
  * the way a conversation made me feel
  * the implicit value system suggested by an essay
  * an unusual behavior a person has

Some alternative concept-words to consider:

  * concept
  * insight
  * node
  * claim
  * note
  * thing
  * item
  * stimulus

The fact that I can’t find a unifying word here probably suggests trouble for the idea I’m thinking about. Maybe it doesn’t make sense to use the same word for a concept which can capture all these things, because the corresponding activities will differ enormously.

I guess the main claim is that I’m interested in investigating this proposition: right now, you encode stuff you want to bring into your practice sessions as questions/tasks/prompts; instead, maybe you should be writing down the thing itself.

To put this another way: to put something into a memory system right now, you encode it into prompts and tasks. What if, instead, you could put the thing itself into the memory system?

## ACT-R production connection

A goofy observation: [[John Anderson]]’s ACT-R models condition in terms of production rules. “If I see two intersecting lines where I know the angle here and I’m trying to find the angle there, I can do X.” They’re quite rote. I’ve been thinking recently that they’re probably the wrong level of abstraction, at least for the instructional designer. It seems unrealistic to imagine that we’re going to model hundreds of production rules for every subject. And possibly quite rigid too. Better, perhaps, to develop some way to infer them from a higher-level definition. FORTRAN for production rules. I’m sure there’s been a lot of work done like that in the [[Intelligent tutoring system]] space; I’m not well-read in the research there.

Anyway, I notice that my complaints about memory systems above rhyme with my observations about ACT-R. A given prompt usually reinforces a narrow, ACT-R- like production rule. Just as the instructional designer really shouldn’t have to encode all the adjacent variations of production rules in ACT-R-based ITSes, a memory system user really shouldn’t have to worry about writing prompts which produce traces of all those adjacent rules. In both cases you want a higher-level language.
