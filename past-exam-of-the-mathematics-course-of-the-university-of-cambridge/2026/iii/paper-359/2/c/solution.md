<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $q=2p+2$ and multiply the vorticity equation by $\omega^{q-1}$, first for an odd power as in the hint. Periodic [integration by parts](../../../../../../integration-by-parts.md) and $\nabla\mathbin\cdot u=0$ give

$$
\nu(q-1)\int_\Omega\omega^{q-2}|\nabla\omega|^2\,dx
+\gamma\|\omega\|_q^q
=\int_\Omega g\omega^{q-1}\,dx.
$$

The diffusion term is nonnegative, while the [Holder inequality](../../../../../../holder-inequality.md) bounds the right-hand side by $\|g\|_q\|\omega\|_q^{q-1}$. Consequently

$$
\gamma\|\omega\|_q\leq\|g\|_q.
$$

On the finite-volume torus, $L^q$ norms increase to the [essential supremum](../../../../../../essential-supremum.md) as $q\to\infty$. Hence the [damped-vorticity maximum estimate](../../../../../../damped-vorticity-maximum-estimate.md) gives

$$
\boxed{\gamma\|\omega\|_\infty\leq\|g\|_\infty}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 359](../../../paper-359-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
