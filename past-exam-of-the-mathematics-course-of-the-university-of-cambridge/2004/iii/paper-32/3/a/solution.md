<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [generalized measurement postulate](../../../../../../generalized-measurement-postulate.md) specifies operators $M_i$ with $\sum_iM_i^\dagger M_i=I$. On a [density matrix](../../../../../../density-matrix.md) $\rho$, the outcome probability and conditional state are

$$
p_i=\operatorname{Tr}(M_i\rho M_i^\dagger),\qquad
\rho_i=\frac{M_i\rho M_i^\dagger}{p_i}\quad(p_i>0).
$$

The probabilities are nonnegative and sum to one. More generally an outcome may contain several [Kraus operators](../../../../../../kraus-operator.md) $M_{i\alpha}$, in which case one sums over $\alpha$ in both formulas. A [projective measurement](../../../../../../projective-measurement.md) with the usual Lüders update is the special case $M_i=P_i$, where $P_i=P_i^\dagger$, $P_iP_j=\delta_{ij}P_i$ and $\sum_iP_i=I$. Projection-valued effects alone fix the projective outcome probabilities, but an additional outcome-dependent unitary can change the conditional state; for the standard projective update the measurement operators themselves are the projectors.

A [POVM](../../../../../../positive-operator-valued-measure.md) is a family of positive effects $E_i$ summing to $I$. Its probabilities are $p_i=\operatorname{Tr}(\rho E_i)$. A [generalized measurement](../../../../../../generalized-measurement-postulate.md) gives effects $E_i=M_i^\dagger M_i$, or $E_i=\sum_\alpha M_{i\alpha}^\dagger M_{i\alpha}$. Conversely $M_i=\sqrt{E_i}$ realizes any [POVM](../../../../../../positive-operator-valued-measure.md). The [POVM does not determine the post-measurement state](../../../../../../povm-does-not-determine-the-post-measurement-state.md): different operators with these same effects have the same probabilities and can have different state updates.

A [pure POVM](../../../../../../pure-positive-operator-valued-measure.md) has rank-one nonzero effects, $E_i=w_i|\psi_i\rangle\langle\psi_i|$, with normalized [pure states](../../../../../../pure-state.md) $|\psi_i\rangle$ and positive $w_i$. Here pure means rank-one effects, not the different property of extremality in the convex set of POVMs.

The [POVM–ensemble duality for the maximally mixed state](../../../../../../povm-ensemble-duality-for-the-maximally-mixed-state.md) is a bijection between POVMs in dimension $d$ and ensemble decompositions of $I/d$. Given effects $E_i$, set

$$
p_i=\frac{\operatorname{Tr}E_i}{d},\qquad \sigma_i=\frac{E_i}{\operatorname{Tr}E_i},
$$

omitting zero effects. Each $\sigma_i$ is a [density matrix](../../../../../../density-matrix.md), $\sum_ip_i=\operatorname{Tr}I/d=1$, and

$$
\sum_ip_i\sigma_i=\frac1d\sum_iE_i=\frac Id.
$$

Conversely, if an ensemble satisfies $\sum_ip_i\sigma_i=I/d$, then $E_i=dp_i\sigma_i$ are positive and sum to $I$, hence form a [POVM](../../../../../../positive-operator-valued-measure.md). Taking traces recovers the original probabilities, so the transformations are inverse. **Pure POVMs correspond exactly to pure-state ensemble decompositions of the maximally mixed state.** For such a POVM, $p_i=w_i/d$ and $\sum_iw_i=d$; it need not be an orthogonal measurement.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
