# GPT-4 can probably estimate whether two flashcards are functionally equivalent

In my simple tests so far, it seems that [[GPT-4]] could be used to assess [[Large language models]]-generated prompts versus a human benchmark (i.e. for [[Using machine learning to generate good spaced repetition prompts from explanatory text]]).

    
    
I’m going to provide you with the text of two spaced repetition flashcards, which we’ll call A and B. Please provide a Likert rating for the following statement: “Practice of Flashcard A and Flashcard B will promote retrieval of the same knowledge.”
    
Flashcard A: Q. Explain the relationship between the role of Newton's second law and the Schrödinger equation. A. Just as Newton's law lets us solve x(t) given initial conditions, the S.E. lets us solve for the wave function. Both are used to tell us essential properties of the particle's behavior (but we don't understand this well yet).
    
Flashcard B: Q. How does the Schrödinger equation's role in quantum mechanics compare to Newton's second law's role in classical mechanics? A. Both are logically analogous, as they determine the future state of a system given initial conditions.
    
---
    
Likert rating: 5 - Strongly agree. Both Flashcard A and Flashcard B focus on the comparison between the Schrödinger equation and Newton's second law, highlighting their roles in determining the future state of a system given initial conditions. Practicing these flashcards will promote retrieval of the same knowledge, as they address the same core concept.

This will need some refinement to e.g. test whether the two prompts expect the same answer. These two flashcards will probably result in the same retrieval, but the answer of the first one is off target relative to the second, so it won’t do the same job in practice of reinforcing that answer.

    
    
Flashcard A: Q. Explain the relationship between the role of Newton's second law and the Schrödinger equation. A. They’re both important equations for students to memorize in classical and quantum physics courses, respectively.
    
Flashcard B: Q. How does the Schrödinger equation's role in quantum mechanics compare to Newton's second law's role in classical mechanics? A. Both are logically analogous, as they determine the future state of a system given initial conditions.

Here’s one try at a refinement:

    
    
I’m going to provide you with the text of two spaced repetition flashcards, which we’ll call A and B. Please provide a Likert rating for the following statement: “Practice of Flashcard A and Flashcard B will promote retrieval of the same knowledge; the feedback provided by comparing one’s own answer to the answers to A and B will reinforce the same knowledge.”

The original prompt gets a Likert rating of 4; the revised one gets a 2.

Refining again:

    
    
I’m going to provide you with the text of two spaced repetition flashcards, which we’ll call A and B. Please provide a Likert rating for the following two statements: S1. “Practice of Flashcard A and Flashcard B will promote retrieval of the same knowledge” S2. “The feedback provided by comparing one’s own answer to the answers to A and B will reinforce the same knowledge.”

Inexplicably, this produces 4/4. Clearly this will need some iteration, and I’ll want to do some validation with manual ratings to make sure I consistently agree with its assessment.s
