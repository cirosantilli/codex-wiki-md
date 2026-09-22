<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the generators $e,f,h$ of the [sl2 Lie algebra](../../../../../../sl2-lie-algebra.md) with $[h,e]=2e$, $[h,f]=-2f$, and $[e,f]=h$. For a finite-dimensional [Lie algebra representation](../../../../../../lie-algebra-representation.md), $h$ is diagonalizable with integral [weights](../../../../../../weight-representation-theory.md). Its [formal character of a weight module](../../../../../../formal-character-of-a-weight-module.md) is

$$
\boxed{\operatorname{ch}V=\sum_{m\in\mathbb Z}(\dim V_m)q^m,\qquad V_m=\{v:hv=mv\}.}
$$

Here $q$ is a formal variable; equivalently the expression is $\operatorname{tr}_V(q^h)$, or the formal sum $\sum_m(\dim V_m)e^m$ with $e^m=q^m$. This records every [weight multiplicity](../../../../../../weight-multiplicity.md), rather than only the [dimension](../../../../../../dimension-vector-space.md).

The [classification of finite-dimensional sl2 representations](../../../../../../classification-of-finite-dimensional-sl2-representations.md) says that $L_d$, the irreducible of [highest weight](../../../../../../highest-weight-of-a-representation.md) $d\ge0$, has the [weight](../../../../../../weight-representation-theory.md) string $d,d-2,\ldots,-d$, each with multiplicity one. Hence

$$
\operatorname{ch}L_d=q^d+q^{d-2}+\cdots+q^{-d}=\frac{q^{d+1}-q^{-(d+1)}}{q-q^{-1}}.
$$

The quotient denotes the displayed [Laurent polynomial](../../../../../../laurent-polynomial.md) and has the removable value $d+1$ at $q=1$. [Formal characters](../../../../../../formal-character-of-a-weight-module.md) are additive on [direct sums](../../../../../../direct-sum.md), so these formulas determine the character of every finite-dimensional module.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
