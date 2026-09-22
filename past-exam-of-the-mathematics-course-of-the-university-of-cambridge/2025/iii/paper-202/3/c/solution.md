<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\theta_t=at^{a-1}$. When $a>1/2$,

$$
\int_0^T\theta_t^2dt
=\frac{a^2}{2a-1}T^{2a-1}<\infty.
$$

The integrand is deterministic, so the [Novikov condition](../../../../../../novikov-s-condition.md) holds. Define an [equivalent probability measure](../../../../../../equivalent-probability-measure.md) $Q$ by

$$
\frac{dQ}{dP}
=\exp\left(-\int_0^T\theta_s\,dW_s-
\frac12\int_0^T\theta_s^2ds\right).
$$

The [Cameron-Martin-Girsanov theorem](../../../../../../girsanov-theorem.md) makes

$$
W_t^Q=W_t+\int_0^t\theta_sds=W_t+t^a=S_t
$$

a $Q$-Brownian motion on $[0,T]$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
