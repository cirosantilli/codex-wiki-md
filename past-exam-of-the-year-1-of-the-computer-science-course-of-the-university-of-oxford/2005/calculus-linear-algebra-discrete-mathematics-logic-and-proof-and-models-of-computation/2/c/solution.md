<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\lambda$ be the single [eigenvalue](../../../../../eigenvalue.md). By [diagonalizability](../../../../../diagonalizable-matrix.md), there is a [basis](../../../../../basis.md) $v_1,\ldots,v_n$ of [eigenvectors](../../../../../eigenvector.md), and every corresponding [eigenvalue](../../../../../eigenvalue.md) is $\lambda$. For any $v=\sum_i a_iv_i$, [linearity](../../../../../linearity.md) gives

$$
T(v)=\sum_i a_iT(v_i)=\sum_i a_i\lambda v_i=\lambda v.
$$

Thus $\boxed{T=\lambda I}$, a [scalar multiple](../../../../../scalar-multiple.md) of the [identity map](../../../../../identity-function.md).

A counterexample to the conclusion without [diagonalizability](../../../../../diagonalizable-matrix.md) is

$$
\boxed{J=\begin{pmatrix}2&1\\0&2\end{pmatrix}.}
$$

Its [characteristic polynomial](../../../../../characteristic-polynomial.md) is $(t-2)^2$, but $(J-2I)(a,b)^\mathsf T=(b,0)^\mathsf T$. The [eigenspace](../../../../../eigenspace.md) for $2$ is therefore $\operatorname{span}\{(1,0)^\mathsf T\}$, of [dimension](../../../../../dimension-vector-space.md) one. There is no [basis](../../../../../basis.md) of [eigenvectors](../../../../../eigenvector.md) in [dimension](../../../../../dimension-vector-space.md) two, so $J$ is not [diagonalizable](../../../../../diagonalizable-matrix.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
