<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the [generalized measurement postulate](../../../../../../generalized-measurement-postulate.md), outcome $m$ is described by a [Kraus operator](../../../../../../kraus-operator.md) $M_m$, with $\sum_mM_m^\dagger M_m=I$. On a [density operator](../../../../../../density-matrix.md) $\rho$ its probability and conditional output, for nonzero probability, are

$$
\boxed{p_m=\operatorname{Tr}(M_m\rho M_m^\dagger),\qquad
\rho_m=M_m\rho M_m^\dagger/p_m}.
$$

For a pure input the conditional vector is $M_m|\psi\rangle/\sqrt{p_m}$. The effects $E_m=M_m^\dagger M_m$ are positive and sum to the identity, defining a [positive operator-valued measure](../../../../../../positive-operator-valued-measure.md).

More generally an outcome can have several [Kraus operators](../../../../../../kraus-operator.md) $M_{m\alpha}$. Then sum over $\alpha$ in both the numerator and the probability, and require $\sum_{m,\alpha}M_{m\alpha}^\dagger M_{m\alpha}=I$.

The usual [projective measurement](../../../../../../projective-measurement.md) with the [Lüders rule](../../../../../../luders-rule.md) is recovered when the measurement operators are mutually orthogonal projections, $M_m=P_m=P_m^\dagger=P_m^2$, $P_mP_n=0$ for $m\ne n$, and $\sum_mP_m=I$. Projector-valued effects alone give projective outcome statistics; to obtain the Lüders state update as well, the instrument must implement $\rho\mapsto P_m\rho P_m$, without an additional conditional state change.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
