<h1 id="40c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $U_m^n=u(mh,nk)$ be the sampled exact solution and let $A_h$ denote the update matrix of the [Forward Euler diffusion scheme](../../../../../../forward-euler-diffusion-scheme.md). For $0\leq\mu\leq1/2$,

$$
(A_hv)_m=\mu v_{m-1}+(1-2\mu)v_m+\mu v_{m+1}
$$

is a convex combination, with the homogeneous boundary values included. Therefore

$$
\|A_hv\|_\infty\leq\|v\|_\infty.
$$

This is the parabolic [discrete maximum principle](../../../../../../discrete-maximum-principle.md) and proves max-norm stability directly.

The [Taylor theorem](../../../../../../taylor-theorem.md) and the [second-order central difference](../../../../../../second-order-central-difference.md) give the exact-grid residual

$$
U^{n+1}=A_hU^n+k\tau^n,
\qquad
\|\tau^n\|_\infty\leq C(k+h^2)
$$

for a sufficiently smooth solution on a fixed interval $0\leq t\leq T$. If $e^n=U^n-u^n$, then

$$
\|e^{n+1}\|_\infty\leq\|e^n\|_\infty+k\|\tau^n\|_\infty.
$$

Iteration for $nk\leq T$ yields

$$
\boxed{\|e^n\|_\infty\leq\|e^0\|_\infty+CT(k+h^2)\longrightarrow0.}
$$

**Thus $\mu\leq1/2$ implies convergence when the initial grid values converge to the initial data.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40C](../../40c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
