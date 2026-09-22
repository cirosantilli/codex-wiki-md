<h1 id="40e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $e_1=(1,0,\ldots,0)^T$. The displayed lower-bidiagonal matrix $Q$ satisfies

$$
A=QQ^T+e_1e_1^T.
$$

Since $P=Q^{-1}$, the [Preconditioned conjugate gradient method](../../../../../../preconditioned-conjugate-gradient-method.md) uses

$$
PAP^T
=I+(Pe_1)(Pe_1)^T.
$$

Solving $Qz=e_1$ gives

$$
z=Pe_1=(1,-1,1,-1,\ldots)^T,
\qquad
z^Tz=n.
$$

The rank-one matrix $I+zz^T$ has eigenvalue $1+n$ in the direction $z$ and eigenvalue $1$ on the $(n-1)$-dimensional orthogonal complement of $z$. It therefore has only two distinct eigenvalues. Part (b) gives

$$
\boxed{\text{the preconditioned method terminates after at most two iterations}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [40E](../../40e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
