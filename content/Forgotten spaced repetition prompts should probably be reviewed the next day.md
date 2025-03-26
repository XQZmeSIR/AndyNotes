# Forgotten spaced repetition prompts should probably be reviewed the next day

My intuition as an Anki user was that it was much too conservative about lapses, completely resetting the prompt interval. So for [[Quantum Country]] and [[Orbit]]’s schedulers, I just made the item “step back” in its progression instead.

With a couple years of data, I can see that this was pretty clearly a mistake. Assuming that we want to maintain a retrievability rate of 85-90%, we probably do in fact want to next review that prompt on the following day.

The effect is steeper with more lapses, as you’d expect. ![](0E3465C7-DBE7-43D8-89F0-0263A48ED222.png)

Also, the longer intervals on these plots have had more repetitions (since the post-lapse interval is a fraction of the previous interval). If you could compare repetition-for-repetition performance, I expect the curve would be even steeper.

Related/unfortunately: [[Simple spaced repetition algorithms mistreat expected failures]]

This seems also to be true for Quantum Country: [[Quantum Country users who forget in-essay exhibit sharp forgetting curves]] (n.b. this analysis covers just the first lapse—I should look at subsequent lapses, too…)

Relatedly: [[Forgotten spaced repetition prompts should probably have smaller future spacing intervals]]
