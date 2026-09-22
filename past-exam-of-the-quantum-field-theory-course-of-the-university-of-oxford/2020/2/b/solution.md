<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [Hermitian operator](../../../../hermitian-operator.md) $Q$, the [operator exponential](../../../../operator-exponential.md) $C_\lambda=e^{i\lambda Q}$ is a [unitary operator](../../../../unitary-operator.md), with $C_\lambda^\dagger=e^{-i\lambda Q}$. Differentiation and $[Q,C_\lambda]=0$ give

$$
\frac{d}{d\lambda}(C_\lambda A C_\lambda^\dagger)
=iQC_\lambda A C_\lambda^\dagger-iC_\lambda A C_\lambda^\dagger Q
=iC_\lambda[Q,A]C_\lambda^\dagger.
$$

When $[Q,A]=cA$, this is the first-order [ordinary differential equation](../../../../ordinary-differential-equation.md) $A'(\lambda)=icA(\lambda)$ with $A(0)=A$. Multiplication by $e^{-ic\lambda}$ makes its derivative zero, proving

$$
\boxed{A(\lambda)=e^{ic\lambda}A.}
$$

Equivalently, the [commutator expansion for exponential conjugation](../../../../commutator-expansion-for-exponential-conjugation.md) has successive nested [commutators](../../../../commutator.md) $c^r A$, whose [exponential series](../../../../exponential-series.md) sums to this expression.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
