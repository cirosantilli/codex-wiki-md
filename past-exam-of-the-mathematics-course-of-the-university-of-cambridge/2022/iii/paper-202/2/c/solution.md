<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Cameron-Martin theorem](../../../../../../cameron-martin-theorem.md) on Wiener space says that the translated measure $\mathbb P_h(A)=\mathbb P(X+h\in A)$ is equivalent to Wiener measure precisely when $h$ is absolutely continuous, $h(0)=0$, and $\dot h\in L^2(\mathbb R_+)$. In that case

$$
\frac{d\mathbb P_h}{d\mathbb P}
=\exp\left(
\int_0^\infty\dot h_s\,dX_s
-\frac12\int_0^\infty\dot h_s^2\,ds\right).
$$

For such $h$, the exponential is a uniformly integrable [stochastic exponential](../../../../../../doleans-dade-exponential.md). Under the measure defined by this density, the [Girsanov theorem](../../../../../../girsanov-theorem.md) makes $X_t-\int_0^t\dot h_sds=X_t-h(t)$ a Brownian motion. This identifies the translated law and proves equivalence; replacing $h$ by $-h$ gives the inverse density.

If $h$ fails the Cameron-Martin condition on some finite interval, the finite-horizon theorem gives singularity there. If it belongs locally but $\int_0^\infty\dot h_s^2ds=\infty$, the log likelihood is a Brownian motion run at that diverging energy clock minus half the clock. It tends to $-\infty$ under one measure and to $+\infty$ under the translate, producing disjoint full-measure events. Thus the measures are singular.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
