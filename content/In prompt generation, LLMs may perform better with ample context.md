# In prompt generation, LLMs may perform better with ample context

Many people have attempted to create systems for [[Using machine learning to generate good spaced repetition prompts from explanatory text]] which operate on highlights. You select a passage, and the model is asked to generate prompts based on the selected text. But unless the selected material is an isolated declarative atom, the model will generally need more context to understand how to generate a good prompt. For example, if you’re selecting a phrase from a textbook, the model needs hints about the level of the textbook, what material has already been introduced, how the idea is being framed, etc. To this end, I’ve found that it helps to provide a few thousand tokens of surrounding text, along with the target itself.

In some sense, this context is doing the job of providing more hints about what’s appropriate for the user; see also [[In prompt generation, LLMs often need extra hints about what angle to reinforce]].

## Example

    
    
<context>Imagine a particle of mass $m$, constrained to move along the $x$ axis, subject to some specified force $F(x, t)$ (Figure 1.1). The program of classical mechanics is to determine the position of the particle at any given time: $x(t)$. Once we know that, we can figure out the velocity $(v=$ $d x / d t)$, the momentum $(p=m v)$, the kinetic energy $\left(T=(1 / 2) m v^2\right)$, or any other dynamical variable of interest. And how do we go about determining $x(t)$ ? We apply Newton's second law: $F=m a$. (For conservative systems - the only kind we shall consider, and, fortunately, the only kind that occur at the microscopic level-the force can be expressed as the derivative of a potential energy function, ${ }^1 F=-\partial V / \partial x$, and Newton's law reads $m d^2 x / d t^2=-\partial V / \partial x$.) This, together with appropriate initial conditions (typically the position and velocity at $t=0$ ), determines $x(t)$
    
Quantum mechanics approaches this same problem quite differently. In this case what we're looking for is the particle's wave function, $\Psi(x, t)$, and we get it by solving the Schrödinger equation: $$ i \hbar \frac{\partial \Psi}{\partial t}=-\frac{\hbar^2}{2 m} \frac{\partial^2 \Psi}{\partial x^2}+V \Psi $$ Here $i$ is the square root of -1 , and $\hbar$ is Planck's constant-or rather, his original constant ( $h$ ) divided by $2 \pi$ : $$ \hbar=\frac{h}{2 \pi}=1.054573 \times 10^{-34} \mathrm{~J} \mathrm{~s} $$ The Schrödinger equation plays a role logically analogous to Newton's second law: Given suitable initial conditions (typically, $\Psi(x, 0)$ ), the Schrödinger equation determines $\Psi(x, t)$ for all future time, just as, in classical mechanics, Newton's law determines $x(t)$ for all future time. $^2$</context>
    
<target>The Schrödinger equation plays a role logically analogous to Newton's second law</target>
    
<hint>how</hint>

With `<context>`: “ **Question:** How does the Schrödinger equation relate to Newton’s second law in terms of their roles in mechanics? **Answer:** Both determine the state of a system at any given time given suitable initial conditions.”

Without: “How is the Schrödinger equation logically analogous to Newton’s second law? **Answer:** The Schrödinger equation relates an evolving quantum state to its environment, just as Newton’s second law relates the motion (acceleration) of an object to the forces acting on it.”

The former is clearly more grounded in the framing presented by the text.
