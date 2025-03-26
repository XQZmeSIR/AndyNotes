# COGS 101B - Lecture 8 - Perception

Perceptions are formed from sensory input and _interpretation_ —which depends on past experiences and mental “hardware”. This explains why computer vision is hard: we’re depending on this extra machinery not present in the input.

Sensory input is inherently ambiguous! e.g. Necker cubes, optical illusions. One everyday version of this problem is the “inverse projection problem”: given the 2D image on our retina, what was the depth and shape of the object in the scene? We’re able to recognize objects at any angle, and when they’re blurred and occluded.

To put this another way: we combine bottom-up processing of raw data with top- down processing using models/knowledge/etc.

 **Unconscious inference** (Hermann von Helmholtz): we perceive the objects and events that would be _most likely_ (top-down) to produce the observed stimuli (bottom-up).

See more related notes in:

  * [[Human perception]]

* * *

Q. What’s the “inverse projection problem” in vision? A. Given a 2D projection of a 3D scene, reconstruct the 3D scene.

Q. How does the inverse projection problem illustrate the role of interpretation in perception? A. You can’t reconstruct a 3D scene from a 2D projection without interpreting it through lots of prior knowledge about objects and your environment.

Q. What’s the word superiority effect? A. People can better recognize letters when they’re presented within (real) words than when they’re presented on their own (or within non-words).

Q. What are the implications of the word superiority effect for perception? A. Top-down processing is involved even when trying to recognize individual letters

[[COGS 101B - Learning, Memory and Attention - LE A00 - Course Podcasts - UC San Diego]]
