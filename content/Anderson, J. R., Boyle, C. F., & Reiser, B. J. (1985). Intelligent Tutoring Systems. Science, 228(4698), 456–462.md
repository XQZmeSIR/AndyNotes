# Anderson, J. R., Boyle, C. F., & Reiser, B. J. (1985). Intelligent Tutoring Systems. Science, 228(4698), 456–462

By [[John Anderson]] and colleagues, summarizing early work on [[Intelligent tutoring system]] in Science.

The paper introduces the concept of an “intelligent tutoring system”, which it contrasts from earlier computer-assisted instruction (CAI) models because it is _generative_ (hence lower-cost) and because it uses a detailed model of the domain and of the student to produce targeted intervention.

The model is built on ACT*, a cognitive theory which posits production rules involving goals, subgoals, and domain actions. Students are thought to work forward and backward simultaneously from some current domain state to some desired goal state.

To learn something in ACT* is to “acquire” a new production rule, through a process called “knowledge compilation”. (This rhymes a lot with [[John Sweller]]’s notion of schema acquisition; see [[Sweller, J. (1988). Cognitive load during problem solving: Effects on learning. Cognitive Science, 12(2), 257–285]]). The authors claim that “new productions are formed only during problem solving”, and so “instruction is effective to the degree that it can be integrated with problem-solving.”

The authors claim that “many errors…are due to failures of working memory rather than to failures of understanding”, so the tutor “encode[s]() on the computer screen much of the information that a student is likely to forget.” (See [[Cognitive load theory]]; here Anderson differs from Sweller in that—as far as I can tell—there’s no discussion of abstraction or chunking as a mechanism to combat working memory limitations)

The concrete tutoring paradigm (“model tracing”) is based on a sequence of “correct” productions for the problem (the “ideal model”) and of annotated error productions (“the bug catalog”). Student responses are mapped to productions; when an incorrect response is given, the bug catalog is consulted and an intervention presented. If the student makes valid steps but is getting far off track, the system will suggest a better path.

The system is mastery-based; that is, students can’t move on to a new concept until they master a given concept.

They ran some very small trials and found promising results: “students working with the computer tutor spent 30 percent less time doing the problems associated with the lessons and scored 43 percent better on the final exam than the students working on their own.”

Q. Why is problem-solving so central to the ACT* theory in ITS? A. Skill acquisition is production acquisition; productions are only formed during problem-solving. (So “instruction is effective to the degree that it can be integrated with problem-solving”)

Q. What is the role of instructional material in ACT* / ITS? A. It’s made part of problem-solving, rather than preceding the problem- solving, to emphasize production acquisition (which “only occurs during problem-solving”).

Q. What is the name given to the learning mechanisms by which new productions are acquired? A. Knowledge compilation.

Q. How does an ITS address working memory limitations? A. By having the tutor display information a student is likely to forget.

Q. What input models specialize the ITS’s behavior for a given problem? A. An “ideal model” (i.e. a sequence of productions for an “ideal” solution); an error catalog of “faulty” productions.

Q. At a high level, how does an ITS behave when a student inputs a response? A. It maps the student response to a production rule and evaluates whether that rule is “valid” based on the domain model; if not, it tries to respond with an intervention from the bug catalog. If so, it does nothing.
