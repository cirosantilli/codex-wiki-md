<h1 id="26j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The equilibrium-delay theorem for a [renewal process](../../../../../../renewal-process.md) with positive holding time $S$, finite mean $\mu$, and distribution function $F$ says that the first future renewal must have the [equilibrium residual-life distribution](../../../../../../equilibrium-residual-life-distribution.md),

$$
F_e(t)=\frac1\mu\int_0^t(1-F(s))\,ds\quad(t\ge0),
$$

independently of subsequent ordinary holding times. This is the residual lifetime seen at a stationary observation time, rather than an ordinary inter-renewal lifetime.

Here $\mu=3/\lambda$ and $1-F(t)=e^{-\lambda t}(1+\lambda t+\lambda^2t^2/2)$. Thus the required initial-delay density is

$$
\boxed{f_{S_1^D}(t)=\frac\lambda3e^{-\lambda t}\left(1+\lambda t+\frac{\lambda^2t^2}{2}\right)\mathbf1_{t>0}.}
$$

Equivalently, choose with equal probability a sum of one, two, or three independent rate-$\lambda$ [exponential random variables](../../../../../../exponential-distribution.md). The three [Erlang distributions](../../../../../../erlang-distribution.md) have densities that average to the displayed density. A concrete stationary construction chooses the phase modulo three of a stationary Poisson clock uniformly; the number of exponential stages until its next third-stage renewal is then uniform on $\{1,2,3\}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26J](../../26j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
