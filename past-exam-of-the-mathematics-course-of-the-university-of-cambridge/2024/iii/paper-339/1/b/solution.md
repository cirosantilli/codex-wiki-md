<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Associate a nonnegative [Lagrange multiplier](../../../../../../lagrange-multiplier.md) $\lambda_i$ with each inequality. The [Lagrangian dual problem](../../../../../../lagrangian-dual-problem.md) begins with

$$
L(x,\lambda)=c^Tx+\lambda^T(Ax-b)
=(c+A^T\lambda)^Tx-b^T\lambda,
\qquad \lambda\geq0.
$$

Its infimum over $x\in\mathbb R^n$ is finite exactly when $A^T\lambda+c=0$, in which case it equals $-b^T\lambda$. The dual [linear program](../../../../../../linear-programming.md) is consequently

$$
\boxed{\max_{\lambda\in\mathbb R^m}
\{-b^T\lambda:A^T\lambda+c=0,\ \lambda\geq0\}}.
$$

For any primal-feasible $x$ and dual-feasible $\lambda$,

$$
-b^T\lambda
\leq-x^TA^T\lambda
=c^Tx,
$$

which proves [weak duality](../../../../../../weak-duality.md). [Strong duality](../../../../../../strong-duality.md) means equality of the two optimal values. The stated strict feasibility is the [Slater condition](../../../../../../slater-s-condition.md); together with finiteness of the primal optimum it gives strong duality and an attained dual optimum $\lambda^*$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
