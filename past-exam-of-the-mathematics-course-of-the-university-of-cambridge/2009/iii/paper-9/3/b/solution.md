<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The appropriate [Poincare-Wirtinger inequality](../../../../../../poincare-wirtinger-inequality.md), with no zero-boundary assumption, is

$$
\boxed{\|u-u_\Omega\|_{L^p(\Omega)}
\leq C_{\Omega,p}\|\nabla u\|_{L^p(\Omega)},\qquad
u_\Omega=\frac1{|\Omega|}\int_\Omega u,\quad1\leq p<n.}
$$

Assume $\Omega$ is nonempty, bounded, connected and has the stated cone property. If this failed, after subtracting the mean and normalizing there would be $u_j\in W^{1,p}(\Omega)$ with

$$
(u_j)_\Omega=0,\qquad \|u_j\|_p=1,\qquad \|\nabla u_j\|_p\longrightarrow0.
$$

The sequence is bounded in $W^{1,p}$. By the permitted [Rellich-Kondrachov compactness theorem](../../../../../../rellich-kondrachov-theorem.md), a subsequence converges strongly in $L^p$ to $u$. For every compactly supported test function, integration by parts and these two convergences show that each [distributional derivative](../../../../../../distributional-derivative.md) of $u$ is zero. A [function with zero weak gradient](../../../../../../sobolev-function-with-zero-weak-gradient.md) is constant on a connected open set: mollification makes it locally constant, and connectedness identifies the local constants.

Convergence in $L^p$ on a finite-measure set also preserves the integral, so $u_\Omega=0$ and the constant is zero. But strong convergence preserves $\|u\|_p=1$, a contradiction. This proves the inequality; connectedness prevents different constants on separate components.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
