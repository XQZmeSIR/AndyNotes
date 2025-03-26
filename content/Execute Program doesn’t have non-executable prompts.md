# Execute Program doesn’t have non-executable prompts

[[Readers answer Execute Program’s prompts by executing a program]]. [[Execute Program]] doesn’t have any other types of prompts.

For example, a lesson on regular expressions might have this prompt:

> Q. What’s the output of `/a..b/.test(“a\ncb”)`? > A. `false`

The reader would answer this prompt by actually inputting `false` into the REPL and executing the expression.

That lesson couldn’t also have this more typical [[Spaced repetition memory system]] prompt:

> Q. What character(s) _doesn’t_ `.` match (in many implementations)? > A. `\n`

Lessons which are primarily conceptual (e.g. [[SQL Constraint Analysis]]) don’t fit well into this model.

Because Execute Program has just one prompt type: [[Execute Program’s prompts act both as application prompts and recall prompts]].

* * *

Q. What’s an example of a prompt which [[Execute Program]] can’t encode? A. [e.g. “Q. What’s the difference between `*` and `+`? A. `*` permits zero matches”]()

Q. Why can’t [[Execute Program]]’s SQL constraint analysis lesson make use of its spaced-repetition system? A. That lesson is mostly conceptual, and its ideas are difficult to encode as executable expressions.

* * *

## References

Conversation with Gary Bernhardt, 2020-03-24
