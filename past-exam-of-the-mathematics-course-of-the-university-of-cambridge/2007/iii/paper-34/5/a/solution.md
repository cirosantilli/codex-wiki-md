<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [generalized measurement postulate](../../../../../../generalized-measurement-postulate.md) specifies [Kraus operators](../../../../../../kraus-operator.md) $M_{i\alpha}$, where $i$ is the recorded outcome and $\alpha$ permits unobserved alternatives for that outcome, satisfying

$$
\boxed{\sum_{i,\alpha}M_{i\alpha}^\dagger M_{i\alpha}=I.}
$$

For a [density operator](../../../../../../density-matrix.md) $\rho$, outcome $i$ has probability and conditional state

$$
\boxed{p_i=\operatorname{Tr}\left(\rho\sum_\alpha M_{i\alpha}^\dagger M_{i\alpha}\right),\qquad
\rho_i=\frac{\sum_\alpha M_{i\alpha}\rho M_{i\alpha}^\dagger}{p_i}\quad(p_i>0).}
$$

With one operator per outcome, this is the usual formula $p_i=\operatorname{Tr}(M_i\rho M_i^\dagger)$, $\rho_i=M_i\rho M_i^\dagger/p_i$. The positive operators $E_i=\sum_\alpha M_{i\alpha}^\dagger M_{i\alpha}$ form a [POVM](../../../../../../positive-operator-valued-measure.md), while the state-update maps form a [quantum instrument](../../../../../../quantum-instrument.md).

The full postulate reduces to the usual [projective measurement](../../../../../../projective-measurement.md) with the Lüders update when there is one operator per outcome and $M_i=P_i$, with $P_i=P_i^\dagger=P_i^2$, $P_iP_j=0$ for $i\ne j$, and $\sum_iP_i=I$. Then $p_i=\operatorname{Tr}(P_i\rho)$ and $\rho_i=P_i\rho P_i/p_i$. Projective effects $E_i=P_i$ alone ensure these probabilities but do not fix the state update: an additional outcome-dependent unitary could still be applied. The choice $M_i=P_i$ makes the required projective state-update condition explicit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
