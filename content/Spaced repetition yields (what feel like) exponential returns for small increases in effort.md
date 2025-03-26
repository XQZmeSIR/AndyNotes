# Spaced repetition yields (what feel like) exponential returns for small increases in effort

[[Spaced repetition memory systems are extremely efficient]], but that phrase doesn’t get across the nature of the efficiency. There are lots of things you might try to improve yourself—reading more books, talking to experts, etc. These things will all help, of course, but they also yield diminishing returns fairly rapidly. Spaced repetition doesn’t work like this. If you spend a few extra minutes reviewing prompts about something you’ve read, you’ll get vastly more out of the material. Each time you subsequently review (constant time), you’ll be able to wait longer until the next review (exponential increase… or at least an increasing increase).

There are some problems with this observation. The exponential phenomenon can be largely seen as an artifact of the review schedule. _It’s_ expanding exponentially, so memory stability seems to be expanding exponentially. But [[Plots of demonstrated retention exaggerate exponential benefit of practice]]. You really want some to look at some kind of continuous “memory stability” parameter, describing (say) the half-life or the time to fall to 90%. And then you want to look at the impact of repetition on that parameter.

That said, the model fit in [[Ye, J., Su, J., & Cao, Y. (2022). A Stochastic Shortest Path Algorithm for Optimizing Spaced Repetition Scheduling. Proceedings of the 28th ACM SIGKDD Conference on Knowledge Discovery and Data Mining, 4381–4390]] for a language learning data set does indeed predict exponential increase in half-life with each repetition (well, compounding increases with a slowly falling geometric constant): [[Calculator Suite - GeoGebra]]

* * *

## References

Matuschak, A., & Nielsen, M. (2019, October 0). _How can we develop transformative tools for thought?_ <https://numinous.productions/ttft>

> Given that the essay takes about 4 or so hours to read, this suggests that a > less than 50% overhead in time commitment can provide many months or years > of retention for almost all the important details in the essay. > > This is the big, counterintuitive advantage of spaced repetition: you get > exponential returns for increased effort. On average, every extra minute of > effort spent in review provides more and more benefit. This is in sharp > contrast with most experiences in life, where we run into diminishing > returns. For instance, ordinarily if you increase the amount of time you > spend reading by 50%, you expect to get no more than 50% extra out of it, > and possibly much less. But with the mnemonic medium when you increase the > amount of time you spend reading by 50%, you may get 10x as much out of it. > Of course, we don’t quite mean those numbers literally. But it does convey > the key idea of getting a strongly non-linear return. It’s a change in the > quality of the medium.
