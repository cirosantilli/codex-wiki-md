# Boltzmann entropy when a restriction is removed

↑ **Parent:** [Boltzmann's entropy formula](boltzmann-s-entropy-formula.md)

In [Boltzmann entropy of a two-box occupancy](boltzmann-entropy-of-a-two-box-occupancy.md), impose an initial restriction that all labels are left. There is one allowed coarse [microstate](microstate.md). Remove that restriction, allowing all occupancy values: the allowed set is now the union of every occupancy [macrostate](macrostate.md), containing $2^N$ strings. If the final description assigns equal [probability](probability.md) to this whole set, its [Boltzmann entropy](boltzmann-s-entropy-formula.md) change is

$$
\Omega_i=1,\qquad \Omega_f=\sum_{k=0}^N\binom Nk=2^N,\qquad
\Delta S=k_B\ln\frac{\Omega_f}{\Omega_i}=Nk_B\ln2.
$$

The counting identity is the [binomial theorem](binomial-theorem.md). For twenty labels, $\Delta S=20k_B\ln2\approx13.862944k_B$. This final description fixes neither box occupancy; it is coarser than the particular [macrostate](macrostate.md) $k=10$, whose [Boltzmann entropy](boltzmann-s-entropy-formula.md) is $k_B\ln184\,756$. The two counts answer different questions, so substituting the balanced [macrostate](macrostate.md) for the full allowed set would change the calculation.

For four labels, the initial all-left string is `0000`; removing the restriction makes all sixteen strings available. The $k=2$ column has only six strings. Accordingly, the whole allowed set has [Boltzmann entropy](boltzmann-s-entropy-formula.md) $k_B\ln16=4k_B\ln2$, while the balanced [macrostate](macrostate.md) has [Boltzmann entropy](boltzmann-s-entropy-formula.md) $k_B\ln6$.

<a id="image-sixteen-configurations-of-four-labeled-particles-grouped-by-left-occupancy-compared-with-the-all-left-restriction"></a>
![](entropy-two-box-configuration-count.png)

**[Figure 3](#image-sixteen-configurations-of-four-labeled-particles-grouped-by-left-occupancy-compared-with-the-all-left-restriction). Sixteen configurations of four labeled particles grouped by left occupancy, compared with the all-left restriction**.

Removing a barrier changes the allowed set immediately, but it does not instantaneously randomize the actual [probability distribution](probability-distribution-split.md). Motion and equilibration must make those configurations accessible. The counting result illustrates the configurational contribution to [free expansion](free-expansion.md); it does not describe the relaxation time or every contribution to the [entropy](entropy-split.md) of a real [gas](gas.md).

## ↑ Ancestors (7)

1. [Boltzmann's entropy formula](boltzmann-s-entropy-formula.md)
2. [Entropy](entropy-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
