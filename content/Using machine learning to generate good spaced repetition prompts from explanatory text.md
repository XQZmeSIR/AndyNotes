# Using machine learning to generate good spaced repetition prompts from explanatory text

A challenging research problem. Some notes:

  * [[GPT-4 can often generate usable spaced repetition prompts for declarative knowledge from explanatory text with guidance]]
    * [[In prompt generation, choosing reinforcement targets and writing prompts for those targets are two separate problems]]
    * [[Framing prompt generation as a filtering problem on reinforcement targets]]
    * [[In prompt generation, LLMs may perform better when given prompt-writing principles]]
    * [[In prompt generation, LLMs often need extra hints about what angle to reinforce]]
    * [[In prompt generation, LLMs may perform better with ample context]]
  * [[In prompt generation, LLMs lack prompt-writing patterns for complex conceptual material]]
  * Some simpler subtasks which LLMs can accomplish:
    * [[GPT-3 can generate shallow variations of spaced repetition prompt questions]]
    * [[GPT-3 can transform cloze deletion prompts into question-answer prompts]]
    * [[GPT-4 can probably estimate whether two flashcards are functionally equivalent]]
    * [[GPT-4 can probably estimate whether one prompt will spoil retrieval of another]]
  * [[A dataset of expert-written prompts would help development of prompt generation systems]]

## Other attempts

  * <http://autonki.com> from Sunny Chen at [[OpenAI]]
  * Polar and [[Sana Labs]] use the OpenAI GPT-3 API
    * [[Sana Labs]] [[fine-tunes]] GPT-3 using known-good content/question/answer data
  * [[Ozzie Kirkby]] did some experiments with [[iarfmoose/t5-base-question-generator · Hugging Face]], which is a fine-tuned [[T5]] model.
  * [[Aithal, S. G., Rao, A. B., & Singh, S. (2021). Automatic question-answer pairs generation and question similarity mechanism in question answering system. Applied Intelligence.]] use ProphetNet (fine-tuned on SQuAD) to generate questions from passages and BERT to answer those questions
  * Steuer, T., Filighera, A., Meuser, T., & Rensing, C. (2021). I Do Not Understand What I Cannot Define: Automatic Question Generation With Pedagogically-Driven Content Selection. ArXiv.
    * a BERT-based model with a separate content selection mechanism
    * helpful bibliography
  * <https://www.r-bloggers.com/2024/01/comparing-gpt-4-3-5-and-some-offline-local-llms-at-the-task-of-generating-flashcards-for-spaced-repetition-e-g-anki/>
    * Simplistic prompt design but some methodical evaluation design

## Reading queue

  * A systematic review: Kurdi, G., Leo, J., Parsia, B., Sattler, U., & Al-Emari, S. (2020). A Systematic Review of Automatic Question Generation for Educational Purposes. International Journal of Artificial Intelligence in Education, 30(1), 121–204. <https://doi.org/10.1007/s40593-019-00186-y>

## Graveyard

  * [[Log: experimenting with GPT-3 to generate spaced repetition prompts]]
