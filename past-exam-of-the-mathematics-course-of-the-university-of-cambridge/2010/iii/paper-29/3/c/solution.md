<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under [Wiener measure](../../../../../../wiener-measure.md), $dX_t=dW_t$ and

$$
[M]_t=\int_0^t\frac{ds}{X_s^2}\qquad(t\le\tau).
$$

The definition of the [stochastic exponential](../../../../../../doleans-dade-exponential.md) gives

$$
d\log Z_t=\frac{dX_t}{X_t}-\frac{dt}{2X_t^2}.
$$

On the other hand, the [Itô formula](../../../../../../ito-s-lemma.md) applied to the logarithm gives precisely

$$
d\log X_t=\frac{dX_t}{X_t}-\frac{dt}{2X_t^2}.
$$

Their initial values differ by $\log x$, so

$$
\boxed{\log Z_t=\log X_t-\log x,\qquad Z_t=X_t/x\quad(t\le\tau),}
$$

[almost surely](../../../../../../almost-sure-convergence.md) under [Wiener measure](../../../../../../wiener-measure.md). In particular,

$$
Z_\tau=\frac Mx\mathbf1_{\{T_M<T_\varepsilon\}}
+\frac\varepsilon x\mathbf1_{\{T_\varepsilon<T_M\}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
