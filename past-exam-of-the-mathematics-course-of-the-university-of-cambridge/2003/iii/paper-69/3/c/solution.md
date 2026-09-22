<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a [best uniform approximation](../../../../../../best-uniform-approximation.md) $p_n\in\mathcal P_n$. It exists because this [vector subspace](../../../../../../vector-subspace.md) is a [finite-dimensional vector space](../../../../../../finite-dimensional-vector-space.md) and a minimizing sequence $q_j$ is bounded: $\|q_j\|_\infty\le\|f\|_\infty+\|f-q_j\|_\infty$. [Finite-dimensional equivalence of norms](../../../../../../finite-dimensional-equivalence-of-norms.md) then supplies a convergent subsequence of coefficients. If $E_n(f)>0$, the [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) gives $n+2$ alternating error extrema. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) supplies a zero $x_{n,k}$ of $f-p_n$ in each of the $n+1$ intervening open intervals. These [interpolation nodes](../../../../../../interpolation-node.md) are distinct, and uniqueness of [polynomial interpolation](../../../../../../polynomial-interpolation.md) gives

$$
\boxed{\ell_n(f)=p_n,\qquad \|\ell_n(f)-f\|_\infty=E_n(f)\longrightarrow0}.
$$

The convergence follows from the [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md). If $E_n(f)=0$, choose any $n+1$ distinct nodes: the [polynomial interpolant](../../../../../../lagrange-polynomial.md) is still $f=p_n$. This constructs [interpolation nodes from best uniform approximation](../../../../../../interpolation-nodes-from-best-uniform-approximation.md); the nodes depend on $f$, and no universal node system for all [continuous functions](../../../../../../continuous-function.md) is asserted.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
