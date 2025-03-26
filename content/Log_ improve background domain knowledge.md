# Log: improve background domain knowledge

## Reading queue

  * Cognitive science
    * [[UCSD Reading List]]
    * What is memory, anyway? What are our best models?
  * Discipline-Based Education Research
    * Dave Pritchard: physics educational work, Mastering Physics
    * Eric Mazur: peer instruction, learning catalytic
    * Carl Wieman
    * Improving How Universities Teach Science
    * e.g. using the Force Concept Inventory

# Log

[[2021-04-02]]

  * [[COGS 101B - Lecture 23 - Memory errors]]
  * [[COGS 101B - Lecture 25 - Knowledge concepts and categories]]

* * *

[[2021-03-26]]

  * [[COGS 101B - Lecture 19 - Long-term Memory - Encoding, retrieval, consolidation]]
  * [[COGS 101B - Lecture 21 - Eyewitness memory]]

* * *

[[2021-03-19]]

  * [[COGS 101B - Lecture 18 - Long-term Memory]]
  * [[COGS 101B - Lecture 19 - Long-term Memory - Encoding, retrieval, consolidation]]

* * *

[[2021-03-12]] (finished 16…)

  * [[COGS 101B - Lecture 17 - Long-term Memory]]

* * *

[[2021-03-05]]

  * [[COGS 101B - Lecture 12 - Attention]]
  * [[COGS 101B - Lecture 13 - Attention]]
  * [[COGS 101B - Lecture 14 - Attention]]
  * lecture 15: broken! oh no! and it’s an introduction to memory!
  * [[COGS 101B - Lecture 16 - Short-term and Working Memory]]

* * *

[[2021-02-26]]

Spent some time consolidating notes from the first 7 lectures. I don’t like what I did last time: writing notes compressing the lecture, then trying to write good [[Evergreen notes]] out of those. The results felt shallow, and the work duplicative. My understanding wasn’t grounded in enough meat to really grasp what was going on. Feels like a high school show-and-tell level understanding. I probably need to read the textbook to really grok what’s going on.

But this week I’m going to try writing SRS prompts as I listen.

  * [[COGS 101B - Lecture 8 - Perception]]
  * (lecture 9 is the midterm)
  * [[COGS 101B - Lecture 10 - Knowledge shapes perception]]
  * [[COGS 101B - Lecture 11 - Knowledge shapes perception continued, attention]]

* * *

[[2021-02-12]] Going to try COGS 101B today: “Learning, Memory & Attention.” 28 lectures in this class. Textbook is “Cognition” by Daniel Reisberg. Prof is Drew Hoffman (“Assistant Teaching Professor”). Course uses ZAPS Labs, which let students recapitulate classic psych experiments (either as instructor or as participant).

It’s a ten-week course. Three 45-minute lectures each week, plus labs, exercises, and reading. 25 total lectures: about 7.5 hours at 2.5x.

Class characterizes itself mostly in terms of psychology / cognitive psychology.

![](685B9E75-95E1-461B-B74A-336E8BD95D52.png) ![](89F6C2D6-039D-45F2-B4D7-E842DD90DD71.png)

### Lecture 2 (01/10, Studying the mind: a brief history)

#### The cognitive revolution (40’s and 50’s)

Tolman and Chomsky proposed that complex behavior is often best explained by positing internal states. The digital computer was also seen as a meaningful metaphor for minds. The revolution also arose from new methods which made it possible to study these internal states, e.g. Shephard and Meltzer (1971).

Tolman’s maze (1948) studied rats in mazes. They’d be repeatedly placed in a position with food in a leg to the right. Operant conditioning would predict that if a rat were placed in a different initial spot, it would turn right from that point. But in fact, the rat finds the food regardless of where it’s initially placed. Tolman suggests that the rat had formed a “ **cognitive map** ,” a mental representation of the maze’s layout.

Skinner wrote “Verbal Behavior,” which claimed that language could be learned through operant-conditioning. Chomsky published a scathing review, pointing out that children produce speech they’ve never heard or been rewarded for. This suggested that complex abilities required understanding more than just observable behavior.

The “information-processing approach” suggests that we can model sequences of mental operations like computer flow diagrams, from input to output. Broadbent (1958) proposed the first “flow diagrams for the mind,” representing attention. ![](AFCB3F48-0E29-474C-8E08-A54F5C247346.png) He had people listen to headphones with different conversations in each ears. People were able to attend to conversations which happened just in one ear, suggesting that we can filter our inputs.

1956: the “birthday of cognitive science,” characterized by a summer research project on AI and the MIT symposium on information processing. A key topic being discussed was: can we make a computer mimic the operations of the human mind? Newell & Simon’s “logic theorist” (1956) attempted this by generating proofs for mathematical theorems.

Shepard and Metzler in 1971 showed people 3D shapes in different orientations and asked them whether they were the same or different: ![](D2CD8B78-B768-47B6-AA5C-B79094E5E801.png) This requires forming a detailed mental representation of the shape and performing a 3D operation on it. Even more surprisingly, he found that the amount of time people needed to answer the question varied (perfectly linearly!) with the angle of necessary rotation! This is a quantitative measure of mental imagery. Remarkable.

All this suggests that we must study the internal mental world to understand behavior, but we can’t study it directly. That’s a challenge! The _transcendental method_ proposes that we can reason backwards from observations to infer the best causal explanation. This is similar to what physicists do, of course: using observable effects to tell us something about an unobservable cause.

These inferences are how we make _cognitive models,_ which represent mental structures and help us visualize/explain/operate on them.

Our model of the brain’s physical structure (“language region”, a model of the visual system) is an example of a _structural model_.

_Process models_ are box-and-arrow systems approximating cognitive mechanisms, following the flow diagrams from the information-processing approach. ![](789D011D-03CB-4B69-8107-23CEDFBC0634.png)

### Lecture 3 (01/12, cognitive neuroscience)

Cognitive neuroscience: the _physiological_ basis for mental processes. How does brain structure relate to brain function?

Basic assumptions on cognitive neuroscience:

  * neurons send electrical signals
  * localization: different parts of the brain perform different functions, so different cognitive processes may cause areas to exhibit more/less electrical activity

Methods:

  * neuropsychology: observe behavior/function of people with damage to healthy people (e.g. H.M.)
  * neuroimaging: observing which regions are active during a task
  * transcranial magnetic stimulation: activating or impeding a region to observe changes in performance

#### Split brain experiment.

Most parts of the brain come in symmetrical pairs (one in each hemisphere). Many structures have differences in function between the left and right side (called **lateralization** ).

The hemispheres are connected by {commissures}, the larges of which is the {corpus callosum}.

This is distinct from **contralateral organization** : structures where the circuits are “crossed,” e.g. the left hemisphere’s motor cortex controls the right side of the body, and the same for the visual field.

A split-brain experiment on patients with severed corpus callosums can show that language is lateralized. A patient who sees a spoon in the left side of their visual field can’t verbalize that (i.e. because their language center is mostly in their left hemisphere), but they can reach for it with their left hand.

#### Neuroimaging

A core challenge of neuro-imaging is navigating a trade-off between spatial resolution (where it happens) and temporal resolution (when it happens).

CT (computed tomography) is better for bony structures. MRI (magnetic resonance imaging) is better for soft tissue.

PET (positron emission tomography) is “an older version of MRI” that works by injecting a radioactive glucose. When a region is more active, it consumes more glucose, which the scanner detects through radioactive decay (emitted positrons interact with electrons in the tissue, which then emit gamma rays). Spatial and temporal resolution is moderate, not great. PET scans are less subject to movement than MRI, though.

fMRI records many MRI pictures over time to understand brain function. An active brain region has increased blood flow. The iron in the blood flow aligns to the magnetic field, and changes in its concentration is detectable. fMRI records voxels of ~2mm^3. But a challenge for fMRI is that just because a region is active when a person’s doing something, that doesn’t mean it’s critical for that task. It’s a correlative measure.

EEG (electroencephalography) has high temporal revolution. You wear an electrode cap which measures electrical activity over many neurons (spatial resolution of several cm^2). It’s useful for observing the brain’s response to an event—the electrical activity which occurs in response to some stimulus.

### Lecture 4 (01/17, cognitive neuroscience continued, learning)

![](2F2A001F-B9A4-42E9-A186-6EEBF6EB0838.png) Overview of neuroimaging ^

Signal-unit recording depends on attaching an electron to a single neuron. (Note: an electron firing involves a shift on the order of 100mV. Pretty large!)

TMS (transcranial magnetic stimulation) induces electrical current in a target area. We can use this to disrupt function, like simulating a lesion.

#### Mental representations

Principle of neural representations: everything we experience is based not on direct contact with stimuli, but on _representation_ of it in the nervous system.

Action potentials all have roughly the same amplitude and shape, so the arrangement of neurons must encode the characteristics of what they represent. One kind of arrangement is _hierarchical processing_ : leaf-level neurons respond to primitive signals; signals from many neurons are pooled to respond to more complex stimuli.

Specificity coding is the theory that there’s a 1:1 connection between neurons and possible representations—e.g. a “grandmother” neuron which fires when you see or think about your grandmother. More likely is population coding, which suggests that representations are encoded in a pattern of neural firing. Sparse coding suggests that these codings involve only a minority of neurons in the relevant area.

Quiorga et al (2008) did single unit recording during epilepsy surgery and exposed patients to pictures of public figures, finding that sparse coding is more likely than population coding, at least for those representations.

Many areas have strong evidence for localization: the fusiform face area for faces, the parahippocampal place area (for places), extrastriate body area (bodies). But there’s also evidence for distributed representation (the opposite proposition): some cognitive functions activate many areas (e.g. faces, memory).

#### Learning

Learning: a behavioral change based on definition; or storage of information in memory as a consequence of experience.

We have hardware which helps us learn. For instance:

  * simple reflexes, like the “orienting response” which makes you turn to face stimuli
  * fixed-action patterns (in other animals) which encode innate skill sequences that the animal doesn’t have to learn, and which it performs mechanically. They’re triggered by stimuli called “releasers.” In many cases it’s possible to fabricate “supernormal stimuli”, exaggerating natural stimuli to produce stronger responses.
  * critical periods: favorable periods in development for learning a particular behavior (ducks imprinting their mothers in some limited period); human language learning appears to be an example

### Lecture 5 (01/19)

Missing!! Dang. I think this was supposed to be a lecture on habituation and sensitization.

### Lecture 6 (01/22)

See [[Classical conditioning]]

### Lecture 7 (01/24: learning)

See [[Operant conditioning]]

#### Cognitive perspective on behaviorist data

See [[Behaviorism]] and [[Cognitivism]]

* * *

[[2021-02-05]]

### Lecture 10: Learning to See (de Sa)

Newly-sighted adults “see but don’t see”—they can distinguish objects but can’t identify them correctly.

One early way that scientists studied visual perception was through single cell electrophysiology: inserting an electrode into some part of the brain, e.g. to demonstrate a cat’s neuron firing preferentially for vertical shapes over horizontal shapes. As the signal progresses into deeper brain regions, combinations of edges and more complex shapes are recognized through convolution of the signals.

But the visual system isn’t just feed-forward: it’s influenced by recent exposure and memory.

Methods for understanding perceptual systems:

  * physiology
    * single cell electrophysiology (i.e. individual neuron response)
    * optical imaging (groups of neurons)
    * microstimulation (examine behavior when regions are stimulated)
  * psychophysics
    * analyze visual illusions
    * analyze lesion cases
  * computational models (i.e. to validate / simulate biological models)

### Lecture 11: developing social skills (Deák)

One of the key motivations for studying the development of traits is that seeing how it emerges can tell us much about its properties.

3 month olds can recognize walking motion from a few dots—but not when they’re upside-down! We can tell when a baby sees things as similar/different by their habituation patterns: how long they look at something before looking away.

4 month olds don’t seem to be able to distinguish mother’s faces from their stranger (if you hide the hairline), but 8 month olds can.

(got bored, skipped ahead)

### Lecture 12: HCI (Hollan)

… mostly shallow, though some of the projects referenced sound quite interesting. But nothing discussed in enough detail to really engage with.

### Lecture 13: midterm review… again!

### Lecture 14: midterm 2

Jeez, this course is 20 class sessions, and _six_ of them are consumed by assessments and their review sessions. And the first lecture is half housekeeping, so a full third of the class is lost. Unfortunate.

### Lecture 15: language learning

Interesting that phoneme errors in kids are somewhat consistent across kids, e.g. th -> f. (Darf Vader)

Some neat discussion of how infants learn to identify word boundaries, but not interested enough to study in detail.

### Lecture 16: swearing (Bergen)

Hearing swears causes increased heart rate and sweat!

People can hold their hands in freezing water longer (and report less pain) when swearing! But if you’re a frequent swearer, it has a lesser effect!

Almost every profane English monosyllabic word ends with a closed syllable.

Aphasia patients are still able to produce swears! Also, patient EC who had one hemisphere of their brain removed was able to swear but struggled to produce other speech. But a patient with a stroke in his basal ganglia _lost_ his ability to swear (couldn’t complete swear words).

### Lecture 17: HCI… jobs? (Philip Guo)

### Lecture 18: “Design at Large” (Klemmer)

“Prototypes are postcards from the future”

“Everyone designs who devises courses of action aimed at changing existing situations into preferred ones.” (Herb Simon)

* * *

[[2021-01-29]]

### Lecture 4 (Eran Mukamel: epigenetic regulation of brain development and plasticity)

Neural cells within a single organism have the same genome, but they grow into different types (neurons vs. glia), located in different places in the brain, and connected to different neighbors. How do they differentiate?

Interesting bit of trivia: at birth, humans have around 50 synapses per 100 µm^3. At adulthood, that falls to 40, and when aged to 30. (Mice have a higher density!)

DNA isn’t stored straight: sections (about 100 base pairs) are wrapped up around histone proteins. Those histone structures are organized in higher level structures with various scaffold proteins.

CH3: a methyl group. Base pairs in DNA can be “methylated,” i.e. have a methyl group attached. It’s a covalent modification, stable enough to last your whole lifetime. These methyl groups affect transcription, and they’re (somewhat) preserved when cells reproduce—i.e. so they may be partially heritable.

When a gene is highly methylated, it is {less} likely to be expressed.

At least in mammals, methylation mostly occurs at “CG sites,” i.e. places where a guanine follows a cytosine in sequence. Pluripotent stem cells have broader methylation, but the significant exception for adults is within neurons, where there’s as much methylation on other cytosine pairs as on CG pairs. In fact, within humans, the non-CG methylation increases throughout adolescence. What’s more, the methylation patterns are similar between individuals, so there may be some biological function. And different cell types have different methylation patterns, consistent across individuals.

Weaver et al found that differences in maternal care in mice produced differences in offspring methylation, which was linked to stress behavior.

Methylation can be measured through shotgun sequencing, by treating the sequences with sodium bisulfite, which converts C to U. But methylated cytosines are “protected” from this mutation, and that difference can be used to detect methylation.

 **Skipping lecture 5, on animal cognition**  
 **Skipping lecture 6, a fairly shallow midterm review**  
 **Skipping lecture 7, the midterm**   Gosh… the info density in this class is so low!

### Lecture 8: mirroring in social cognition (Pineda)

One hypothesis for the increase in social brain size is that our increasingly social environment put increasing demands on our brain: the “social brain hypothesis.” Dunbar suggests that the size of our cortex relates to the size of the social network we live in.

Q. What is the “social brain hypothesis”? A. Increased human cortex size was driven by demands from increasingly social environments.

Q. What key value does Dunbar suggest predicts the size of an organism’s cortex? A. Size of social network

We have evolved neural systems for motor imitation, coordination, empathy, and theory of mind—all core social mechanics. e.g. If you stick your tongue out at a newborn infant, it will imitate you.

Tung et al found that if two primates spend time together, they end up sharing a microbiome! Meadow et al found a similar result for a _cloud of microbes_ which supposedly float around humans.

We understand others’ behavior through simulation. For example, we’ll map visual perceptions of motion onto our own motor cortex. This and related phenomena are called mirroring systems. There are specific cells we call “mirror neurons” which fire both when we make a movement and when we observe another person making the same movement. Autistic individuals have less activity in these mirroring systems.

Hands and faces have disproportionate numbers of neurons devoted to them; this may be in part because those body parts are disproportionately involved in social interaction.

### Lecture 9: social cognition and social interaction (Rossano)

(didn’t find this very interesting)

* * *

[[2021-01-22]] I’m starting by pulling course catalogs and syllabi from UCSD’s cogsci department, since that’s apparently the first cogsci department. There’s an intro course (a survey providing a map of the field—a “buffet”) and a course focused on learning and memory, as well as a reading list.

### Lecture 1 (intro; overview)

Watching the “intro to cog sci” lectures at 2x would take 15 hours, or about 5 weeks of Friday afternoons. I’ll probably skip much of it. Let’s watch the first lecture to get the feel.

Q. cogsci: What is top-down processing? A. Higher level processes (thoughts, memories) influencing lower level processes (perception)

Q. cogsci: What is a divergent pathway? A. One pre-synaptic neuron; many post-synaptic neurons

Q. cogsci: What is convergent processing? A. Many pre-synaptic neurons; one pre-synaptic neuron

Q. What’s an example of a way in which perception is affected by memory? A. e.g. If you know what a distorted recording says, you can perceive the voice much more clearly.

Q. What’s the McGurk effect? A. Auditory perception distorted by visual perception: watching a person’s lips say “guh” while listening to them say “buh,” you’ll hear “guh.”

Finished watching first lecture. Not clear to me yet whether these will be valuable. Having a survey might be useful. I’ll skim the second lecture now. Was a very light overview of data science.

### Lecture 3: adult neurogenesis (Lara Rangel)

Third lecture: adult neurogenesis (Rangel). Mostly occurs in the
**subventricular zone** of the lateral ventricle, where they typically migrate to the olfactory bulb, and the **subgranular zone** of the dentate gyrus in the hippocampus, which is important for learning/memory.

The dentate gyrus appears to be involved in discriminating between similar past experiences. The hypothesis is that neurogenesis supports this time-base discrimination: developing neurons are particularly excitable, becoming sensitive to experiences which occurred during their two-week development period. So over time, as waves of new neurons develop, they’ll be differentially activated by experiences according to time.

Q. What brain region is key to discriminating memories of similar past experiences? A. The dentate gyrus

Q. How might adult neurogenesis explain how the dentate gyrus distinguishes between memories of similar events which took place at different times? A. New neurons become sensitive to stimuli which occur during their first two weeks of development; successive generations of new neurons can therefore discriminate time
