<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Set

$$
B=I-\gamma A^*A.
$$

Starting from $x_0=0$, repeated substitution in [Landweber iteration](../../../../../../landweber-iteration.md) gives

$$
\boxed{
x_{n+1}
=\gamma\sum_{k=0}^{n}
(I-\gamma A^*A)^kA^*y}.
$$

This is the finite partial sum of a [Neumann series](../../../../../../neumann-series.md). Whenever $A^*A$ is boundedly invertible on the relevant subspace and $\lVert I-\gamma A^*A\rVert<1$,

$$
\boxed{
(A^*A)^{-1}
=\gamma\sum_{k=0}^{\infty}
(I-\gamma A^*A)^k},
$$

so

$$
x_{n+1}\longrightarrow
(A^*A)^{-1}A^*y=A^\dagger y.
$$

For a genuinely compact operator on an infinite-dimensional space, nonzero singular values can accumulate at zero, so this inverse is generally unbounded and the Neumann series need not converge in operator norm. Under the condition in part ii it nevertheless converges componentwise on admissible data to the [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md); stopping after finitely many terms suppresses poorly determined small-singular-value components and acts as a [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
