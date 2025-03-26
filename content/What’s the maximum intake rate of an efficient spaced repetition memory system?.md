# What’s the maximum intake rate of an efficient spaced repetition memory system?

Imagine that I add 40 new prompts a day, that I always get all of them right in every review, and that their intervals expand on Quantum Country’s fixed schedule. At the one year mark, I’ll be reviewing:

  * prompts from 5 days ago
  * prompts added 5+14=19 days ago
  * prompts from 19+30=49 days ago
  * prompts from 49+60=109 days ago
  * prompts from 109+120=229 days ago

So in this instance I’d be reviewing 200 prompts. If a six-second average holds, that’s 20 minutes per day. If we insist on a ten minute limit, that gives me a capacity of 100 prompts, which means about 20 new prompts per day.

Because of the exponent, two years doesn’t change much. If I keep adding 40/day, after adding another ~15k in the following year, I’d be reviewing 240 per day (about 24 minutes). If we want to stick to the ten-minute limit, this would mean 17 new prompts per day. A third year adds another 40 daily prompts under these assumptions; a fourth year adds none.

Of course, this is assuming that I get every answer correct all the time. Assuming a 10% error rate, at the 1-year mark I’d be reviewing 241 prompts instead of 200. Not so bad! This brings my 10-minute capacity from 20/day (7.3k/year to 16/day (5.8k/year). With a 5% error rate, it’s 18/day (around 6.5k/year). The difference is substantial enough to be worth pursuing, but it’s not make-or-break. A 20% error rate yields a 13/day throughput (around 4.8k/year).

So to put it another way, if you can decrease the error rate from 20% to 5%, you can add 1/3 more prompts in the same review period.

Note, though, that Quantum Country’s schedule may not be a good reference for optimality bounds: [[Quantum Country users rarely forget after demonstrating five-day retention]]! See also [[Optimizing spaced repetition system schedules]].

    
    
const p = 0.9; const np = 1 - p; const newCards = 40; const ease = 2.5; const max = 365;
    
const queue = [{baseDays: 5, factor: 1}]; let total = 0; while (queue.length > 0) { const {baseDays, factor} = queue.shift(); if (baseDays > max || factor < 0.0001) { continue; } total += factor; queue.push({baseDays: baseDays * ease, factor: factor * p}, {baseDays: Math.max(5, baseDays / ease), factor: factor * np}); } console.log(total * newCards);

Q. In a lifetime, roughly how many items can be learned using a 2020-era spaced repetition memory system? A. $10^6$
