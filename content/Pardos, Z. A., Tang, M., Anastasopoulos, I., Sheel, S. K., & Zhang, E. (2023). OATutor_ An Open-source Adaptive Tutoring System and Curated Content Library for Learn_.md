# Pardos, Z. A., Tang, M., Anastasopoulos, I., Sheel, S. K., & Zhang, E. (2023). OATutor: An Open-source Adaptive Tutoring System and Curated Content Library for Learning Sciences Research. Proceedings of the 2023 CHI Conference on Human Factors in Computing Systems, 1–17

Documents the first open-source implementation of a general-purpose [[Intelligent tutoring system]]. As part of the project, they created a framework for adapting several [[OpenStax]] textbooks to the platform, and deployed it [[here]].

It’s remarkable to me that in the nearly forty years of ITS history, there has been no open-source ITS. In fact, I stumbled on this paper today when I realized that I’ve been reading about ITS for years but have never actually _used_ a real one myself.

I find [[ACT-R]] incredibly tantalizing, intellectually. And I admire how [[John Anderson]]’s [[Cognitive Tutor]]s take cognitive architecture seriously in a way that more simplistic KA-style exercises don’t. I’m very interested in JRA’s anecdotes about the tutors being so beloved that the cause disciplinary problems. But I _hate_ using this ITS, in much the way I’d imagined I might given my read of the prior papers.

I think it’s a good exercise to dig into why this is. There’s _something_ about ITS that attracts me, even as most of it repels me. Maybe if I figure out what that is, I can generate some interesting ideas for my own work.

  * The multiple choice format reduces some problems to near-triviality. This does not really encourage much careful thought:
    * ![](image.png)
  * The questions are unmotivated and obnoxious. The worst kind of joyless worksheet math. Why am I doing this? I can guess, but I feel a vaguely noxious indifference from the author of this problem:
    * ![](image%202.png)
  * Though the system supports multi-step problems, all the questions I’ve tried, like the examples above, are single-step, which loses much of the meaningful diagnostic and intervention advantage of JRA’s ITS.
  * There’s no complex modeling of production rules or knowledge compilation happening here, like in a [[Cognitive Tutor]]. Instead, problems are assigned a coarse skill like `classifying_a_real_number`. This is just the basic Khan Academy knowledge architecture. 
  * Cognitive Tutors have a library of exemplary errors and explanatory messages associated with each. This system just starts presenting hints in response to a wrong answer (where the hint is not specific to the selected wrong answer).
  * The interaction of inputting answers via multiple choice or a text box makes me feel like I’m at the DMV. Or Kumon, I suppose. I’m squeezing all the rich activity going on in my head into a 1-bit “right or wrong” answer. Ugh ugh ugh.
  * From the paper’s contribution descriptions, it seems that most of the material work here was done by undergrad researchers; I suppose that explains a lot of what I see here, but I wish Zachary had taken a stronger hand.
  * If you think of this as an OSS, serverless, DIY-friendly Khan Academy, rather than a [[Cognitive Tutor]]-style ITS, it’s a very nice contribution!

Because this system is so much more simplistic than JRA’s designs, it’s hard for me to map my experience here onto that, unfortunately. Amazing how hard it is to actually try a [[Cognitive Tutor]]-style ITS.
