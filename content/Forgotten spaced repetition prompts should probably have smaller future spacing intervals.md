# Forgotten spaced repetition prompts should probably have smaller future spacing intervals

My naive implementation of a [[Spaced repetition memory system]] scheduling algorithm in [[Quantum Country]] and [[Orbit]] has a constant geometric expansion factor for intervals. I thought: well… maybe that’s fine for most conceptual material.

But after a few years of data from my Orbit reviews, it appears not to be. ![](8BCD0FDF-A27C-4AF0-91C7-17F3EA651522.png) Rows and columns are number of lapses and repetitions since last lapse.

In the top row, we see pretty strong evidence that if a prompt is not forgotten, Orbit’s expansion factor of 2.3 is roughly fine.

In the second row, there was one lapse. We can see in the first column that [[Forgotten spaced repetition prompts should probably be reviewed the next day]]. But also: notice that the recall rates _fall_ with each repetition since the lapse. That’s strong evidence that a 2.3 factor is too large for these prompts.

* * *

I’m not exactly sure what to do about this in the context of a) [[Orbit]], with its binary response feedback; and b) given [[Simple spaced repetition algorithms mistreat expected failures]]. The simplest thing would be to contract the rate on failure, and to recover it slightly with each subsequent success, so that, say, 4 subsequent successes would “make up for” one early failure.

Roughly:

    
    
const baseEFactor = 2.3; const eFactorRecovery = 0.2;
    
function srsFunc(previous, evaluation) { if (previous == null) { previous = {n:0, interval:0, efactor: baseEFactor} } if (evaluation.score < 3) { const efactor = Math.max(1, previous.efactor * 0.75) return {n: 0, efactor: efactor, interval: 1} } else { const efactor = eFactorRecovery * baseEFactor + (1 - eFactorRecovery) * previous.efactor; const newInterval = previous.interval < 1 ? 5 : Math.max(1, previous.interval * previous.efactor); return {n: previous.n + 1, efactor, interval: newInterval} } }

n.b. an important problem with this “low-pass” recovery approach is that it probably behaves backwards from how it should: if you lapse 3 times, you’ll recover to the ease of the second lapse after one correct response, and to the ease of the first lapse after two more, and then only to the original ease after (roughly) 5-6 more.
