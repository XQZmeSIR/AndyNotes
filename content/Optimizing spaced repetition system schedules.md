# Optimizing spaced repetition system schedules

Many papers published along these lines. Collecting some favorites:

  * [[Mozer, M. C., & Lindsey, R. V. (2016). Predicting and Improving Memory Retention: Psychological Theory Matters in the Big Data Era. In M. N. Jones (Ed.), Big data in cognitive science (pp. 34–64).]]
  * [[Ye, J., Su, J., & Cao, Y. (2022). A Stochastic Shortest Path Algorithm for Optimizing Spaced Repetition Scheduling. Proceedings of the 28th ACM SIGKDD Conference on Knowledge Discovery and Data Mining, 4381–4390]]
  * [[Ebisu]] (a solution inspired by Bayesian statistics)
  * [[Comparison]] of contemporary implementations by [[Jarrett Ye]] and collaborators
  * Shu, M., Balepur, N., Feng, S., & Boyd-Graber, J. (2024). KARL: Knowledge-Aware Retrieval and Representations aid Retention and Learning in Students (arXiv:2402.12291). arXiv. <http://arxiv.org/abs/2402.12291>
    * this model cleverly uses BERT-based similarity metrics to parameterize new items

Some of my own notes on the subject:

  * [[Conceptual information may have much slower optimal spaced repetition schedules]]
  * [[Forgotten spaced repetition prompts should probably be reviewed the next day]]
  * [[Forgotten spaced repetition prompts should probably have smaller future spacing intervals]]
  * more: [[Quantum Country data analyses]]

## Queue

  * Tabibian, B., Upadhyay, U., De, A., Zarezade, A., Schölkopf, B., & Gomez-Rodriguez, M. (2019). Enhancing human learning via spaced repetition optimization. Proceedings of the National Academy of Sciences, 116(10), 3988–3993. <https://doi.org/10.1073/pnas.1815156116>
    * derives an “optimal” scheduling algorithm using control theory
  * Settles, B., & Meeder, B. (2016). A Trainable Spaced Repetition Model for Language Learning. Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers), 1848–1858. <https://doi.org/10.18653/v1/P16-1174>
    * “high-life regression” tested at scale on Duolingo
