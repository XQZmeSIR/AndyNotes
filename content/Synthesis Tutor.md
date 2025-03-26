# Synthesis Tutor

Some notes on the preview [[demo]] of the tutor produced by [[Synthesis (startup)]]; I haven’t seen the full system (insofar as more exists as of [[2023-06-14]]).

## What they did

The demo is a lesson on binary representation of numbers with some light reference to place value. It’s around 10 minutes long.

The interface consists of two components:

  * a chat-style interface in which the tutor’s instruction is presented as messages; input is occasionally offered via a small set of buttons (e.g. choosing “Let’s do another” or “I’m done”) or numeric input
  * a shared interface displaying the linked representation of a binary number in several representations (evolving in complexity over time, a la [[Cognitive scaffolding]])

The lesson is a scripted sequence of messages delivered from the tutor to the student via the chat interface, but with some extra [[Dynamic medium]] affordances:

  * Sometimes the messages will ask the student to do something with the binary number interface, and pause until the machine’s in some state.
    * In some cases, if the machine is placed into a “bad” state, or if you take too long, the tutor will send an extra message to try to help.
    * Conversely, the tutor can “lock” the binary number interface when in the middle of a longer explanation.
  * The tutor’s script also includes programmed changes to the machine’s representation over time.
  * There’s some very simple branching structure to the script:
    * The tutor will respond to your input numeric/radio answers, either validating a correct answer or providing an explanation in response to an incorrect answer.
    * In the final activity (but not earlier?), you’re asked to try again until you answer correctly.
    * It _seems_ like incorrect answers may also provoke an additional scripted activity intended to help explain the error earlier (as an [[Intelligent tutoring system]] would do), but in my experiments, the extra activities are assigned in any case—just with different text justifications.

The script tries to guide some implicit learning in the binary representation interface, which it then formalizes through explicit instruction. It then tries to ensure that you’ve reached the learning objectives by closing the lesson with an exercise which repeats until the student is successful.

## Interpretation

This is roughly a [[Narrated explorable]]: there’s a [[Dynamic medium]] representing the mathematical concept, shared by author and by reader, presented within an authored narrative. Unlike most [[Explorable explanations]], the script behaves and responds (very minimally) to reader action, roughly on the level of most of [[Nicky Case]]’s projects.

The simple branching mechanics seem roughly like those of 70’s-era computer assisted instruction (CAI) systems. It’s not obvious to me that that’s such a bad thing, but I can easily imagine completing the lesson’s gated final exercise without having understood several of its key ideas. The authors say that the system is based on the [[DARPA Digital Tutor]] work, but I don’t see those mechanics here at all, at least at the instructional design level. A “real” ITS would be able to diagnose that I hadn’t understood, say, that each place value doubles the value of the previous, and would move me to a task to reinforce that atom. This system only has an all-or-nothing gate at the end, without the fine- grained modeling that’s the hallmark of ITS.

Classic CAI systems also embedded instruction into exercises and dynamic representations, but (like most [[Explorable explanations]]) this system emphasizes exploration and discovery with the representation, rather than immediately jumping to formality as most classic systems do.

Still, compared to a worksheet or a Khan Academy video/exercise combo, this is a clear improvement in many respects. It’s nice to see more dynamic representations with linked narration in action. The conversational transcript is a good solution to the problem of presenting instruction simultaneous with a dynamic representation, and it offers a natural way to solicit multimodal responses from the student which can’t be expressed directly in the dynamic representation. And while PLATO and classic [[Intelligent tutoring system]] implementations like [[GeometryTutor]] include dynamic representations, modern interface design patterns certainly afford opportunities for improvement.

The narration is poorly executed, with low emotional affect. It’s hampered by an automated text-to-speech voice and prose which often reads as condescending (to me, anyway). The author makes only an offhand attempt to create intellectual need for the material being taught. Once the material is learned, no attempt is made to explain its significance or to connect it to subsequent learning objectives. I don’t believe that the narrator/author is actually interested in talking about this subject ([[Authored environments are significantly colored by authors’ motivations]]).

See also [[Synthesis Tutor (private)]])
