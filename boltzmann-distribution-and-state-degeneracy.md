# Boltzmann distribution and state degeneracy

↑ **Parent:** [Boltzmann distribution](boltzmann-distribution.md)

Group [microstates](microstate.md) by their [energy](energy-split.md) $E$. The [state degeneracy](state-degeneracy.md) $g(E)$ counts how many [microstates](microstate.md) have that [energy](energy-split.md); their aggregate [probability](probability.md) is

$$
P(E)=\sum_{i:E_i=E}p_i=\frac{g(E)e^{-\beta E}}{Z},\qquad
Z=\sum_{\text{distinct }E}g(E)e^{-\beta E}.
$$

Here $P(E)$ is the [probability](probability.md) of the [macrostate](macrostate.md) retaining only [energy](energy-split.md), while $p_i$ is the [probability](probability.md) of one individual [microstate](microstate.md). For two such [macrostates](macrostate.md),

$$
\frac{P(E_a)}{P(E_b)}=\frac{g(E_a)}{g(E_b)}e^{-\beta(E_a-E_b)}.
$$

Counting more [microstates](microstate.md) can compensate for a smaller [Boltzmann factor](boltzmann-factor.md). Omitting the [state degeneracy](state-degeneracy.md) confuses a sum over [microstates](microstate.md) with a sum over distinct [energies](energy-split.md). [MIT 5.62, spring 2008, lecture 3, page 4: degeneracy and the aggregate energy probability](https://ocw.mit.edu/courses/5-62-physical-chemistry-ii-spring-2008/bda82786b6014d3f468798339f658629_03_562ln08.pdf)

## ↑ Ancestors (6)

1. [Boltzmann distribution](boltzmann-distribution.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
