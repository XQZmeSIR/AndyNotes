# DARPA Digital Tutor

The DARPA Digital Tutor was an [[Intelligent tutoring system]] developed to train new Navy sailors to become IT technicians. Deployed in a program which included a human expert available on-demand (when the system detects the need), it achieved dramatic learning gains over a six-week program, producing students who outperformed experienced Fleet technicians in a variety of authentic tasks.

Concrete design details in the 2014 report are quite scant—too scant to build on. Unfortunately, Fletcher’s several followups recycle the text from the 2014 report without adding specific detail about the architecture of the system. The system is an “eclectic and pragmatic” design, clearly influenced by the ITS heritage, but without claiming any specific system architectures as antecedents.

Some details of the design:

  * The organizers first had human 1:1 tutors create a 16-week course, then induced an instructional design off their work.
  * The Tutor course was developed into a curriculum with a sequence of subtopics. Learners would spend a fixed amount of time in each segment, with faster learners reaching more complex material in that topic.
  * It’s centered on problem-solving, with some explicit instruction. The problem-solving often takes place through interaction with real network systems, which the Tutor can observe and track.
  * There are zero citations of [[John Anderson]] or his Cognitive Tutors, but the Digital Tutor seems to follow similar lines of formal student modeling: “The Tutor relies on a back-end that involves classic knowledge engineering—feature extraction, ontologies, and inferencing. The Inference Engine captures problem-solving processes—the strategy and path each learner is using to solve problems based on what the learner understands or misunderstands.”
  * This modeling is used (somehow—it’s not described) to choose a next instructional element: “This Engine then uses the information to decide what to specify next, what instructional technique to use, and how to present it.”
  * The Tutor uses a conversational interface, where it can offer explanations and assess student understanding. This seems very along the lines of [[AutoTutor]], but again, description is too scant to really understand what’s going on. (two Graesser cites in the 2014 report, though not explicitly of AutoTutor)
    * One interesting conversational element that’s mentioned: it’ll “promote learner reflection and abstraction” by soliciting explanations and connections, asking probing questions, and so on.
  * Human mentors are available at all times; the system has a module which assesses whether the conversation’s gotten beyond what the system can do, and it’ll summon a mentor if needed.

I don’t have a clear picture, at all, of how this system actually works. I’m pretty frustrated about that. The system was clearly developed through a lot of empirical iteration (see quote below), but that doesn’t mean it can’t be well documented.

> Finally, no “magic sauce” or specific academic theory was used to produce > the DARPA Digital Tutor. It was designed and developed by using empirical > means to identify high-quality, but well-known, tutorial ingredients and > applying them in proportions determined by systematic, empirical testing. > (Fletcher, 2019)

Could one FoIA the details of this system? It sounds like they used a contractor to design and build the thing. Surely there are design documents?

For that matter: who actually lead the design of this system? The 2014 report is published by The Institute for Defense Analysis, “an independent third- party evaluator.” If it’s an independent third party, then that suggests its authors, Fletcher and Morrison, didn’t design the system. Ralph Chatham was the DARPA program officer, but I don’t imagine that the program officer did the design work. One other thing that confuses me: Fletcher writes that DARPA—the agency—carried out this R&D program. But DARPA doesn’t generally do R&D as far as I know; it funds others.

## Acuitus

[[This 2020 EdSurge article]] leads me to believe that a Sunnyvale company called [[Acuitus]] did the work. It was founded in 1999 by John Newkirk and Maria Machado, who had long careers in the semiconductor industry before turning their attention to education, inspired by [[Herb Simon]]’s “learning engineering” frame.

> He has gotten a lot of support in the form of more than $50 million in > funding from U.S. government agencies including the Defense Advanced > Research Projects Agency (DARPA), the Department of Defense’s research shop > for big new ideas.

Acuitus is now commercializing the technology for IT training, focused particularly on veteran job training. See Fletcher (2017) for more. Not much public information about it. But there is one solitary screenshot in the EdSurge article, which provides some good clues: ![](image.png)

  * An instructional interface is presented alongside a live machine
  * The student is presented with a concrete task to achieve in the live system
  * The training system begins by “discussing the situation”, probing the student’s understanding with questions, and responding with appropriate feedback and follow-up tasks.
  * It can observe the student’s actions in the live system and respond appropriately.
  * The instructional interface uses a text-conversational modality.
  * I see a lot of influence from both [[AutoTutor]] and [[Cognitive Tutor]] (“information structures”)

One Redditor [[gives a testimonial]] of the Acuitus offering:

> Upon graduation I had a job lined up doing desktop support for a federal > agency making $27/hour with no benefits. Since it was a contract I left it > about 8 months later. Since then my job titles have advanced to Network > Admin, Network Engineer, Information Systems Security Officer, to my current > job as a Cybersecurity Engineer making about $140k. > > When I think back on it, I was taking a big risk for my family so I could > attend the program. But it was the best thing I could have done. I don't > know if I would have done it if it weren't free for me. I'm glad and > grateful for everything Acuitus did and if you're looking for a > recommendation, I give them 100% of my support.

## Synthesis

[[Synthesis (startup)]] claims to have “partnered with the team that created the original DARPA program. We expanded upon their research, tailor-made a platform for kids ages 7-10, and extended what they achieved with modern AI tools.” It’s hard for me to see the concrete connection in their [[Synthesis Tutor]]. It doesn’t seem to be doing the kind of deep knowledge modeling described in the DARPA report. I’d guess it’s more an advisory-vibes thing, along the lines of Khan Academy’s relationship with Carol Dweck.

## References

  * Fletcher, J. D., & Morrison, J. E. (2014). _Accelerating Development of Expertise: A Digital Tutor for Navy Technical Training_. Institute for Defense Analyses.
  * Fletcher, J. D. (2017). The value of digital tutoring and accelerated expertise for military veterans. _Educational Technology Research and Development_ , _65_ (3), 679–698. ~<https://www.jstor.org/stable/45018573>~
  * Fletcher, J. D. (2018). Adapting Learning with Digital Tutoring. Technology, Instruction, Cognition and Learning, 11(1).
  * Fletcher, J. D. (2019). Adaptive Instructional Systems and Digital Tutoring. In R. A. Sottilare & J. Schwarz (Eds.), Adaptive Instructional Systems (Vol. 11597, pp. 615–633). Springer International Publishing. <https://doi.org/10.1007/978-3-030-22341-0_48>   (unfortunately, Fletcher’s several follow-ups don’t meaningfully expand on details of the Tutor—he’s often copying and pasting verbatim text)

### Commentaries

  * <https://www.lesswrong.com/posts/vbWBJGWyWyKyoxLBe/darpa-digital-tutor-four-months-to-total-technical-expertise>
  * [[On Bloom's two sigma problem: A systematic review of the effectiveness of mastery learning, tutoring, and direct instruction]]
