<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An ensemble with normalized quantum states $|\psi_a\rangle$ and probabilities $p_a\geq0$, $\sum_ap_a=1$, has [density matrix](../../../../density-matrix-split.md)

$$
\boxed{\rho=\sum_a p_a|\psi_a\rangle\langle\psi_a|}.
$$

Each rank-one projector is [Hermitian](../../../../hermitian-operator.md), so $\rho^\dagger=\rho$. Taking the [trace](../../../../matrix-trace.md) in any [orthonormal basis](../../../../orthonormal-basis.md) gives

$$
\operatorname{Tr}\rho=\sum_a p_a\langle\psi_a|\psi_a\rangle=1.
$$

It is also positive: $\langle v|\rho|v\rangle=\sum_ap_a|\langle\psi_a|v\rangle|^2\geq0$. Its [eigenvalues](../../../../eigenvalue.md) $\lambda_a$ are therefore nonnegative and sum to one. Hence

$$
\operatorname{Tr}\rho^2=\sum_a\lambda_a^2\leq\left(\sum_a\lambda_a\right)^2=1,
$$

with equality exactly when one [eigenvalue](../../../../eigenvalue.md) is one and the others are zero. Thus the [purity of a density operator](../../../../purity-of-a-density-operator.md) distinguishes

$$
\boxed{\text{pure state: }\operatorname{Tr}\rho^2=1,\qquad
\text{mixed state: }\operatorname{Tr}\rho^2<1}.
$$

Equivalently, a [pure state](../../../../pure-state.md) has $\rho^2=\rho$ and rank one. In a $d$-dimensional [Hilbert space](../../../../hilbert-space-split.md), purity is at least $1/d$, attained by the [maximally mixed state](../../../../maximally-mixed-state.md) $I/d$.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
