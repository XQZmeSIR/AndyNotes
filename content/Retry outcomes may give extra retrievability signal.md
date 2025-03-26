# Retry outcomes may give extra retrievability signal

A big problem for models and evaluation in a [[Spaced repetition memory system]] is that you’re trying to estimate a continuous value (probability of recall, or retrievability per [[Two-component model of memory]]) over time, but all you get are these sparse one-bit binomial samples: remembered, or didn’t remember. If a reader failed to remember, their retrievability might be 10%, or it might be 90%.

But in the presence of a typical [[SRS retry mechanism]], suppose the reader failed to remember in the retry attempt shortly following that first attempt. Now your estimate of the retrievability at the first attempt should be revised downward. It should be revised further downward if there are multiple failures.

I’m not sure how to actually build a model incorporating this. How much should the retrievability estimate fall with each subsequent failure? I’m not sure how to get any “ground truth” here.

This kind of signal _sort of_ appears in academic literature, where it’s common for the protocol to specify that subjects repeatedly practice items until they succeed. The number of attempts is sometimes analyzed as a variable. [[Hermann Ebbinghaus]] used the number of attempts as the almost exclusive signal (a coarse signal of retrievability) in [[Ebbinghaus, H. (1913). Memory: A Contribution to Experimental Psychology (H. A. Ruger & C. E. Bussenius, Trans.). (Original work published 1885)]].

## References

This idea came up in a conversation with [[Giacomo Randazzo]] on [[2022-02-22]]; he complained that he had to discard many of his “forgotten” samples because they were “retry” attempts. At first I thought: well, of course you have to discard them; they’re meaningless because the ISI is almost zero. But then I realized what I describe here.
