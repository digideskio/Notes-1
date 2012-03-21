Physics 112: Statistical Mechanics
==================================
January 18, 2012
----------------

Organization
-----------
Goals
 * Deeper understanding of concepts: less mysterious.
   + Entropy
   + Free energy
   + Chemical potential
   + Statistical mechanics
	  - Fluctuations
	  - Kinetic theory background ← use of simulations
   + Recognition of physics in a "context-rich" situation, i.e. real life.
 * Acquire computational tools
   + Quantitative
   + Problem-solving skills
 * Linkages to
   + everyday life
	 - bridge between microscopic and macroscopic
	 - irreversibility
	 - engineering
   + modern physics
	 - frontier
	 - applications e.g. astronomy, cosmology
	   · condensed matter physics, low temperature
   + History

Participation
 * Focus: Conceptual Understandidng
   + We learn by construction/reconstruction of your mental models.
   + This process is both intensely personal and social (learn through
	 others)
   + focus on grades, formulae, short cuts
 * Before lecture
   + Read book and notes because our use of clickers which decreases
	 the in-class presentation time, there will be testing of this
	 reading.
   + Play with applet simulations → intuition. (You can suggest others
	 you can find)
* In class
  + Beginning of class: typically a conceptual question/applet
  + Peer instruction questions:
	- A conceptual question
	- Vote (with clickers)
	- Discussion in small groups
	- Vote again
  + Active participation during lecture: questions, clickers
  + "One minute" random quizzes (check attention to the material)
* Out of class
  + Homework
  + Working groups on problems if you like (but you write your own
	solution)
  + Discussion sections (but try homework first)
  + Office hours (come with questions)

Clickers:
* Systematic use in class begins Mon, Jan 23.

[ More boring administrative stuff; not particularly unique to this
  particular class. Largely duplicated from the syllabus. ]

[ note to self: 277 Cory ]
Physics 112: Statistical Mechanics
==================================
Kinetic Theory 1 / Probabilities. January 23, 2012
--------------------------------------------------
Details:
 * clickers
 * homework -- due in LeConte reading room
 * webcasts
 * Discussion sections

Ideal Gas
 * particle interaction leads to thermal equilibrium.
 * particle probability distributions are independent
 * particle systems where interaction time ≪ mean free time between
   collisions

Motivations: statistical mechanics and fluctuations
===================================================
The need for statistical mechanics
----------------------------------
How to describe large systems.
------------------------------
 * very large
 * at finite temperature – not at rest
   + velocity v ≈ 300m/s @ 300K.
 * Constant collisions
   + mean free path λ ≈ 0.1 μm.
 * Probabilistic description. 1 particle
   + Classically
	 - Have to track both position and velocity/momentum.
	 - We will introduce a phase space. The probability distribution
	   on phase space = position × momentum.
	 - Problem is that states are treated as continuous.
   + Quantum – states are actually discrete / countable.

N particles
-----------
In many cases it is a good approximation to treat particles as
independent. We will call this an ideal gas.

Temperature, pressure, entropy
------------------------------

Temperature as a measure of mean energy of excitations of the system. Two
reasons: 1) usually more degrees of freedom than spatial degrees of freedom
(spin (e.g. ferromagnetism), and 2) other effects: quantum gas: Fermi-Dirac
exclusion principle (i.e. we cannot put two particles in the same state)
means that we have to stack in energy. Their mean energy is very large,
even at 0K.

Pressure as a measure of energy density or "average" force per unit area on
walls of container.

Entropy as a measure of the state of disorder of a system. Modern
definition: σ = -∑pi log(pi). 0 if in one state, max if flat distribution.
Physics 112: Statistical Mechanics
==================================
Kinetic Theory 2 / Probabilities. January 25, 2012
--------------------------------------------------
# House keeping.
# Fast introduction to kinetic theory.
 * Equilibrium
 * Vibrations
# Probabilities.
 * Distributions
 * Moments

How a system reaches equilibrium
================================

Diffusion. True also in probability space. An isolated system tends to
evolve toward maximum flatness.

We won't speak classically of position + momentum, but rather of
states. Quantum states. The same thing happens in the case of probability.

It turns out that when all the properties are equal, we have maximum
entropy. Equilibrium occurs when "you are maximally flat".

Fluctuations
============

Fluctuations are the effect of life if you don't have an infinite number of
degrees of freedom. Which never happens. One of the fundamental properties
is noise. Noise is intrinsic to the finity of degrees of freedom.

Central limit theorem. Fluctuations decrease as samples increase.

Probabilities
=============

Probabilistic event: occurs in an uncontrolled manner, described by random
variables. parameters are fixed (even if unknown).

# Discrete case
 * consider bins.

An example of discrete probabilities is a histogram. Raw counts.

Cannot determine probabilities via experiments. Probability distributions
add up to 1. Probabilities cannot be negative.

# Continuous case
 * Actually a lie.

Moments. Stuff.
Physics 112: Statistical Mechanics
==================================
Kinetic Theory 3 / Probabilities. January 27, 2012
--------------------------------------------------

Various probability stuffs. Continuous distirbutions. Sum/average of
independent events. Central limit theorem.

  P(s) ≥ 0, ∑ P(s) = 1
  〈y〉 = ∑y(s)P(s) [ this is the first moment. ]

  y(s) = 35 δ{i,k}. 〈y〉 = ∑ 35δ{i,k} = 35/38.

Variance:
  σ² = 〈(y(s) - 〈y〉)²〉 = 〈y²〉 - 2〈y〈y〉〉+ 〈y〉² = 〈y²〉 - 〈y〉²

root mean square (rms) ≡ standard deviation

Independence. Usually, if I have two random variables, x and y, the
probability of P(x,y) = P(x|y)P(y) ≠ P(x) × P(y). We say we have
independence iff P(x,y) = P(x)P(y). In other words, P(x|y) = P(x).

You can define a correlation coefficient to be
  (x - 〈x〉)(y - 〈y〉)/(σxσy).

Independence ⇒ ρ = 0. Converse not necessarily true.

Continuous distributions. Histograms. The case where a variable is
continuous. We now have probability _densities_.

  f(x)dx = g(y)dy = f(x,y)(dx/dy)dy.
  f(x) ≥ 0, ∑f(x)dx = 1.

Moments: we can define moments in exactly the same way as before.
The moment of a variable y(x)

〈y(x)〉 = ∫y(x)f(x)dx.
  μ = 〈x〉 = ∫xf(x)dx.
  σ² = 〈x²〉 - 〈x〉² = ∫x²f(x)dx - (∫xf(x)dx)².

f(x,y)dxdy = g(x)dx h(y)dy. Factoring works the same way, if our
variables are independent.

Normal distributions: Gaussian.

It is very important to put the differential element (dx or dy) because the
function changes depending on what the differential element is. The
histogram depends on what variable you choose to plot. If I choose x or x²,
my histogram will be different. Usually.

The mean is in the middle of a normal distribution because the third
moment is 0.

Full-width half maximum (FWHM) ≈ 2.3σ

A is called the mode, i.e. the maximum. In a distribution with nonzero skew
(like the Maxwell-Boltzmann), the mode is different from the mean.

mean: location.
standard deviation: width.
skewness: symmetry.
kurtosis: peakedness.

Fourier transform is the characteristic function. The log of this is stuff
with cumulants.

Sum of random variables:
x ≡ y + z
〈x〉 = 〈y〉 + 〈z〉.
σ²x = σ²y + σ²z + 2ρσyσz.
Independence ⇒ ρ = 0; σ²x = σ²y + σ²z

h(x)dx = (f*g)(x)dx ⇒ the cumulants add!

Proof: Convolution in original space is equivalent to product in Fourier
space. Hence for a sum, the characteristic functions multiply and the logs
of characteristic functions add.

Central limit theorem: Cool if our variables actually are independent.
Physics 112: Statistical Mechanics
==================================
Entropy and Stuff. January 30, 2012
-----------------------------------
Homework
========
First one is due today, second one is posted.

Central Limit Theorem
=====================

Taking N independent random variables x{i} of average μ₀ and of variance
σ₀², the experimental average A = (1/N)∑x{i}.  f(A)dA →(N→∞)
1/(√(2π)σ)exp(-(A-μ)²/2σ²)dA; μ = μ₀, σ² = σ₀²/N.

This is different from 〈A〉, which would just be an integral.

The other thing is that σ² = σ₀²/N. The variance decreases as 1/N, or the
standard deviation decreases as 1/√N. This is fairly typical of stochastic
processes, where the relative width decreases as 1/√N. Overall width will
increase if you don't normalize, but relative width decreases.

The relative widths of kurtosis and skewness go to zero as we add more
terms.

Consequences for Thermodynamics
-------------------------------

Because of large number of particles, averages are very peaked around mean.
 * System well characterized by mean = ",macroscopic quantity".
 * Fluctuations are very small.
 * Not a lot of difference between most probable value, mean value,
   and experimental value.

Dealing with systems with large degrees of freedom. Temperature, for
instance, is related largely to the kinetic energy of the particles. It
will be very well-defined and have very few fluctuations if we are just
measuring the mean of said particles, and it will be very peaked around the
mean.

The central limit theorem makes thermodynamics meaningful.

Quantum States of a System
==========================
States of a System
------------------
Not covering spins. ALso, marginal definition of entropy.

(mostly chapters 1 and 2 of Kittel and Kroemer)
 * States / COnfigurations
 * Probabilities fo States
   + Fundamental assumptions
   + Entropy
 * Counting States
 * Entropy of an ideal gas.

State = Quantum State.
 * Well-defined, unique.
 * Discrete ≠ "classical thermodynamcs" where entropy was depending on
   resolution ΔE.

Boltzmann for reasons that he did not fully understand arrived at the
conclusion that he had to have discrete states. This was before Planck and
quantum mechanics. Boltzmann was always doubting himself to the point that
he took his own life. So when you are a little bit despaired, think about
Boltzmann.

It's amazing that a guy like that who contributed so much to modern physics
was unsure of himself.

Configuration = Macroscopic specification of system
 * Macroscopic Variables
   + Extensive: U, S, F, H, V, N (not normalized)
   + Intensive: T, P, μ (chemical potential)
 * Not unique: depends on level of details needed.
 * Variables + constraints ⇒ not independent.

Many microstates (states) correspond to a single macrostate
(configuration).

Quantum Mechanics in 1 transparency
-----------------------------------
Fundamental postulates
 * State of one particle is characterized by a wave function.
 * Probability distribution = |Ψ(x,t)|^2 with 〈Ψ|Ψ〉 = ∫{Ψ(x)*}Ψ(x)dx = 1.
 * Physical quantity → Hermitian operator.
 * In general, not fixed outcome. Expected value of Ô = 〈Ψ|Ô|Ψ〉.
 * Eigenstate ≡ state with a fixed outcome e.g. Ô|Ψ〉 = o|Ψ〉, where o
   is a number.
 * A finite system has discrete eigenvalues.

1-dimensional case, infinitely deep square well. Solve via separation
of variables, construct Fourier series.

If you solve this equation, you can show that in that case, the wave
function has to go to 0 at the wall.

That's just a particle in a box. If you ask yourself what is the momentum
of this particle, this particle is actually a series of two momenta. It
does not have a well-defined momentum, since it is going back and forth.
Physics 112: Statistical Mechanics
==================================
Entropy and Stuff. Feb 1, 2012
------------------------------

REMINDER: states ⇒ microstates; configurations ⇒ macrostates.

Overview:
 * Discrete states
 * Isolated system in equilibrium

Postulate; H theorem. One of the finest works in physics by
Boltzmann. Shows that entropy is increasing. The probability distributions
of the states tend to equalize. Whatever initial probabilities tend to
evolve toward equilibrium.

 * Counting states

Quantum Mechanics (again)
=========================

Particle in a box (or, if you like, an infinite square well). By the axioms
of quantum mechanics, these solutions are identical to the modes of a
vibrating string.

[ clicker question regarding distance between momentum states. Talk
  about Uncertainty principle. ]
ℏ/2L: distance between momentum states.

quantization comes from the combination of both the eigenvalue equation as
well as the specific boundary conditions.

Same thing happens with a hydrogen atom. We have an electron orbiting
around the photon, and Bohr said that if you turn the nucleus by 2π, your
function should come back on itself. And then if you solve the radial
Schrödinger equation, it is the solution where you have something finite at
the origin and 0 at infinity which gives the quantization of energy.

Basically resonance conditions, like a vibrating string, will give us
discrete energy levels.

SPIN
====

Particles can carry a spin – a unit of angular momentum. Actually, they can
carry an angular momentum. Carrying integers and half-integers of angular
momentum – former are known as fermions, and latter are known as
bosons. Very different.

If I have a spin of 1, it can point up, nowhere, or down. The photon, which
is massless, is spin 1 with 2 spin states. (exception: usu. spin s ⇒ 2s+1
states.)

ε = mB, where m = magnetic moment, B = magnetic field. emission of photons,
directions of spin.

Important implication in medicine: MRI is the magnetic resonance
imaging. Uses this property to see where the spins of the hydrogen
are. Just looking at hydrogen, basically.

Energy now is is proportional to r².

Fundamental postulate
=====================

Probabilistic description of state of a system.

Systems in equilibrium. An isolated system in equilibrium is equally likely
to be in any of its accessible states. Kittel does not specify in
"equilibrium". It does not matter if we are close to equilibrium.

Consequences
------------

Probability of a configuration:
 * Probability of configuration: simple counting problem, normalized.

This allows us to compute probabilities of configurations. This method is
conventionally called a microcanonical computation. Characterized by being
very awkward, cumbersome, difficult to implement, and so on.

Entropy
=======

σ = -∑p log p= -H. H = Negentropy = Information (Shannon).

For an isolated system in equilibrium: identical to Kittel. In classical
thermodynamics, definition usually used is dQ = TdS.

Basically, we have a nondeterministic finite-state machine (weighted
probabilities and all) being run many times simultaneously. H theorem tells
us it will reach equilibrium i.e. all currents will cancel.

Γ{rs} = Γ{sr} ⇒ H theorem. Symmetry of the transition rate will cause the
evolution of the probabilities to converge eventually to a flat
distribution (_of microstates_). Else you have a nonzero divergence in more
than one state.

Sterling approximation: number of states goes to a gaussian.
Physics 112: Statistical Mechanics
==================================
Entropy and Stuff. Feb 3, 2012
------------------------------

homework #2:
exp(u² - 2ρuv + v²) ⇒ exp(u² + (v-ρu)² - ρ²u²)

Counting States: Discrete States
================================

With just counting states and some assumptions as to what pressure and
temperature are, we have PV = NkT and U = 3NkT/2.

Density of spatial states per unit phase space
----------------------------------------------

Phase space: Position space (x) ⊗ (p) Momentum space.

Density of quantum states (orbital states) is 1/ℏⁿ per particle (n ≡
dimensions). That is, if I have a volume in the phase space, I can count
the number of orbital states for one particle by dividing this volume by ℏ³
(in three dimensions).

The volume of the phase space is just the integral of (1/ℏ³)d³xd³p.

Ideal Gas
---------

Now consider N particles in weak interactions. Total energy U is
constant. g = ∏∫d³xd³p/ℏ³ⁿ. Insert a δ(∑p{i}²/2M - U). Basically imposing
that the total energy of my system is U. The product of dx{i} will give
Vⁿ. So there is no problem there. But what about the d³p{i}δ(∑...)?
Imposing some of the p{i}²/2n to be equal to U. I'm looking now at the
surface of a sphere with a certain radius.

If we have one particle in one dimension, we have only one momentum
space. In large dimensions, g ∝ VⁿU^{³⁽ⁿ⁻¹⁾/₂}/h³ⁿ.

[ Reasoning: for momentum integral: we need to conserve energy. ]

[ We are basically speaking of the surface of a volume in 3N-space. ]

σ = S/k = log(g) = log(VⁿU^{³ⁿ/₂}) + constant
  = nlog(V) + 3Nlog(U)/2 + constant.

In that case, can write dU = TdS - pdV. Or, if you prefer, τdσ - pdV.

Solve for U: U = Aexp(2σ/3N)V^{⁻²/₃}.

τ = ∂U/∂σ = 2U/3N ⇔ U = 3NkT/2.

p = -∂U/∂V = 2U/3V ⇔ pV = Nτ ≡ NkT.
Physics 112: Statistical Mechanics
==================================
Entropy and Stuff. Feb 6, 2012
------------------------------

[[ Talk about clickers. ]]

So far:
-------
σ = -∑\p log p   ✓

H theorem: with an isolated system, probabilities of states evolve to being
equal.

Consequence of the H theorem: If I am looking at the probability of a
configuration, the probability is equal to (states in configuration) /
(total states)

σ = log (g{t}) (mathematically equivalent to the first statement)

Counting of states to get the entropy.

Density of orbitals (quantum spatial wave functions) in phase space is
1/ℏ**{d} (dimension of space)

Once again: phase space ≡ position space (x) ⊗ (p) momentum space. Good way
to compute the number of spatial states. degrees of freedom (spin,
rotation, vibration).

Number of states g(spatial states) of a system of energy U in a volume
V is g ∼ U^(³ⁿ/₂)Vⁿ = exp(σ). τ ≡ kT, σ ≡ S/k
τ = ∂U/∂σ)y ⇒ U = (3/2)Nτ
P = -∂U/∂V)σ ⇒ PV = Nτ

Just as natural, if not more so, to work with σ(U,V) ≡ log(VⁿU^(³ⁿ/₂)).

**We must be careful to note, when working with partial derivatives,
  which variables we are keeping constant.**

This is a very useful way of defining pressure and temperature once we have
counted states.

τ = 1/(∂σ/∂U)V,n, p = τ∂σ/∂V)U,n

We were starting with the phase space for our n particles. d³ⁿxd³ⁿp/(ℏ³ⁿ):
density of our states. We want to then integrate over the volume, but we
choose the states such that U fixed. Represents in our 3n-dimensional
momentum space a sphere.

δ[√(∑∑p²{ik}) - √(2MU)]. Take advantage of filtering effect of δ.

radius of sphere in 3N momentum space. r has dimension r^{d-1}. In the
general case, we'll have Ω³ⁿr³ⁿ⁻¹.

Thus we have Ω√(2MU)³ⁿ⁻¹/ℏ³ⁿ.

δ has dimension of 1/p. ∫δ(x)dP = 1

Sackur Tetrode formula: entropy of an ideal gas. S/k = N(log(n₀/n) + 5/2)
Physics 112: Statistical Mechanics
==================================
Entropy and Stuff. Feb 8, 2012
------------------------------

Divide g{t} by a missing N!, which is from indistinguishability of
particles / quantum states. Also, experiments were off by a very large
factor.

g{t} = Ω{3N}√(2MΔU)V^{N}U^{3(N-1)/2}/(N!ℏ^{3N})

Quantum density. What remains of our counting states.
σ = N(log(n{Q}/n+5/2).
n = N/V, n{Q} = (2πM/ℏ² 2U/3N)^{3/2}

Free expansion of gas (isolated system ⇒ no particle/heat exchange): final
temperature = initial temperature.

Entropy is increasing, however, since volume is increasing.

Chapter Three:

Equilibrium, Thermodynamics, Potential
======================================

RECALL:

1/τ =  ∂σ/∂U|V,N
p/τ =  ∂σ/∂V|U,N
μ/τ = ­∂σ/∂N|U,V

For an ideal gas in 3space:
U = (3/2)Nτ
τ ≡ kT
pV = Nτ

States of a combination of two systems
--------------------------------------

Take 2 systems and put them in contact.

Put them in weak interactions U = U₁ + U₂, V = V₁ + V₂, N = N₁ + N₂

Number of states g₁(U₁,V₁,N₁), g₂(U₂,V₂,N₂). Weak interaction ⇒ quantum
states are not modified.

How many states do we have in the combined system?
g₁g₂

What is the configuration of maximum probability? The number of states in
g(U₁,V₁,N₁)/g{t}. Take a derivative with respect to U₁ to see where the
extremum of this function is.

∂g₁/∂U₁ g₂ + g₁ ∂g₂/∂U₁ ≡ 0.
∂g₁/∂U₁ g₂ - g₁ ∂g₂/∂U₂ = 0.
(¹/g₁)∂g₁/∂U₁ = (¹/g₂)∂g₂/∂U₂.
∂log(g₁)/∂U₁ = ∂log(g₂)/∂U₂.
∂σ₁/∂U₁ = ∂σ₂/∂U₂.
1/τ₁ = 1/τ₂.
Physics 112: Statistical Mechanics
==================================
Equilibrium, Thermodynamics, Potential. Feb 10, 2012
----------------------------------------------------

# Midterm
# Equilibrium between two two systems
# Laws of Thermodynamics

At the end of last lecture, we were considering two systems which can
exchange energy, volume, particles. We were asking ourselves what was the
most probable configuration U₁,V₁,N₁. ∂σ₁/∂U₁ = ∂σ₂/∂U₂ ≡ 1/τ. Similarly,
∂σ₁/∂V₁ = ∂σ₂/∂V₂ = p/τ. ∂σ₁/∂N₁ = ∂σ₂/∂N₂ = -μ/τ (μ for one species) –
definitions.

The configuration of maximum probability share the same pressure,
temperature, potential.

The important thing is that the distribution of the system around this most
probable configuration is very peaked and becomes more peaked as we get
more particles (see central limit theorem).

Did not put volume because it is difficult to define walls.

The last point I wanted to make: by putting the system in contact, we have
increased the entropy of the system. That we know from the H theorem.

What Kittel and Kroemer say is approximately correct. "Entropy increases
because most probable configuration by default is greater than what you
started with before". This is approximate because they are speaking about
the most probable configuration.

σ{max} < σ; σ{max} ≈ σ (very very close, though, because our probability
distribution is very peaked. This is why Kittel and Kroemer is merely an
approximation)

In practice, it does not really matter, since this is a good enough
approximation for the systems that we work with: σ-σ{max} ≪ σ =
N(log(n{Q}/n)+5/2) [Sackur tetrode formula].

Kittel & Kroemer does recognize that, but it is presented in a slightly
confusing manner.

We have shown that indeed the temperature behaves as the temperature we
know. We have not yet shown that this is the same pressure.

Chemical potential affects various things such as rates of
diffusion. Determined by species of particles. However, at equilibrium, by
the H theorem, the chemical potential is equal in all accessible states.

What is chemical potential? It is a measure of the concentration! (verify
by working out -τ ∂σ/∂N). A lot of work for a very simple result. But this
is much more powerful. We will use this to look at batteries, equilibrium
in various systems.


MIDTERM: Friday the 24th. 8:10-9:00. Why Friday and not Monday? Turns out
there is an important workshop on dark matter in UCLA. There is a potential
problem: Monday the 20th is President's day, so no class, no office
hours. Proposition: Tuesday the 21st, we have extended office hours from
4:00-6:00.

Alex's review sessions: Wednesday 15th (5-6), Wednesday 22nd (6-8).

You should take this midterm seriously but not panic too much about it. I
will also give you, next week, maybe before Wednesday, a small diagnostic
quiz that allows you to see where you are.

BACK TO THERMO.

Thermodynamics were developed over a century and a half from the late 1700s
to the early 1900s. Basically, by the beginning of the twentieth century,
there was this concept of three laws of thermodynamics (actually 4: the 0th
law says that at equilibrium, pressure, temperature, chem. potential are
equal).

The first law comes directly from our definition

dσ = 1/τ dU + p/τ dV -∑μ/τ dN. Now, I can multiply by τ and we get
dU = τdσ - pdV + ∑μdN: change in energy = heat - work + chemical work

You can have many different expressions, but basically, this is a
consequence of our definition.

Second law of thermodynamics: when an isolated system evolves from a
non-equilibrium configuration to equilibrium, its entropy will increase.

Third law: entropy is zero at zero temperature (or log of number of states
occupied) ⇒ method to compute entropy.
	If there is only one ground state, at zero temperature, all of the
	particles will be in this ground state (not fermions) and there is only
	one state. p₀ = 1; p{i} = 0 ⇒ σ = 0. If there are several ground
	states, this is degenerate; you will have a log g, where g is the
	number of ground states.

Fermions: all of particles cannot be in the ground state. What you should
remember is that at zero temperature, there is one (or several) ways to put
all of the particles.

Thermodynamic identities. Rewrite slides in different ways depending on
what are your independent variables.

How do we measure entropy experimentally? There is a problem with assuming
ideal gas: not valid close to absolute zero. For that matter,
Sackur-tetrode is not valid at absolute zero. The classical approximation
breaks down when n > n{Q}.
Physics 112: Statistical Mechanics
==================================
Macroscopic Thermodynamics. Feb 13, 2012
----------------------------------------------------

Nader Mirabolfuthi. 343 Old LeConte. 12-1p.

Review of some thermodynamics concepts, laws and applications.
Thermodynamic functions: Maxwell relations
Heat engines, refrigerators: Carnot cycle.

dQ = dE + dW.

The laws of thermodynamics were developed by people who didn't use
statistics.

equilibrium: A↔B.

0th law: equilibrium. 1st law: energy (heat in the form of energy). 2nd
law: entropy of isolated system increasing.

An exact differential is a well-defined function in terms of multiple
variables x and y. Very important feature: conservative vector
field. Internal energy is actually a state function of the system, whereas
heat and work can be added arbitrarily. Place bars to denote non-exact
differentials.

PV = nτ: equation of state: relates observables with the system (pressure,
volume, temperature).

pV = νRT, TdS = pdV + dE. Therefore dS = P/T dV + dE/T. Since E = E(T,V),
dE = ∂E/∂T dT + ∂E/∂V dV. So dS = nR/V dV + 1/T (∂E/∂T dT + ∂E/∂V dV).

So dS = (νR/V + 1/T ∂E/∂V)dV + 1/T ∂E/∂T.

S = S(T,V). Also a state function. So we can write dS, therefore, as:

∂S/∂T dT + ∂S/∂V dV = ... ⇒ ∂S/∂T = νR/V ∂E/∂V + 1/T; ∂S/∂V = 1/T ∂E/∂T.

Working through the math,

∂²S/∂V∂T = 1/T² ∂E/∂T + 1/T ∂E/∂V∂T = 1/T ∂E/∂V∂T.

Specific heats: ∂Q/∂T while holding various parameters constant.

Adiabatic vs. isothermal expansion. γ ≡ C{p}/C{v}.
Physics 112: Statistical Mechanics
==================================
Macroscopic Thermodynamics. Feb 15, 2012
----------------------------------------

Recap of last time: we proved that the internal energy of an ideal gas was
a state variable.

Maxwell relations and their proof: from τdσ = dU + pdV,
	* U = U(σ,V) ⇒ dU = τdσ - pdV
	  + Internal energy
	* H = H(σ,P) ⇒ dH = τdσ + Vdp
	  + Enthalpy
	  + H = U + PV
	* F = F(τ,V) ⇒ dF = -σdτ - pdV
	  + Helmholtz free energy
	  + F = U - τσ
	* G = G(τ,P) ⇒ dG = -σdτ + Vdp
	  + Gibbs free energy
	  + G = U - PV + τσ

exact differential: f = f(x,y) ⇒ df = (∂f/∂x)dx + (∂f/∂y)dy.

For an ideal gas, we found C{p} - C{v} = k{B}N{A}. But C ≡ dQ/dt. If Q or T
were exact differentials, regardless with which path they took, we should
have had the same dQ/dT. The same for work because the first thermodynamic
law combines heat and work, and energy is an exact differential.

∂τ/∂V = -∂p/∂σ
dU = τdσ - pdV. U ⇒ dU = (∂U/∂σ)∂σ (∂U/∂V)∂V.

A necessary condition for an exact differential is that the derivatives
commute. In other words, _take the curl_.

More relations:

∂τ/∂V = –∂p/∂σ
∂τ/∂p =  ∂V/∂σ
∂σ/∂V = –∂p/∂τ
∂σ/∂p = –∂V/∂τ

We just get these from various formulations of first law of thermo (U, H,
F, G): by virtue of being exact differentials, their derivatives commute.

General relations for the specific heat:

C{V} = (∂Q/∂τ){V} = T(∂σ/∂τ){V}
C{p} = (∂Q/∂τ){p} = T(∂σ/∂τ){p}

Thus C{v} = C{p} + τ(∂σ/∂P·∂P/∂τ)

lpha ≡ 1/V ∂V/∂τ. "volume coefficient of expansion"

κ ≡ -1/V ∂V/∂p "isothermal compressibility"

Therefore C{p} - C{v} = Vτ(lpha²/κ)

What's needed to calculate entropy

Use the relations shown in the previous part. All we need are C{v} and
equation of state. But C{v} is also computable using equation of state at a
given V₀.

σ(τ,V) = σ(τ₀,V₀) + ∫C{v}(τ′,V)dτ′/τ′ + ∫dV′(∂P{v}(τ₀,V′)/∂τ)

Same for internal energy.

dU = C{v}dτ + (τ∂P/∂τ - P)dV
∂U/∂τ = C{v}
∂U/∂V = τ∂P/∂τ - P.

Example van der Waals gas (particle interactions):
(P + a/v²)(v-b) = k{B}N{A}τ (v ≡ V/ν
Physics 112: Statistical Mechanics
==================================
Applications of Classical Thermodynamics. Feb 17, 2012
------------------------------------------------------

Heat engines, refrigerators, and Carnot cycle
---------------------------------------------
Historically very important: industrial revolution. Easy to do mechanical
work and transform to heat: mechanical, electrical. What about the
opposite? Not at the expense of machine itself: otherwise no cyclic.

Also has interesting physical importance: this was a new thing: how to
study energy? Joule showed there was an equivalence between work done and
heat released.

η = w/q₁ ≤ 1 - τ₂/τ₁. Equality holds only for quasi-static.

Carnot cycle: alternating adiabatic / isothermal expansion /
contraction. Maximum attainable efficiency for given τ₁, τ₂.

Reversibility
-------------

Entropy constant / always in equilibrium. Relaxation of constraints: if you
enforce the original constraints, and the system returns to its initial
state, it is reversible.

t{operation}, t{equilibrium}. t{o} » t{e}. Other possibility: t{e} ≫
t{o}. Also reversible. Becomes bad when these two are of the same order of
magnitude.

Clausius statement for 2nd law of thermodynamics: effectively, Carnot
engine is maximally efficient, given τ₁, τ₂. (q₂/q₁ ≤ τ₂/τ₁)

Joule-Thomson process: H = U + PV ⇒ H₁ = H₂ if dQ = 0.
μ ≡ V/C{p} (τlpha - 1)
Physics 112: Statistical Mechanics
==================================
Chemical Potential. Feb 22, 2012
--------------------------------

# Midterm
  * One page of notes. Clarification: One side of one sheet. No explicit
	ruling against oversized paper. Reasoning: it is always good to
	reconstruct what you have learned.
	+ Put things in your own terms and understand what you don't understand
	  and why you don't understand.
	  $\cdot$ There are some formulae that are useless to understand. (n_{Q}, n,
		etc.) This is not a memorizing test. I would like you to understand
		the concepts.
  * Will take about a week for grading.
  * No need for blue book. May want scratch paper if you like, but no blue
	book necessary.
# Exact differentials
  * Evolving system.
	+ Energy can be defined. Not necessarily useful.
	+ Entropy can also be defined.
	  $\cdot$ $\sigma = \log g_{t}$ only holds in equilibrium for an isolated system.
	  $\cdot$ In this case, it is well-defined by $\sigma \equiv -\sum p(t) \log p(t)$.
  * Heat transfer is not an exact differential.
# Chemical potential
  * Why is it called a potential?
  * Action mass law

Most common state is such that the sum of chemical potentials is equal to
zero. $\mu_{i} = \tau \log (n/n_{Q_i})$.
Physics 112: Statistical Mechanics
==================================
Chemical Potential. Feb 27, 2012
--------------------------------

Conference result (dark matter): unfortunately a negative result. A number
of groups (two in particular) claimed that they saw signals that could be
the result of WIMPs which are responsible for dark matter. MACHOs were
bad.

What we have done so far is referred to the microcanonical method (the name
does not matter). Basically, we have been counting states. With the
postulate of the H theorem, this allowed us to define entropy as $-\sum_i
p_i \log p_i$. ( Various reminders of definitions of temperature, pressure,
chemical potential. )

The system $S$ is in one state of energy $\epsilon$. How does the number of
the states in the reservoir evolve as $\epsilon$ increases? Since the two
systems are isolated, the total energy of the system is constant. As one
increases, the other decreases. Energy is directly proportional to the
number of states and inversely proportional to the probability of being in
a state.

Now we are equipped to derive the Boltzmann distribution.

We know that the number of states is $g_{R}(U_0 - \epsilon)$, where $g_R
\equiv (U_0 - \epsilon)^{3N/2}$.

$$
= A(U_0 - \epsilon)^{3N/2}
\\ = AU_0^{3N/2}(1-\frac{\epsilon}{3N\tau_R/2})^{3N/2}
\\ \Rightarrow AU_0^{3N/2}e^{-\epsilon/\tau_R}
$$

Configuration that we are looking at: state of the system
$S$.

$$Pr[S \in \epsilon ] \propto g_R(U_0 - \epsilon)$$

\begin{align}
\frac{Pr[S \in \epsilon_1]}{Pr[S \in \epsilon_2]}
= \frac{g_R(U_0 - \epsilon_1)}{g_R(U_0 - \epsilon_2)}
\\ = \frac{\exp(-\sigma_R(U_0-\epsilon_1))}
{\exp(-\sigma_R(U_0-\epsilon_2))}
\\ = \frac{\exp(-\frac{\epsilon_1}{\tau})}
{\exp(-\frac{\epsilon_2}{\tau})}
\end{align}

$$
Pr[S \in \epsilon] = \frac{e^{-\epsilon/\tau}}{\sum_s e^{-\epsilon
s/\tau}}
\\ (z \equiv \sum_s e^{-\epsilon s/\tau})$$

$z$ is known as the partition function.

So let me take a two-level system, where state 1 has $\epsilon = 0$, and
state 2 has energy $\epsilon$.

So the probability of being in state 1 is $\frac{\exp(-0/\tau)}{1 +
\exp(-\epsilon/\tau)} = \frac{1}{1 + \exp(-\epsilon/\tau)}$.

Likewise, the probability of being in state 2 is $\frac{\exp(-\epsilon/\tau)}{1 +
\exp(-\epsilon/\tau)} = \frac{1}{\exp(\epsilon/\tau) + 1}$.

As I increase the temperature, I can excite the system, and at some
temperature, the two states are equiprobable with 50%. 

The second example we will take is the Maxwell distribution, where a
particle in a gas in contact with a reservoir (which can be the rest of the
gas). To be continued on Wednesday.
Physics 112: Statistical Mechanics
==================================
Boltzmann Distribution. Feb 29, 2012
------------------------------------
5.1 Constant number of particles
================================
Boltzmann factor
----------------
Recall: two-state system, we could write down the Boltzmann
distribution. Note that heat capacity will peak when there is a maximum
change in state ($C_V = \pderiv{Q}{T} = \pderiv{U}{T}$.)

Let's go back a bit and try to understand where this equation is coming
from. Why does the probability that S in a quantum state energy $\epsilon$
decrease exponentially with $\epsilon$? As you increase $\epsilon$, since
the total energy $U_R$ is fixed, the energy and number of states in the
reservoir decrease (conservation of energy).

* Examples

Free particle at temperature $\tau$. Assumption: no additional degrees of
freedom (no spin, not a multi-atom molecule).

$\text{Pr}[dV , p+dp, d\Omega] = \frac{\sum \exp(-p^2/(2M\tau))}{Z}$

That's where we're using our recipe (result that we derived before) that
the density of states in phase space is merely $\frac{1}{\hbar^3}$. So the
number of states in a differential volume element is $\frac{dV d^3p}
{\hbar^3}$. Define $d^3p \equiv p^2 dp d\cos\theta d\phi$ (further defining
$d\Omega \equiv d\cos\theta d\phi$, where $\Omega$ is the solid angle
moment), i.e. convert to spherical coordinates. The above probability thus
reduces to $\frac{1}{Z} \exp(-p^2 /(2M\tau)) \frac{dV p^2 dp d\Omega}
{\hbar^3}$.

Normalizing to N particles (i.e. choosing $Z$ such that this sum is 1)
yields $f(v)dv d\Omega = n\left(\frac{M}{2\pi\tau}\right)^{3/2}
exp\left(-\frac{Mv^2}{2\tau}\right)v^2 dv d\Omega$. Note that $\hbar^3$
disappeared entirely. Important distribution, Boltzmann (we often call it
the Maxwell distribution).

Why does the Maxwell distribution have a $v^2$ term? It's a result of the
Jacobian matrix, which effectively tells us that the density of quantum
states per unit velocity interval in the system $S$ goes to zero as $v^2$
when $v$ goes to zero. Only works when the reservoir is very big relative
to the system. Cannot possibly be from the normalization, since this is a
function of $v$.

Notice that the slope of $f(v)$ is zero at $v=0$, whereas the slope of
$f(\epsilon)$ is $\infty$ at $v=0$.

Why doesn't the system S stay in a state of energy $\epsilon$? Continuous
exchange between $S \leftrightarrow R$ of excitations of energy
$\tau$. Thoughts: Uncertainty principle technically governs everything, but
that's not particularly useful. Each excitation in the reservoir will have
a typical energy $\approx \tau$. Thermal fluctuations of the order of
\tau. Difficult to get. $\epsilon \gg \tau$, $\text{Pr}[\epsilon]
\propto \exp(-\epsilon/\tau)$

With an electron cloud (since those are fermions), you have some more
complicated physics going on, but you have a Fermi gas, and you will be
exchanging energy on the order of $\tau$. In a crystal or a solid, you will
exchange phonons with energy on the order of $\tau$. Regardless of what
system you have, you are exchanging quantum energy packets on the order of
$\tau$.

Partition  function
-------------------
$Z = \sum_s \exp(-\epsilon_s/\tau$. Let's see, then, that we can compute
that. We can ask ourselves, what is the mean energy of the system? $U =
\avg{\epsilon} = \sum_s \frac{\epsilon_s e^{-\epsilon_s/\tau}}{Z}$. But
look, think about what $\pderiv{\log Z}{\tau}$ will look like.

Aside: we still have time to do the entropy.

$\sigma = -\sum p_s \log p_s = -\frac{\sum
e^{-\epsilon_s/\tau}}{Z}\left[-\frac{\epsilon_s}{\tau} - \log z\right]$.

What you see is just $\sum \frac{1}{\tau}\frac{\epsilon_s e^{-\epsilon_s
/\tau}}{Z} + \log Z = \frac{U}{\tau} + \log Z = \pderiv{\tau\log Z|}{\tau}$

$F = U - \tau\sigma = -\tau\log Z$.

[ done for the day. Fairly powerful tool. ]

Ideal gas (again!)
------------------
 * Entropy = Sackur-Tetrode formula

5.2 Exchange of particles
=========================
Gibbs factor
------------

Grand Partition Function as a calculation tool [ Gibbs Sum (grand canonical methods) ]
-------------------------------------
A very powerful tool. More technical, but important.

5.3 Fluctuations
================
Physics 112: Statistical Mechanics
==================================
Partition Function. Mar 2, 2012
-------------------------------

# Midterm
  * Office hours
# Partition function as computational tool
# Ideal gas

We are looking at a totally different method of computing entropy. Instead
of the microcanonical method -- counting states (impose U; difficult), Then
we are putting the system in contact with a reservoir. We came to the
conclusion that $\prob{i} = \frac{1}{Z}e^{-\epsilon_i/\tau}$. So that's a
totally different method, which tends to be much easier.

From what you have seen, it is quite easy to get ahold of the thermodynamic
quantities you know of.

$$
\sigma = \pderiv{\tau\log Z}{\tau}
\\ F =  U - \tau\sigma = -\tau\log Z \implies \sigma = -\pderiv{F}{\tau}
\\ U = \avg{\epsilon} = \sum \epsilon_i p_i = \tau^2 \pderiv{\log Z}{\tau}
= -\tau^2\pderiv{\frac{F}{\tau}}{\tau}
$$

Examples
--------

Consider a two-level system with energies 0 and $\epsilon$. $Z = 1 +
e^{-\epsilon/\tau}$, trivially. Therefore $U = \tau^2\pderiv{\log z}{\tau}
= \tau^2\frac{\frac{1}{\tau^2}e^{-\epsilon/\tau}}{1 + e^{-\epsilon/\tau}} =
\frac{1}{e^{\epsilon/\tau} + 1}$.

Now, for an ideal gas: $Z = \sum_s e^{-\epsilon_s/\tau} = \int \frac{d^3q
d^3p}{\hbar^3}e^{-\epsilon}{\tau}$. Phase space integral. Things are very
simple.

This is equivalent to $\frac{V}{\hbar^3}\int dp_x e^{-p_x^2/2M\tau} dp_y
e^{-p_y^2/2M\tau} dp_z e^{-p_z^2/2M\tau} = \frac{V}{\hbar^3}\left(
\sqrt{2\pi M\tau}\right)^3 = V\left(\frac{2\pi M\tau}{\hbar^2}\right)^3/2 =
n_Q$.

$\avg{\epsilon} = \frac{3}{2} \frac{\tau^2}{\tau} = \frac{3}{2}\tau$

The power of $Z$ is that either you can do these sums very easily
(e.g. geometric series), or the terms grow so fast that you can just take
the first term, or you can use the integral approximation as we have done
here.

Harmonic Oscillator
-------------------

$E = \sum e^{-s\hbar\omega/\tau} = \left(\sum e^{-\hbar\omega/\tau}
\right)^s = \frac{1}{1 - e^{\hbar\omega/\tau}}$

These are known as the canonical methods, which are fairly powerful. I may
come back to this question of density of states. I have probably told you
enough on how to sum over discrete states. We may come back when we review
the material.

I have spoken long enough about this fairly technical thing. Let's ask
ourselves how to extend this to multiple systems (e.g. 2).

The partition function of 2 systems is merely the product if the systems
are distinguishable, and the product divided by $2!$ (approximately) if
they are indistinguishable. Consider indistinguishability of "quantum
states", where each state is a system.

Therefore if we have N indistinguishable systems, $Z(N) \approx \frac{1}
{N!} Z(1)^N$. This is a low occupation number approximation due to Gibbs.

$$Z_1 = e^{-mB/\tau} + e^{mB/\tau} = 2\cosh\frac{mB}{\tau} \\ Z = Z_1^N =
2^N\cosh^N\frac{mB}{\tau} \implies U = -NmB\tanh\frac{mb}{\tau}.$$

Thus $M = \frac{U}{BV} = nm\tanh\frac{mB}{\tau}$.

[ curie temperature: where M disappears ]

* Why is the division of the product by N! approximate?

As mentioned earlier, this is a low concentration approximation, i.e. the
probability of having two systems in the same state is negligible. The
error we accumulate is due to fewer terms appearing in the sum.

In other words, we have very weak correlation coefficients.
Physics 112: Statistical Mechanics
==================================
Ideal gas, Gibbs distribution: Mar 5, 2012
------------------------------------------
Ideal Gas
=========

We previously focused on the partition function, which is $\sum_s
e^{-\epsilon_s/\tau}$. This so-called "canonical" method is much simpler,
usually, than counting states with the constraint that energy is fixed. So
that's the advantage of that method, and so, from the partition function by
appropriate derivatives (usu. of the log), you can get all the quantities
that you like (energy, entropy, free energy, chemical potential, pressure,
and so forth).

If I have $N$ systems, $Z = (Z_1)^N$ (if the systems are distinguishable),
and $Z \approx \frac{(Z_1)^N}{N!}$ if the systems are indistinguishable. We
discussed last time why this is an approximation: sparseness of states.

For the ideal gas, we found that $Z = Vn_Q$, where $n_Q\equiv \parens{
\frac{M\tau}{2\pi\hbar^2}}^{3/2}$. This is $\approx \frac{1}
{\lambda^3}$. So this is really a quantum density satisfied by putting
particles a wavelength apart, and I cannot do much better than that.

If I apply the Gibbs recipe there, what I get is that $Z_N =
\frac{1}{N!}\parens{Vn_Q\right}^N$. So $\log Z_N = N\log(Vn_Q) - \log N!$. We
use the Stirling approximation to say $\log N! \approx N\log N - N$. Thus
$\log Z_N = N\log(\frac{n_Q}{\frac{N}{V}}) + N = N\log \frac{n_Q}{n} + N$.

When we introduce free energy, we have $F = -\tau\log Z$; $p =
-\pderiv{F}{V}$; $\sigma -\pderiv{F}{\tau}$.

Barometric equation
-------------------
Assume the atmosphere has constant temperature. How does the density
decrease with altitude z? The way the book does it is $\mu = \const$, since
we are in thermal equilibrium. But $\mu$ has two pieces: the internal
chemical potential ($\tau\log\parens{\frac{n}{n_Q}}$) and external chemical
potential, which is just the potential in the gravitational field, namely
$mqz$. This has to be constant, which implies that $n = n_0\exp\parens{
-\frac{mqz}{\tau}}$.

The problem with this derivation is that it is at a very high level. We
need to invoke the chemical potential. Very similar problem to density of a
centrifuge, or density of ions in the membrane of a cell.

This is one way of doing things. There are actually two other ways of doing
things.

Single-particle occupancy of levels at different altitude
---------------------------------------------------------
Instead of considering the atmosphere to be in equilibrium, I would
ask myself (the more intuitive way of doing it), what is the probability
that a given molecule is at the altitude $z$? I (Sadoulet) would say that
$\epsilon = \epsilon_k + mgz$ (energy is kinetic energy + potential
energy). The probability of being at the altitude $z$ would be proportional
to $\exp\parens{-\frac{\epsilon_k + mgz}{\tau}}$. The density, therefore,
has to be proportional to $\exp\parens{-\frac{mgz}{\tau}}$.

The problem with these two derivations is that they do not generalize very
well to the point where you are not in equilibrium.

Hydrodynamic equilibrium
------------------------
The third way of doing it (which you have likely done in Physics 7) is to
consider a slab of thickness $dz$ and consider the hydrodynamic
equilibrium. The force pushing up on this slab is $pA$, whereas the force
pushing down on the slab is $(p + dp)A$. Our slab has a certain mass and
particle density, and so the downward force (due to gravity) is $nmAz
g$. Putting that all together, we have $pA - (p + dp)A = nmgzA$. This leads
directly to $\frac{1}{n}\deriv{p}{z} = -mg$. This is totally general. If we
have $pV = N\tau$, $p = \frac{N}{V}\tau = n\tau$. Since $\frac{\tau}{\p}
\deriv{p}{z} = -mg \iff \frac{1}{n} \deriv{n}{z} = -\frac{mg}{\tau} \implies
p \sim \exp\parens{-\frac{ngz}{\tau}}$. This generalizes to the case when
the temperature is not constant.

(various clicker questions)

Grand partition function: $\sum_{S,N} \exp\parens{-\frac{\epsilon(N) - \mu
N}{\tau}}$

Gibbs Distribution
==================
Exchange not only energy, but also particles.
Physics 112: Statistical Mechanics
==================================
Gibbs Distribution: Mar 7, 2012
-------------------------------
The mathematics of the Gibbs distribution is not difficult so much as
complicated. What is difficult is determining what phenomena this
explains.

$$\prob{S \in \epsilon_s(N_s), N_s} \propto g \propto \exp
\parens{-\frac{\epsilon_s(N_s)}{\tau}} \exp\parens{\frac{\mu}{\tau}}
\\ = \frac{1}{z} \exp\parens{-\frac{\epsilon_s - \mu}{\tau}}
\\ z \equiv \sum \exp\parens{-\frac{\epsilon_s - \mu}{\tau}}
$$

We call this the Gibbs distribution (z is, as we recall, the grand
partition function).

Often, chemists prefer to consider chemical potential $\lambda_i \equiv
\exp \parens{\frac{\mu_i}{\tau}}$. 

This is weak interaction. What it means is that as we keep adding particles
at the quantum level, we don't change the wave function. They don't care
how many particles are in the system.

Often, we will simply use $\prob{\epsilon_s} = \frac{1}{z}\exp \parens
{-\frac{(\epsilon_s - \mu)N}{\tau}}$.

A common problem with this distribution, by the way, is that we are
extremely general, and sometimes it is difficult to know what this
represents in practice, so we should take examples and try to think about
the examples to consider what these mean in practice.

Maybe the simplest example I can take is a Fermi-Dirac distribution. Let us
consider an energy level $\epsilon_s$, and I have a fermion, which has a
half-integer spin, e.g. an electron (spin $\frac{1}{2}$). If we listen to
Pauli, at most one fermion can occupy each state.

Therefore $N_s \in \{0,1\}$. $\prob{N_s=0} = \frac{1}{z}$; $\prob {N_s=1} =
\frac{1}{z} e^{-(\epsilon_s-\mu)/\tau}$. So $z = 1 + e^{-(\epsilon_s-\mu)/
\tau}$. Plugging this back in, we have $\prob{N_s=0} = \frac{1}{1 + e^{
-(\epsilon_s-\mu)/ \tau}}$; $\prob {N_s=1} = \frac{ e^{-(\epsilon_s-\mu) /
\tau}}{1 + e^{-( \epsilon_s-\mu)/ \tau}} = \frac{1} {e^{( \epsilon_s -
\mu)/\tau} + 1}$. Examples: gas absorption: heme in myoglobin, hemoglobin,
walls. Energy bands of materials (bandgaps).

Determining $\mu$, when considering hemoglobin and stuff. All we need is
the density of $O_2$ in the blood. So how can we compute this? Remember
what we said about mass action law. If we are a dilute system of particles,
they will have the same properties as the gas: they will barely interact
with each other, so states will be independent, and we can then apply the
ideal gas approach.

We can also apply this to our dissolved gas, and $\mu_{gas} = \tau\log
\frac{n}{n_Q}$. This is an ideal gas in the sense of weakly-interacting
n-body system.

Chemists and biologists like to put the pressure, since the partial
pressure is something you can measure easily. Langmuir adsorption isotherm:
$f = \frac{p}{\tau n_Q\exp\parens{\frac{\epsilon}{\tau}} + p}$.

Aside: Pauli was an enormous guy, German/Swiss physicist. Very bright but
very unforgiving. Lack of understanding: not a question.

Adsorption: fraction occupied $= f$. Same form as Fermi-Dirac. Adsorption
dependence on $\mu$ can clearly be observed to be positive: as $\mu$
increases, the fraction of occupied sites increases. However, as $\tau$
increases, the fraction of occupied sites decreases. (binding energy:
$-\epsilon$)

Ionized impurities in a semiconductor: K&K p370. Doping. Donor: tends to
have one more electron; acceptor: tends to have one fewer electron. $\mu$
(Fermi level) determined by electron concentration in semiconductor.
Physics 112: Statistical Mechanics
==================================
Gibbs Grand Partition Function: Mar 9, 2012
-------------------------------------------
Gibbs grand partition function, fluctuations, what is minimized when a
system is in thermal equilibrium with a bath?

Next midterm is Monday, March 19.

I would like to move the third midterm from April 20 to April 13 for two
reasons: one, it's a week before we finish; two, allows me to go to a small
workshop in Davis. Interesting workshop, announced at last minute, purpose
is to try to understand what the LHC tells us about dark matter.

There was an announcement by Fermilab that they may have seen the
Higgs. CERN might have seen the Higgs. Not convinced by announcements so
far: more publicity than anything else.

Let's go rapidly through the grand partition function. Remember, we were
speaking of a system, which was exchanging with a reservoir both energy and
particles. What we had shown was that $\prob{\epsilon_s(n)} = \frac{1}{z}
\exp (-\frac{\epsilon-\mu N}{\tau})$, $z = \sum_{s,N} \exp(-\frac{\epsilon
- \mu N}{\tau})$. In most cases, we'll have $\epsilon_s(N) = \epsilon_s
N$. So that's the Gibbs formalism. Almost exactly in the same way as in the
Boltzmann formalism, we can deduce a number of things about the derivatives
of the log of this partition.

For instance: taking into account one species, $\avg{N} = \sum_{s,N}
\frac{1}{Z} N\exp (-\frac{\epsilon_s(N)-N}{\tau})$. See, if I were to take
$\pderiv{\log Z}{\mu}$, I would have $\sum_{s,N} \frac{N}{\tau}\exp (-\frac
{\epsilon_s(N)-N}{\tau})$. And so $\mu = \tau\pderiv{\log Z}{\mu}$.

So let's take two examples: Fermi-Dirac distribution.

Fermions versus bosons: fermions have half-integer spins, follow
Fermi-Dirac distributions; bosons have integer spins, follow Bose-Einstein
distribution.

So in the Fermi-dirac, we have $\avg{N} = \tau \pderiv{\log Z}{\mu} =
\frac{\exp(-(\epsilon-\mu)/\tau)}{1 + \exp(-(\epsilon-\mu)/\tau)} =
\frac{1}{\exp((\epsilon-\mu)/\tau) + 1}$.

Bose-Einstein: $z = \sum_N e^{-\frac{(\epsilon-\mu)N}{\tau}}$. You
recognize this is a geometric series and is thus equal to
$\frac{1}{1-\exp(-(\epsilon-\mu)/ \tau)}$. $\avg{N} = \tau\pderiv{\log Z}
{\mu} = \frac{\exp((\epsilon-\mu)/\tau)}{1 - \exp((\epsilon-\mu)/\tau)} =
\frac{1}{\exp((\epsilon-\mu)/\tau) - 1}$

Note that as $\epsilon-\mu \to 0$, this quantity diverges: Bose-Einstein
condensation. On the other hand, for a Fermi-Dirac distribution, this
converges to 1.

Just pay attention to $\sigma = \sum_{s,N}p_{s,N}\log p_{s,N}$. I will put
into this expansion my Gibbs factor $\frac{1}{Z}\exp(-\frac{-\epsilon_s(N)
- \mu N}{\tau})$.

$$
\log z + \sum_{s,N} p_{s,N} \frac{\epsilon_s(N)}{\tau} - \sum_{s,N} p_{s,N}
\frac{\mu N}{\tau}
\\ = \log Z + \frac{\avg{\epsilon_s}}{\tau} - \frac{\avg{N}\mu}{\tau}
\\ = \pderiv{\tau\log Z}{\tau}
$$

You have to be careful. The formulae are different with the grand partition
as opposed to without the partition function. $\Omega \equiv F - \sum_{\mu_i}
\avg{N_i} = -\tau\log Z$.

Note that $\sigma = \pderiv{\tau\log Z}{\tau}$ while $\Omega = -\tau\log Z$
as a result of the thermodynamics identity.

Fluctuations
------------
Actually, we started to speak about what I am going to say. There are
fluctuations when we are exchanging particles or energy with the
reservoir. The number, the energy is not fixed, and if I am exchanging
particles, they fluctuate. I told you about the mean number of particles
there; we spoke before abotu the mean energy. But now we can try to compute
the variance (or root-mean-square/standard deviation) of this quantity.

For instance, you remember that for a Boltzmann distribution (not
exchanging particles, so I don't need the grand partition function),
$\avg{E} = \tau^2\pderiv{\log Z}{\tau}$. The variance, you should remmeber,
is simply $\sigma_E^2 = \avg{E^2} - \avg{E}^2 = \sum \epsilon_s^2
e^{-\epsilon_s/\tau} - \parens{\sum \epsilon_s e^{-\epsilon_s/\tau}}^2$. If
you differentiated this expression with respect to $\tau$, you got this
expression, which was this elegant, if not beautiful formula $\avg{N} =
\tau\pderiv{\log Z}{\mu} = \tau^2\pderiv{\log \avg{E}}{\tau} = \tau^2
\pderiv{\tau^2 \pderiv{\log Z} {\tau}}{\tau}$.

So $\sigma_N^2 = \avg{N^2} - \avg{N}^2 = \tau \pderiv{}{\mu}
\parens{\tau\pderiv{\log Z}{\mu}}$.

Let me quickly do my calculations for my Fermi-Dirac and Bose-Einstein
distributions, considering $\sigma_N$. So I have to take $\sigma_N^2 =
\tau\pderiv{\avg{N}}{\mu}$. So for Fermi-Dirac, we have $\frac {e^
{(\epsilon -\mu)/ \tau}}{e^{(\epsilon-\mu)/\tau} + 1} = \avg{N}(1-\avg{N})$.

Note that the variance is actually less than $N$, so less than the Poisson
distribution.

If I were to do the same thing for the Bose-Einstein distribution, I would
get $\avg{N}\parens{1 + \avg{N}}$. So the fluctuations at N = 0 are
absolutely enormous.

So we say that the Bosons like to travel in flux.

Physicist joke: astronomers are fermions, particle physicists are bosons.
Physics 112: Statistical Mechanics
==================================
What is Minimized; Black Body: Mar 12, 2012
------------------------------------------
Housekeeping
============
Remember that we have a midterm next Monday. Some material is in the
book. The next midterm would be Friday (April 13/14, depending on which is
Friday).

Today, office hours moved to 1:30-2:15. Review session on Saturday.

What is minimized?
==================
Would like to start by asking you a question: in the conditions we have
been speaking about (system s in contact with reservoir), exchanging only
energy, does it go to a state of minimum energy? No; remember the constant
exchange of energy (constant kicking, so to speak).

Contrary to a system which is able to lose energy to vacuum, Does not
evolve to state of minimum energy. Contrary to an isolated system, does not
evolve to a configuration of maximum entropy (entropy of combination of
reservoir and system is maximized).

Evolves to a configuration of minimum Free Energy ("balance between
tendency to lose energy and to maximize entropy")

Landau Free Energy & Enthalpy
-----------------------------
More rigorously: We cannot defint he temperature of the system out of
equilibrium. So we introduce $F_L(U_S) \equiv U_S \tau_R\sigma_S(U_S)$
(Landau Free Energy; constant volume) and $G_L(U_S, V_S) \equiv U_S
\tau_R\sigma_S(U_S,V_S) + p_RV_S$ (Landau Free Enthalpy; constant
pressure). The difference between ordinary free energy and the Landau free
energy is that the ordinary free energy is a function of the system $S$
that is only defined at equilibrium, whereas Landau Free Energy is defined
everywhere.

What we want to show that this $F_L$ is the value that is maximized. We can
simply count states.

$\sigma_{tot}(U_S) = \sigma_R(U-U_S) + \sigma_S(U_S) = \sigma_R(U) -
\pderiv {\sigma_R}{U}U_S + \sigma_S(U_S) = \sigma_R(U) - \frac
{1}{\tau_R}U_S + \sigma_S = \sigma_R(U) - \frac{1}{\tau_R}F_L(U_S)$

The most probable configuration maximizes $\sigma_{tot}$, which minimizes
$F_L$. Note that this implies that $\pderiv{F_L(U_S)}{U_S} = 0 \iff \pderiv
{\sigma_S(U_S)}{U_S} = \frac{1}{\tau_R}$ (by the definition of Landau free
energy).

When minimized, temperature of system is equal to temperature of reservoir.

Landau Grand potential
----------------------
If we exchange particles, what is minimized is $\Omega_L(U_S,N_S) \equiv
U_S - \tau_R\sigma_S(U_S,N_S) - \mu_R N_S$ (the Landau Grand Potential).

This will be useful when we do phase transitions. They get interesting in
statistical mechanics, and people are using this Landau Free Energy.

Aside
=====
This completes the material for the midterm. Since I do not like to
emphasize memorization, this time is that you get two pages (one sheet
double-sided) of notes of formulae. The main thing is not the formulae, but
rather how to apply them. So many formulae now that if you apply them now,

Black Body radiation
====================
Let us begin with the Planck distribution.

Usual way to consider a gas of photons in thermal equilibrium. (take
$\omega \equiv 2\pi v$) Let's think of it in a single mode of cavity, and
consider the number of photons in that mode. Harmonic oscillation:
$\omega$. If I have s photons in this mode, the energy would be $\emf
\equiv s\hbar\omega$; $s \in \mathbb{Z_+}$. So $Z = \sum_s e^{-s\hbar\omega
/ \tau}$, roughly. So $\avg{S} = \frac{\tau^2}{\hbar\omega} \pderiv{\log Z}
{\tau} = \frac{e^{-\hbar\omega/\tau}}{1 - \e^{-\hbar\omega/\tau}} -
\frac{1}{\e^{\hbar\omega/\tau} - 1}$. So $\avg{\emf_\omega} = \frac{\hbar
\omega}{e^{\hbar\omega/\tau} - 1}$

Two quantifications: first quantification (wave-like): discrete states in
massive particles; obvious cavity modes for photons. The second
quantification was of discrete particles: it was reversed -- it was obvious
that massive particles were quantized as discrete particles, but not so
much that photons were quantized in numbers -- Planck.

Questoin: why is the mean energy per mode decreasing with energy? For
$\hbar\omega > \tau$, it is more nad more difficult for the bath to create
a photon: I need $\hbar\omega$ to create a photon, and if it's too large, I
don't have enough energy available.

Photon properties. Maxwell equations in vacuum.

Mean energy density: Is $\hbar\omega$ the mean energy density as a function
of frequency? No; we have to fold in the frequency density of the modes
$D(\omega)d\omega$ which can be computed with our $\frac{1}{h^3}$ rule.

The density of states is $2\frac{d^3xd^3p}{h^3}$. (2 is the polarisation
factor) Note that $pc = \hbar\omega$, and $d^3p = p^2 dp d\Omega$. So our
density is $\frac{2d^3x(\hbar\omega)^2\hbard\omegad\Omega}{c^3\hbar^3}$. We
can use the fact that $\hbar^3 = \frac{1}{8\pi/3}$. If we are not
interested in the direction of the photons, we integrate on solid angle and
we get $u_\omega d\omega = u_vdv = \frac{\8\pi hv^3dv}{c^3(\exp(hv/\tau) -
1)$. I would like you to be able to derive this from first principles,
rather than rote memorization.
Physics 112: Statistical Mechanics
==================================
Black Body: Mar 14, 2012
========================
Office hours: today from 3:30-4:30; extra at Friday from 3-4.

Review Saturday @ 10:30.

Black Body
=========
Radiation energy density between $\omega$ and $\omega+d\omega$? 

Would like to rederive black-body law in a slightly different way. Recall:
speaking of photons in equilibrium with a metallic cavity. In that case,
the average number of photons at frequency $\omega$ is $\frac{1}{e^{\hbar
\omega/\tau} - 1}$. The minus is coming from the fact that we have a boson,
the spin of which is 1. Some of you are more comfortable with $\nu = \frac
{\omega}{2\pi}$, in which case the energy is $\frac{1}{e^{\hbar
\nu/\tau} - 1$}.

We can write $u_\nu(\nu,\theta,\phi) 2\frac{d^3xd\nu d\Omega}{h^3} =
\avg{s}h\nu 2\frac{d^3xd^p}{h^3}$ (we need to pull out this factor of two
to account for the polarization). We can then use that $p = \frac{\epsilon}
{c} = \frac{h\nu}{c}$. If I'm not interested in the direction, I have to
integrate over the angles, which gives me a factor of $4\pi$, and so our
net result is $u_\nu(\nu)d^3xd\nu = \frac{8\pi h\nu^3d\nu d^3x}{c^3(e^{h
\nu/\tau}-1)}$

Cosmic microwave radiation
--------------------------

Example of most perfect black body that we know: photons in equilibrium in
early universe. In the early universe, the tempmerature was over 3000 K. We
had mostly $p + e^-$ at that time. The mean free path was very low; protons
interacting with electrons. So what you had was a plasma; effectively
opaque to photons -- very high scattering. At about 3000 degrees, universe
then becomes transparent: hydrogen forms, and photons don't scatter.

So all around us, we see this radiation (discovered in the 60s), and it is
no longer at this temperature. The radiation has been shifted and is now at
about 3K -- in microwave band; roughly mm wavelength.

Difficult to make black body radiator to calibrate instrument: primary
limiting factor.

Fluctuations of temperature are $10^{-5}$ of mean temperature. You can
measure these as frequencies. You get this marvelous spectrum with wiggles,
and we see the plasma vibrating, in some sense. This gives us a lot of
information: tells us that the universe is especially flat; tells us the
amount of protons and neutrons in the universe; tells us the amount of dark
matter.

Allows us, for instance, to look at a lot of cosmology parameters.

We can also measure polarization; gravitational potential waves shaking
this plasma.

These fluctuations are (difficult to prove) responsible to the formation of
structure: they are responsible for the formation of galaxies.

European satellite this year named Planck, which will achieve more accurate
results.

Could lecture for over ten hours on this subject, but that is not the
subject of this class.

Planck
======

Before: physicists only considered continuum. We did not know about the
second quantization, that photons come with energy $h\nu$. Physicists of
19th century just wrote the partition function, summing over states. If you
do this, you get $\tau/\epsilon_0$, independent of frequency. The mystery
was you had to sum over modes (frequencies), and you'd get infinity. This
is a problem.

Planck introduced the quantization of states. Planck did not clearly
understand what he was saying. The photons comes in quanta of $\hbar
\omega$. Thus there is a cut-off at $\epsilon=\tau$, and so you do not have
what was called the ultraviolet catastrophe. This was 1903.

In 1905, Einstein published two articles, one which was about this
commenting on how quantization explains the photoelectric effect -- this is
why he got his Nobel prize. The same year he also published his paper on
special relativity, and so he did not have to work an 8-5 job.

Have we solved everything?
--------------------------
No: zero point energy. We have again an infinite sum. This is related to
the problem of the vacuum energy, dark energy, and the cosmological
constant.

Namely, $\epsilon_\omega = \frac{\hbar\omega}{2} + s(\hbar \omega )$. This
is related to what we consider vacuum energy, dark energy (maybe), and the
cosmological constant.

Note: important to sum instead of integrate.

Let me try to ask you why we did not use the Gibbs formalism? Photons
appear and disappear in interaction with cavity. However, this is a
different formula.

The reason why we do not use this is that the chemical potential of the
photon must be zero. Why? Special case of mass action law; entropy of the
reservoir does not change when we change the number of photons (keeping the
energy constant); and the photons is its own antiparticle.

Namely: $\mu_\gamma + \mu_e - \mu_e = 0 \implies \mu_y = 0$; $\pderiv
{\sigma_R}{N_{\gamma BB}}\bigg|_U = -\frac{\mu_\gamma}{\tau} = 0$. And
finally $\gamma + \gamma \leftrightarrow e \bar{e}$. We will see that the
chemical potential of the antiparticle is the same as that of a 

It is perfectly fine to use the Gibbs formalism; it is just that
$\mu_\gamma$ is zero.

Theme of this course: there are often three different ways of deriving the
same result: microcanonical (counting states), canonical (Boltzmann), and
grand canonical (Gibbs formalism).

Counting number of states: Kittel and Kroemer go through a painful counting
of number of states using quantum numbers. Of course, same result.

Flux through an aperture. Do not forget cosine factor: volume of oblique
cylinder is $cdtdA\cos\theta$.
Physics 112: Statistical Mechanics
==================================
Black Body: Mar 16, 2012
========================

As usual, housekeeping. Then comments on grand partition function. And then
we will come back to the black body approach and finish the
Stefan-Boltzmann law, speak about Kircchoff.

Wednesday moving again office hours: going to SF to participate in a
roundtable discussion between artists and scientists on the concept of
space: "how do we know that things we don't see exist?" (i.e. dark matter,
dark energy). The thing is very strange (suggested by an artist) is that
the main question is about creativity. Important for scientist, yes, but
this is not useful for invisible space; we do not create things; we are
forced to believe these things.

There has been some confusion regarding the grand partition
functions. $\frak{Z} = \sum_s e^{-\frac{\epsilon_s(N_s)-\mu
N_s}{\tau}}$. We have been using this primarily for a system of one state
$\epsilon_i$. In this case, the partition function $\frak{Z}_i =
\sum_{N_i} e^{(\epsilon_i-n_i)N_i/\tau}$. Then, we get similarly that the
average number of particles of this state is $\tau \pderiv{\log \frak
{Z}_i}{\mu}$.

Thus if we have a system with all possible states, $N = \sum \avg{N_i} =
\sum_i \tau \pderiv{\log\frak{Z}_i}{\mu_i}$. Therefore $\avg{U} =
\sum_i \tau\epsilon_i \pderiv{\log\frak{Z}_i}{\mu}$.

However, we could also approach this by considering our system to be an
ensemble of states from the start. In order to specify this, I must
specify the number of particles that have specific energies.

Rather, $\frak{Z} = \sum e^{-\frac{\sum \epsilon_i N_i - \mu\sum
N_i}{\tau}} = \prod_i(\frak{Z}_i)$.

We can then explore a bit: $\avg{N} = \tau\pderiv{\log \frak{Z}}{\mu} =
\sum_i \tau\pderiv{}{\mu}\log z_i$ (after some simple arithmetic
manipulations)

By the way, if you do it either way, you have no problem with the
distinguishability of the various states. You take that into account
automatically.

Note that this is different from the case where the system is an ensemble
of particles.

Recall: flux through an aperture requires us to integrate over an oblique
cylinder, which has area $cdtdA\cos\theta$.

$u_\omega(\theta,\phi d\omega d\Omega = \frac{\hbar\omega^3d\omega}{\pi^2
c^2(\exp(\hbar\omega/\tau) - 1)}$. This is the energy density of photons
moving in the direction $\theta, \phi$. If I'm interested in the flux
density, i.e. the brightness, there I am just looking at what happens
taking a unitary $dA$ perpendicular to the direction. We consider
$I_\nu(\theta,\phi)d\omega d\Omega dt dA = \frac{\hbar\omega^3
d\omega}{\pi^2 c^2(\exp(\hbar\omega/\tau) - 1)} cdt dA$. $I_\nu$ is just
$\frac{2h\nu^3d\nu dt dA}{c^2(\exp() - 1)}$.

With a fixed aperture, $J_\nu dA dt d\nu = \int \frac{2h\nu^3
d\nu}{c^3(\exp() - 1)} cdtdA\cos\theta d\Omega$. We have to be careful
here: we do not integrate beyond $\frac{\pi}{2}$, since those photons are
going the wrong way -- the only photons that go through the aperture are
moving toward the aperture.

So what we have finally is $\frac{4\pi h \nu^3 d\nu dtdA}{c^2(\exp(h\nu /
\tau) - 1)} = \frac{c}{4} u_\nu d\nu dA dt$. Note here that $u_\nu$ is the
energy density integrated over the solid angle.

Therefore if I am interested in the total energy in my volume, I will
integrate $\int u_\nu(\theta,\phi)d\nu d\Omega dV = \int \frac{8\pi h\nu^3
d\nu}{c^3(\exp(h\nu/\tau)-1)} = \frac{8\pi V}{h^3 c^3} \int_0^\infty
\frac{\tau^4 x^3 dx}{\exp(x)-1}$. The total energy, therefore, goes as $a_B
T^4\; a_B = \frac{\pi^2 k_B^4}{15\hbar^3 c^3}$.

Similarly, if you were to look at thte total flux through a fixed aperture,
we will do the same calculation, but now what we will get $J =
\frac{c}{4}a_B t^4 = \sigma_B t^4$.

You can also get the entropy and the number of particles by just
integration. For entropy, you can either integrate $d\sigma/d\tau$ or just
remember the density of states, which goes as $T^3$, as does the number.

Why do we have a $T^4$ for energy density but a $T^3$ for entropy or number
of photons? By the way, entropy is proportional to number of photons, which
makes sense. Mathematically, this appears as a result of change of
variables. So what is the effect that dominates? It is the increase of the
density of states with energy. Density of states goes as $\omega^2
d\omega$, which comes directly from the counting of states. Since $\omega$
is of the order of $\frac{\tau}{\hbar}$, we get here that the number goes
as $T^3$. Of course, when I'm looking at energy, I have one extra factor of
temperature ($\tau \equiv k_B T$), and that's where $T^4$ comes in.
Physics 112: Statistical Mechanics
==================================
Black Body: Mar 21, 2012
========================
Overview
========
Black body: Detailed balance, Kirchhoff laws

Midterm on the fifteenth. No homework due on thirteenth.

As mentioned last week, cannot be at office hours this afternoon, going to
SF for panel discussion between artists and scientists about space and the
unknown. Instead, I would like to propose office hours on Friday 3-4.

Examining of histogram. Happy about no very low grades; 7.5 points lower;
smaller spread.

There are still people in the class writing something like $\mu =
\pderiv{\sigma}{N} = \pderiv{U}{N}$ without putting any indication of what
the independent variables are. The second type of problem which seems
serious are confusions. One of these is that between isolated systems and
systems in contact with a bath. Of course, at equilibrium, the probability
of a given state is $\frac{1}{g_i}$ (H theorem), and in the second case,
they are not equiprobable and are given by the Boltzmann distribution (or
Gibbs).

Also, people assuming everything is an ideal gas. Don't do that. Putting
random formulae shows that you don't understand the problem, so you'll lose
points.

Statistical mechanics is much bigger than just **classical** ideal
gases. And it's much more than Thermodynamics identity. Those are
distortions of coming from Physics 7; you tend to write the Thermodynamics
identity over and over; we have much more powerful ways to do things: we
can compute entropy from first principles. And then people use $dU = \tau
d\sigma - pdV + \mu dN$, but people without a lash will put $U =
\tau\sigma$. Reverse-engineering, it does not work.

Also, we'll use the best two midterms out of three.

For these things, any questions? Alex has the midterms, and I will have
them on Friday.

Black Body
==========

We are in black body radiation. What I would like to focus on today is heat
imbalance. We have actually a very specific black body radiator, which is a
cavity with metallic walls. We were thinking about the modes in this cavity
and the photons in thermal equilibrium. Now, what we will do is put another
system in communication with this cavity and ask ourselves: what is the
radiation of this cavity? (these two systems are at the same temperature
and communicate through an internal aperture)

Suppose that first that the second system is a black body. By this, we mean
something that absorbs all radiation. So a cavity with a very small hole is
a very good approximation for a black body: if I send a photon into this
hole, it will not come back.

Can imagine more black bodies -- what we use in our field: rubber with a
lot of carbon in it (does not reflect, only absorbs).

By construction there, if we have these two systems communicating, the
energy emitted by one is the energy absorbed by the other.

First question, which is very simple: how does the energy emitted by system
1 compares to energy absorbed by system 1? Since they are at the same
temperature, the energy emitted by either system is the same (consider
formula derived last lecture).

**Principle of detailed balance**. Consequence: the spectrum of radiation
emitted by a black body is the "black body" spectrum calculated before.

This is a very simple argument, but very powerful. Proof: $\frac{c}{4}A
u_{BB} = \frac{c}{4}Au_{cavity} \implies u_{BB} = u_{cavity}$. Emits in an
isotopic way exactly as the cavity. We could have inserted a frequency
filter or a direction selector, and these still remain constant.

Let's modify the situation. Instead of a black body, let's consider a grey
body, and let's define an absorption coefficient $a \equiv \frac {\text
{power absorbed}}{\text{power received}}$. In principle, this could depend
on angle and frequency. So the question now that we ask ourselves is how does
the energy of a grey body compare to energy emitted by a black body?

For this, we must consider both the reflected BB energy and GB emission by
walls.

Notice that the energy received by the black body is $(1 - a)(BB) + a(BB) =
BB$. Emission coefficient = $e = \frac{\text{power emitted}}{\text{power
black body}}$. $a = e$ -- usually known as Kirchhoff law. The black body
receives back exactly what it emits. Therefore its temperature stays
constant.

Very useful in many applications. At the basis of the Nyquist noise or
Johnson noise. We will come back to this. You can show that the amount of
power emitted $U d\nu = 4kTRd\nu$. This is explained not very well, I'm
afraid, in Kittel and Kroemer, but this is the cause for many sources of
noise in our electronic circuits. More specifically, a theorem known as the
dissipation/noise theorem: any system capable of absorbing radiation is
making noise: if it absorbs radiation and has constant temperature, it will
have to emit *something* to stay at constant temperature. This is deeply
ingrained in quantum mechanics: anything that absorbs emits.

In order to detect anything, we absorb energy. And because we absorb
energy, we must emit energy.

There are many applications. Let me just give you an orientation. In many
cases, in all the sensing applications, we can say that we are at least
roughly a black body radiator, which has a certain surface area $A_e$, and
we are looking at it with some sort of telescope with a certain reception
area $A_r$. There is a simple relationship if the distance is $d$. The
source is seen from the receptor to fill a solid angle $\Omega_r$, which is
basically, for small angles, just $\theta^2$. Similarly, the solid angle as
seen by the emitter is $\Omega_e = \frac{A_r}{d^2}$; likewise, $\Omega_r =
\frac{A_e}{d^2}$, and so if you take the ratio of the two, you have
$\frac{\Omega_e}{\Omega_r} = \frac{A_r}{A_e}$. Purely from geometry, but an
important result.

If we have something that is diffraction-limited, then $\Delta \theta \sim
\frac{\lambda}{R}$. This means that $\Omega_r \approx \Delta\theta^2 \sim
\frac{\lambda^2}{R^2}$. Since our area goes as $\pi R^2$, $\Omega_r A_r =
\lambda^2$. With these two sets of equations, we can look at various
situations in astronomy. We'll do that rapidly at the beginning of next
lecture. I will also probably speak about phonons on Friday, and we'll see
if we can start the Fermi-Dirac/Bose-Einstein.