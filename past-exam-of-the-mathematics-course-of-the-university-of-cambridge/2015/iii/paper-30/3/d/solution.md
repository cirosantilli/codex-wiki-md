<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because $K$ is continuous, adapted, and strictly positive, $K^{-1/2}$ is predictable and locally integrable against $M$. Define

$$
\boxed{W_t=\int_0^t K_s^{-1/2}\,dM_s,\qquad H_t=\sqrt{K_t}.}
$$

The [quadratic variation of a stochastic integral](../../../../../../quadratic-variation-of-a-stochastic-integral.md) is

$$
\langle W\rangle_t=\int_0^t K_s^{-1}\,d\langle M\rangle_s=t.
$$

Thus $W$ starts at zero and is a [continuous local martingale](../../../../../../continuous-local-martingale.md) with bracket $t$. The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) makes it a [Brownian motion](../../../../../../brownian-motion-split.md) in the original filtration.

The process $H$ is continuous and adapted, and $\int_0^tH_s^2\,ds=\int_0^tK_s\,ds<\infty$ almost surely. The [associativity of stochastic integration](../../../../../../associativity-of-stochastic-integration.md) gives

$$
\boxed{\int_0^tH_s\,dW_s
=\int_0^t\sqrt{K_s}K_s^{-1/2}\,dM_s=M_t-M_0.}
$$

This is the [stochastic-integral representation from absolutely continuous quadratic variation](../../../../../../stochastic-integral-representation-from-absolutely-continuous-quadratic-variation.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
