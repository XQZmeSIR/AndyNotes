# Mozer, M. C., & Lindsey, R. V. (2016). Predicting and Improving Memory Retention: Psychological Theory Matters in the Big Data Era. In M. N. Jones (Ed.), Big data in cognitive science (pp. 34–64).

This book chapter is a condensed summary of the major project from Lindsey’s thesis (2014) and an elaboration on the related 2014 paper from Lindsey et al.

It builds on the prior multi-scale context model (Mozer et al, 2009) in two main ways: first, by introducing item-difficulty and student-ability parameters which better capture non-uniform content and student populations; and second, by adding parameters which are used to summarize a student’s study history.

The key innovation here is that the authors constrain general-purpose machine learning models with terms corresponding to psychological models of memory and learning. The insight is that if you’re trying to learn a tensor describing how students behave on item i at time t, the time points aren’t independent: they’re meaningfully related in a way described by the mechanics of memory.

In the first major section, the authors describe how traditional item-response theory can be combined with the established power-law [[Forgetting curve]] function to create a predictive model for forgetting after a single study session using relatively few parameters (one per student, one per item, and a time scaling parameter).

The second major section extends that work by incorporating a term for the study history.

They use this model to construct a scheduler which prioritizes items by how close they are to a forgetting threshold. They find that models which omit study history or the latent parameters don’t do as well.

Q. How does collaborative filtering apply to the problem of predicting student knowledge? A. Imagine a tensor of students x problems x time; you’re trying to predict the missing cells.

Q. Key difference in approach, relative to purely data-driven knowledge state models? A. Incorporates constraints based on psychological models of memory

Q. Broadly, what two approaches do they use to incorporate varying skill levels and difficulty into the forgetting curve? A. Modified decay rate; modified initial memory strength constant

Q. What are the two parameters of the 1PL model of IRT? A. $d _i$, the difficulty of the item; and $a_ s$, the ability of the student.

Q. What is the predicted response of the 1PL model of IRT? A. $Logistic[a - d]()$, i.e. $\frac{1}{1 + exp(d - a)}$

Q. What does the DASH model stand for? A. Difficulty, ability, study history

Q. Schematically, what’s DASH’s predicted response? A. $Logistic[a - d + h]()$, where $h$ captures the study history.

## References

Lindsey, R. (2014). _Probabilistic Models of Student Learning and Forgetting_. University of Colorado.

Lindsey, R. V., Shroyer, J. D., Pashler, H., & Mozer, M. C. (2014). Improving Students’ Long-Term Knowledge Retention Through Personalized Review. Psychological Science, 25(3), 639–647. <https://doi.org/10.1177/0956797613504302>

[[Mozer, M. C., Pashler, H., Cepeda, N., Lindsey, R., & Vul, E. (2009). Predicting the Optimal Spacing of Study: A Multiscale Context Model of Memory. In Y. Bengio, D. Schuurmans, J. Lafferty, C. K. I. Williams, & A. Culotta (Eds.), Advances in Neural Information Processing Systems 22 (pp. 1321–1329).]]
