<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $q_i=a^{ij}D_j u$. If $u$ is a [classical solution](../../../../../../classical-solution.md), multiply $-\partial_iq_i=f$ by a smooth function $v$ and apply the [divergence theorem](../../../../../../divergence-theorem.md). The [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) $q_iN_i=0$ removes the boundary term and gives

$$
\int_Ua^{ij}D_juD_iv
=\int_Ufv.
$$

The [density of smooth functions in a Sobolev space](../../../../../../density-of-smooth-functions-in-a-sobolev-space.md) and boundedness of the coefficients extend this identity to every $v\in H^1(U)$, so $u$ is a [weak solution](../../../../../../weak-solution.md).

Conversely, take $v$ to be a [test function](../../../../../../test-function.md) compactly supported in $U$. The [weak formulation](../../../../../../weak-formulation.md) says

$$
\int_U\bigl[-\partial_i(a^{ij}\partial_ju)-f\bigr]v=0.
$$

The [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives the equation in $U$. Under the regularity implicit in the stated notion of a classical solution, it holds pointwise. Applying [integration by parts](../../../../../../integration-by-parts.md) again with arbitrary $v\in H^1(U)$ leaves

$$
\int_{\partial U}(a^{ij}\partial_ju)N_i\,Tv=0,
$$

where $T$ is the [trace operator](../../../../../../sobolev-trace-theorem.md). Traces of smooth functions can be chosen arbitrarily on the boundary, so the boundary [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives $(a^{ij}\partial_ju)N_i=0$. Thus $u$ is a classical solution.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
