# Ye, J., Su, J., & Cao, Y. (2022). A Stochastic Shortest Path Algorithm for Optimizing Spaced Repetition Scheduling. Proceedings of the 28th ACM SIGKDD Conference on Knowledge Discovery and Data Mining, 4381–4390

On [[Optimizing spaced repetition system schedules]]. From Jarrett Ye, a patron.

For me, the interesting central idea in this paper is that they use _half- life_ as a key representation of the state of a [[Spaced repetition memory system]] prompt. The trouble, of course, is that you can’t directly measure a prompt’s half-life. You get one binary observation, and you don’t get to repeat it, since the practice event changes the future half-life. The sequence of half-lives for an item are correlated, of course, but—still, tricky.

Their approach is to stratify the items into “difficulty groups” based on their initial recall rate taken across the population of users. Then they can fit half-life parameters for subsequent events using pooled groups of users. One can imagine, [[Item response theory]]-style, adding an extra per-user “ability”/“familiarity” parameter as well.

Then the authors introduce a Markov time-series model for describing transitions of half-life and difficulty given a response. This is implemented as an Anki plugin here: [[GitHub - open-spaced-repetition/fsrs4anki: A modern Anki custom scheduling based on free spaced repetition scheduler algorithm]]
