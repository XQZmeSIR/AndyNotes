# Simple spaced repetition algorithms mistreat expected failures

Most [[Spaced repetition memory system]] algorithms have a target recall rate in mind. Typical values are something like 85%-90%. But this means that in a typical session, if everything’s going exactly right, we should _expect_ to miss 10-15% of questions. And this isn’t (necessarily) because our encoding of those items is poorer than the others: memory is, at least in part, inherently stochastic.

Say that you’re going to review ten items, each of which has p=0.9. You should expect to miss one of them. But there’s no reason to treat the one that you missed differently from any of the others. They all have the same “hidden value” of retrievability. So you should treat them all identically, if you had perfect information.

But SM-2 will decrease the ease factor of the card, and its interval will grow more slowly forever, even if you always remember it.

The trouble, of course, is that we can’t actually _measure_ this hidden value. So what should we do when you miss an item? How do we know if that’s one of the “expected” failures or a “real” lapse, requiring more reinforcement? We can’t, really, but we can take a Bayesian approach. If the item continues to be marked as OK, we should eventually be persuaded that the lapse was one of those 1-in-10 errors. We should eventually treat it like its peers again. See [[Ebisu]] for a Bayesian approach.

Jarrett Ye’s implementation of [[Ye, J., Su, J., & Cao, Y. (2022). A Stochastic Shortest Path Algorithm for Optimizing Spaced Repetition Scheduling. Proceedings of the 28th ACM SIGKDD Conference on Knowledge Discovery and Data Mining, 4381–4390]] includes a low-pass regression to the initial difficulty. I wonder if regressing to the initial difficulty is the right call—the same issues apply there, right? Maybe better to regress to a mean difficulty?

## References

[[The Ease Factor Problem]]
