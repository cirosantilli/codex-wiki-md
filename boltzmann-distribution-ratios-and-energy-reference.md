# Boltzmann distribution ratios and energy reference

↑ **Parent:** [Boltzmann distribution](boltzmann-distribution.md)

For two individual [microstates](microstate.md), the [partition function](canonical-partition-function.md) cancels:

$$
\frac{p_i}{p_j}=e^{-\beta(E_i-E_j)}.
$$

At positive [temperature](temperature.md), a higher-[energy](energy.md) individual [microstate](microstate.md) is less probable, and equal-[energy](energy.md) individual [microstates](microstate.md) are equally probable. For example, a gap $E_i-E_j=k_BT\ln2$, using the [natural logarithm](natural-logarithm.md), gives $p_i/p_j=1/2$. This comparison concerns individual [microstates](microstate.md); a whole [macrostate](macrostate.md) can contain several of them.

Changing the reference for [energy](energy.md) leaves every [probability](probability.md) unchanged. If all [energies](energy.md) become $E_i'=E_i+C$ for the same constant $C$, then

$$
Z'=e^{-\beta C}Z,\qquad
p_i'=\frac{e^{-\beta(E_i+C)}}{e^{-\beta C}Z}=p_i.
$$

The [partition function](canonical-partition-function.md) itself changes, but its common factor cancels in the [Boltzmann distribution](boltzmann-distribution.md). Thus choosing a [ground state](ground-state.md) [energy](energy.md) of zero simplifies calculations without changing populations. The [expected value](expected-value.md) of [energy](energy.md) shifts by $C$, as it must when its reference changes.

## ↑ Ancestors (6)

1. [Boltzmann distribution](boltzmann-distribution.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
