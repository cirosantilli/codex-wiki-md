<h1 id="9g/solution">Solution</h1>

↑ **Parent:** [9G](../9g.md)

The [dual space](../../../../../dual-space.md) is $V^*=\operatorname{Hom}_F(V,F)$, the [vector space](../../../../../vector-space-split.md) of all [linear functionals](../../../../../linear-functional.md) with pointwise operations. For finite $d=\dim V$, choose a basis $v_1,\ldots,v_d$ and define its [dual basis](../../../../../dual-basis.md) by $\varepsilon_j(v_i)=\delta_{ij}$. Every [linear functional](../../../../../linear-functional.md) is $\ell=\sum_j\ell(v_j)\varepsilon_j$, and evaluation on each $v_i$ proves that the $\varepsilon_j$ are [linearly independent](../../../../../linear-independence.md). Thus **$\dim V^*=\dim V=d$**. This dimension formula is a finite-dimensional assertion.

On the space of [polynomials](../../../../../polynomial-split.md) of degree at most $n$, define the evaluation map $E(p)=(p(a_0),\ldots,p(a_n))$. Its kernel is zero: a nonzero degree-at-most-$n$ [polynomial](../../../../../polynomial-split.md) cannot have $n+1$ distinct roots. Since domain and codomain both have dimension $n+1$, $E$ is an [isomorphism](../../../../../isomorphism.md). The evaluations therefore form a basis of the [dual space](../../../../../dual-space.md). The [linear functional](../../../../../linear-functional.md) $p\mapsto p'(0)$ has a unique expansion in that basis, proving the existence and uniqueness of the requested weights.

Explicitly, use the [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) basis

$$
\ell_j(x)=\prod_{i\ne j}\frac{x-a_i}{a_j-a_i},\qquad p(x)=\sum_{j=0}^np(a_j)\ell_j(x).
$$

The [differentiation weights from nodal evaluations](../../../../../differentiation-weights-from-nodal-evaluations.md) are **$\lambda_j=\ell_j'(0)$**. If a node is zero, no singular reciprocal formula is needed: differentiate the finite product directly. For $n=0$ the sole weight is zero.

## ↑ Ancestors (10)

1. [9G](../9g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
