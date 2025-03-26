# Missed answers in Execute Program’s reviews don’t penalize the student unless they “give up”

[[Execute Program]]’s [[Spaced repetition memory system]] prompts are machine-graded, so if readers make semantically-unimportant typos in their responses, the system marks the prompt wrong. These false negatives can be quite annoying, particularly since [[Execute Program’s lessons don’t unlock until you’ve successfully reviewed their prerequisites]]. In the SQL course, the false negative rate is high enough that in early 2020, the system was changed so that incorrect responses no longer “count” as failing, so long as the student eventually produces a correct answer. Readers can try as many times as they want, and the next review’s interval will still increase according to the SRS curve. Subsequent lessons unlock irrespective of user performance.

If a user can’t produce an answer, even after several tries, they can finally “give up” to see the correct answer. If they give up in this way, then the question’s interval decreases as usually occurs for forgotten answers in SRS.

See [[Self-graded spaced repetition memory systems avoid false negatives]] and [[Self-grading vs. machine-grading in spaced repetition memory systems]].

* * *

## References

  * Conversation with Gary Bernhardt, 2020-03-24
  * Email with Gary Bernhardt, 2020-04-07. [[Re: Progress mechanics for spaced memory systems]])
