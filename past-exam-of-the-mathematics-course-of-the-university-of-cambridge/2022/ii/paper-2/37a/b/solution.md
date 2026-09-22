<h1 id="37a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [Gibbs entropy](../../../../../../gibbs-entropy.md)

$$
S=-k_B\sum_n p_n\log p_n,
$$

first maximize subject only to $\sum_np_n=1$ over $\Omega$ accessible microstates. A [Lagrange multiplier](../../../../../../lagrange-multiplier.md) gives

$$
-(\log p_n+1)+\alpha=0,
$$

so every $p_n$ is equal. Normalization yields the [microcanonical ensemble](../../../../../../microcanonical-ensemble.md)

$$
\boxed{p_n=\frac1\Omega}.
$$

For the canonical ensemble, impose both normalization and the mean-energy constraint $\sum_np_nE_n=E$. Stationarity of

$$
-\sum_np_n\log p_n-\alpha\sum_np_n-\beta\sum_np_nE_n
$$

gives $p_n=C e^{-\beta E_n}$. The [canonical partition function](../../../../../../canonical-partition-function.md) fixes $C$, so

$$
\boxed{p_n=\frac{e^{-\beta E_n}}{Z}},
\qquad
Z=\sum_ne^{-\beta E_n}.
$$

Thermodynamic consistency identifies $\beta=(k_BT)^{-1}$. This is the [maximum-entropy derivation of equilibrium ensembles](../../../../../../maximum-entropy-derivation-of-equilibrium-ensembles.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [37A](../../37a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
