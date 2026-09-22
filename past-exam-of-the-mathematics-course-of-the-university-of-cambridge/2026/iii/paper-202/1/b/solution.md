<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $K_t=\sqrt{H_t}$ and define the [stochastic integral](../../../../../../stochastic-integral.md)

$$
W_t=\int_0^t\frac1{\sqrt{H_s}}\,dX_s.
$$

Strict positivity and predictability of $H$ make the integrand locally admissible. The process $W$ is a continuous local martingale starting from zero, and the [quadratic variation of a stochastic integral](../../../../../../quadratic-variation-of-a-stochastic-integral.md) gives

$$
[W]_t=\int_0^t\frac1{H_s}\,d[X]_s
=\int_0^t\frac1{H_s}H_s\,ds=t.
$$

By the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md), $W$ is a Brownian motion. The [associativity of stochastic integration](../../../../../../associativity-of-stochastic-integration.md) then yields

$$
\int_0^tK_s\,dW_s
=\int_0^t\sqrt{H_s}\frac1{\sqrt{H_s}}\,dX_s
=X_t-X_0,
$$

which is the required representation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
