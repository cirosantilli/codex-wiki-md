# Polynomial reduction of matrix powers

↑ **Parent:** [Cayley-Hamilton theorem](cayley-hamilton-theorem-split.md)

By [polynomial division](polynomial-division.md), write $f(t)=q(t)\chi_A(t)+r(t)$ with $\deg r<n$. Because $\chi_A$ is a [monic polynomial](monic-polynomial.md), this division works even over a [commutative ring](commutative-ring.md). Evaluating at $A$ makes the multiple of $\chi_A(A)$ vanish, leaving $f(A)=r(A)$. This explains the reduction in [two-coefficient reduction of matrix powers](two-coefficient-reduction-of-matrix-powers.md) without multiplying out every intermediate [matrix](matrix.md).

Over a [field](field.md), the [minimal polynomial](minimal-polynomial.md) $m_A$ divides $\chi_A$ and gives the strongest such universal reduction: use the [polynomial remainder](remainder-of-polynomial-division.md) modulo $m_A$ instead. For the [scalar matrix](scalar-matrix.md) $2I_2$, the [characteristic polynomial](characteristic-polynomial.md) is $(t-2)^2$, while the [minimal polynomial](minimal-polynomial.md) is only $t-2$. Every [matrix power](matrix-power.md) is then a scalar multiple of $I_2$.

## ↑ Ancestors (8)

1. [Cayley-Hamilton theorem](cayley-hamilton-theorem-split.md)
2. [Minimal polynomial](minimal-polynomial.md)
3. [Operator theory](linear-operator-theory-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
