# Additivity of Boltzmann entropy

↑ **Parent:** [Boltzmann's entropy formula](boltzmann-s-entropy-formula.md)

For two subsystems with independently specified [macrostates](macrostate.md), suppose every allowed [microstate](microstate.md) of $A$ can be paired with every allowed [microstate](microstate.md) of $B$. Their allowed set is a [Cartesian product](cartesian-product.md). With equal [probability](probability.md) for each pair, [Boltzmann's entropy formula](boltzmann-s-entropy-formula.md) gives

$$
\Omega_{AB}=\Omega_A\Omega_B,\qquad
S_{AB}=k_B\ln(\Omega_A\Omega_B)=S_A+S_B.
$$

For example, take two [independent](independent-random-variables.md) copies of the toy model, each with two labels choosing between its two boxes. Each copy has four configurations and [Boltzmann entropy](boltzmann-s-entropy-formula.md) $k_B\ln4$. Combining their [independent](independent-random-variables.md) labels gives sixteen configurations and [Boltzmann entropy](boltzmann-s-entropy-formula.md) $k_B\ln16=2k_B\ln4$. This explains why [entropy](entropy.md) adds even though microscopic counts multiply. [MIT, §7.4, equation 7.17: independent state counts multiply](https://web.mit.edu/16.unified/www/FALL/thermodynamics/notes/node57.html)

The product assumption matters. A constraint shared between the subsystems can forbid some pairs; for example, fixing only their combined [energy](energy.md) generally requires summing over its possible divisions. See [entropy maximization under thermal contact](entropy-maximization-under-thermal-contact.md) for how [thermal equilibrium](thermal-equilibrium.md) selects the dominant division. Statistical [independence](independent-random-variables.md) cannot be inferred merely from drawing a boundary between two parts.

## ↑ Ancestors (7)

1. [Boltzmann's entropy formula](boltzmann-s-entropy-formula.md)
2. [Entropy](entropy.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Boltzmann's entropy formula](boltzmann-s-entropy-formula.md)
