<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

The [dual vector space](../../../../../linear-functional.md) is $V^*=\operatorname{Hom}_{\mathbb R}(V,\mathbb R)$, the [vector space](../../../../../vector-space-split.md) of all [linear functionals](../../../../../linear-functional.md) on $V$. For a [vector subspace](../../../../../vector-subspace.md) $U\leq V$, its [annihilator of a vector subspace](../../../../../annihilator-of-a-vector-subspace.md) is

$$
U^0=\{\phi\in V^*: \phi(u)=0\text{ for every }u\in U\}.
$$

Given a [basis](../../../../../basis.md) $x_1,\ldots,x_n$, define $x_i^*$ by $x_i^*(x_j)=\delta_{ij}$ and extend linearly. If $\sum_i a_i x_i^*=0$, evaluation at $x_j$ gives $a_j=0$, so the $x_i^*$ are [linearly independent](../../../../../linear-independence.md). Every $\phi\in V^*$ satisfies

$$
\phi=\sum_{i=1}^n\phi(x_i)x_i^*,
$$

so they also [span](../../../../../linear-span.md) $V^*$ and therefore form its [dual basis](../../../../../dual-basis.md).

Write $\phi=a x_1^*+b x_2^*+c x_3^*+d x_4^*$. The condition $\phi\in U^0$ is

$$
a+2b+3c+4d=0,\qquad 5a+6b+7c+8d=0.
$$

[Gaussian elimination](../../../../../gaussian-elimination.md) gives $b=-2c-3d$ and $a=c+2d$. Hence

$$
\boxed{U^0=\operatorname{span}\{x_1^*-2x_2^*+x_3^*,\;2x_1^*-3x_2^*+x_4^*\}.}
$$

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
