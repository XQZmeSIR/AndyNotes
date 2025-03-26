# Simple application prompts can be presented the same way as recall prompts in the mnemonic medium

[[The mnemonic medium can help readers apply what they’ve learned through simple application prompts]]. Such prompts share many features with our existing recall prompts:

  * They can be completed in < 20 seconds
  * They won’t feel terribly effortful
  * They can be self-graded
  * A binary grade is probably sufficient
  * They benefit from the [[Spacing effect]] (albeit possibly with a different schedule)
  * “Progress” can be reasonably characterized as “providing correct answers repeatedly and with increasing intervals of non-study”
  * While [[Application prompts should vary when repeated]], those variations can reasonably be grouped as a single “prompt”/“exercise” entity which accrues progress as its constituents are completed.
    * Note that this requires variations to be mostly fungible—conceptually measuring the same hidden variable.
  * A single prompt won’t be terribly useful, but progress over a few dozen will meaningful learning
  * They benefit from shuffling and batching (again, possibly with different parameters)

Because the experiences of these question types have so much overlap, solutions to the design problems of memory prompts should mostly apply to the design problems of simple application prompts. This suggests that simple application prompts can be presented with little adaptation in the existing review environment of a [[Spaced repetition memory system]].

## Functional differences from recall prompts

From a system perspective, application prompts differ in a few ways from memory prompts:

  * The system should present different question/answer pairs each time ([[Application prompts should vary when repeated]]), grouped within a single “prompt”/“exercise” entity that accrues progress.
  * Such prompts will sometimes need to provide an explanation of how the answer was produced. The explanation’s not “part” of the answer: readers should understand that they’re not meant to make their answer as incorrect if they found it a different way.
  * If readers fail to answer an application prompt, they shouldn’t be asked to retry it in the same session. To maintain variation, the retry attempt would need to show a different question. This would either place a much greater burden on the author or would make the variations cycle much more quickly. Relatedly: unless the grouped “prompt”/“exercise” entity is given its own clear identity, the user will likely interpret the retry prompt as a separate problem, not an opportunity to reattempt a prior problem.

None of these differences is terribly significant.

## Narrative implications for the mnemonic medium

Though the functional differences are relatively small, these prompts force us to change how we describe the [[Mnemonic medium]], how we frame our calls to action, how we narratize progress, and so on.

In practice, this has meant:

  * modifying “almost effortlessly remember what you read” to “almost effortlessly remember and apply what you read”
  * using more general wording in the user journey copy, e.g.:
    * “you remembered” -> “you were able to answer”
    * “remember” -> “correctly answer”
    * “reinforce your memory of the material” -> “reinforce your grasp of the material”
    * etc
