<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $N$ distinguishable lattice sites occupied by $N_i$ mutually indistinguishable atoms of each species, the number of configurations is

$$
\Omega=\frac{N!}{\prod_{i=1}^nN_i!},\qquad
N_i=X_iN,\quad\sum_iX_i=1.
$$

Using [Stirling's approximation](../../../../../stirling-formula.md),

$$
\ln\Omega\simeq
N\ln N-\sum_iN_i\ln N_i
=-N\sum_iX_i\ln X_i.
$$

For one mole, $N=N_A$ and $k_BN_A=R$, so

$$
\Delta S_{\rm mix}=-R\sum_iX_i\ln X_i.
$$

[Equiatomic configurational entropy](../../../../../equiatomic-configurational-entropy.md) follows when the composition has $X_i=1/n$, giving

$$
\boxed{\Delta S_{\rm mix}=R\ln n.}
$$

The reference is the unmixed configurational arrangement, and the model assumes random site occupation without [short-range order](../../../../../short-range-order.md). It counts [configurational entropy](../../../../../configurational-entropy.md), not all vibrational, electronic or magnetic [entropy](../../../../../entropy-split.md). A large number of elements does not by itself guarantee a stable single [solid solution](../../../../../solid-solution.md): competing [thermodynamic phases](../../../../../thermodynamic-phase.md) and the [enthalpy](../../../../../enthalpy-split.md) term also enter the [Gibbs free energy](../../../../../gibbs-free-energy.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the materials science course of the University of Cambridge](../../../../split.md)
6. [Materials science course of the University of Cambridge](../../../../../materials-science-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
