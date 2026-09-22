<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $f\in C_b^2$. Boundedness of $a,b$ and the derivatives gives a finite bound $\|Lf\|_\infty$. On $0\leq t\leq T$ the assumed local [martingale](../../../../../../martingale-split.md) satisfies

$$
\left|f(X_t)-f(X_0)-\int_0^tLf(X_s)\,ds\right|\leq2\|f\|_\infty+T\|Lf\|_\infty.
$$

It is therefore a bounded local [martingale](../../../../../../martingale-split.md) on this time interval. To check the true [martingale](../../../../../../martingale-split.md) property directly, stop at a localizing sequence, apply its conditional [martingale](../../../../../../martingale-split.md) identity, and pass to the limit by [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) using this deterministic bound. Since $T$ is arbitrary,

$$
\boxed{X\text{ solves the diffusion martingale problem }\mathbf M(a,b).}
$$

The hypothesis for every $C^2$ test function contains the required $C_b^2$ class. No integrability assumption on the unbounded test functions is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
