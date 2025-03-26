# Ngo et al. The Alignment Problem from a Deep Learning Perspective (2023)

> We argue that if AGI-level policies are trained using a currently-popular > set of techniques, those policies may learn to reward hack in situationally- > aware ways, develop misaligned internally-represented goals (in part caused > by reward hacking), then carry out undesirable power-seeking behavior in > pursuit of them.

Q. What example does Amodei et al (2017) give for a RLHF-trained policy which engages in reward hacking? A. A ball-grabbing claw learns to play the claw between the camera and ball in a way which fools human supervisors.

Q. What do the authors mean by situational awareness, citing Cotra (2022)? A. Identifying and applying the most relevant knowledge for their context.

Q. Why do the authors argue that future models will tend to develop situational awareness? A. It will produce higher reward on many RL tasks (e.g. understanding what behaviors human raters want from ML systems).

{situationally-aware reward hacking}: {failure mode in which a policy behaves as intended most of the time, but exploits misspecified rewards only when it predicts it won’t be detected}

{goal misgeneralization}: {failure mode in which a policy that performs well on its training distribution advances some high-level goal outside distribution, but not the intended one}

Q. Empirical example of goal misgeneralize (Langosco et al 2022)? A. Reward given for opening boxes; one key needed per box. During training, boxes outnumber keys; during testing, keys outnumber boxes. Agents try to collect as many keys as they can, even though there aren’t enough boxes to use them on (i.e. they misgeneralize a goal of collecting keys, rather than opening boxes)

Q. What is the inner alignment problem? A. Ensuring that models learn desirable internally-represented goals (in contrast to the “outer” alignment problem of specifying the right rewards)

Q. Three reasons listed why misaligned goals may be rewarded? A. Consistent reward misspecification (e.g. supervisors assigning rewards based on incorrect beliefs); fixation on feedback mechanism (e.g. maximizing the number the supervisor writes); spurious correlations between rewards and environmental features (e.g. the box-key RL example)

Q. Some people hope that an AGI which learns a misaligned goal will also learn some aligned goals which prevent serious misbehavior. What problem do the authors raise? A. The nearest unblocked strategy problem: any loopholes in those aligned constraints will likely be exploited.

The {nearest unblocked strategy} problem: an AI which {strongly optimizes for a (misaligned) goal will exploit even small loopholes in (aligned) constraints}. e.g. {in a model which has learned a goal of honesty and of making money, any small deviation between the learned honesty goal and our honesty concept will likely be exploited, to find policies which it classifies as honest (which we would classify as dishonest)—because those policies will often /make more money than their neighbors}

{instrumental convergence thesis}: {there are some subgoals that are instrumentally useful for achieving almost any final goal (e.g. survival, acquiring resources, preserving its goals)}; i.e. many goals incentivize {power-seeking}

Q. Why do the authors argue that goals which motivate power-seeking would be reinforce during training? A. A situationally-aware model would likely identify instrumental strategies like “achieve high reward so that it is deployed widely, and so that its goals are not changed”

Q. What two categories of threat model do the authors discuss? A. assisted decision-making (mass-deployed AGI systems manipulate users, are delegated more responsibility until they effectively control institutions); weapons development (drug development AI synthesizes toxins)

Q. What historical precedent do the authors suggest for the threat model of assisted decision-making? (i.e. mass-deployed AGI systems manipulate users, are delegated more responsibility until they effectively control institutions) A. multinational corporations subverting governments of small countries
