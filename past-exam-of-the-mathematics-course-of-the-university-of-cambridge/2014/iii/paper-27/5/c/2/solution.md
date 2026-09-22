<h1 id="5/c/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the positive [exponential Brownian martingale](../../../../../../../exponential-brownian-martingale.md)

$$
M_t=\exp(2\lambda W_t-2\lambda^2t).
$$

The [strong law for Brownian motion](../../../../../../../strong-law-for-brownian-motion.md), $W_t/t\to0$, makes its exponent tend to $-\infty$ and hence $M_t\to0$. If $S=\sup_{t\geq0}(W_t-\lambda t)$, then $\sup M=e^{2\lambda S}$. Part (b) gives, for $x>0$,

$$
\mathbb P(S>x)=e^{-2\lambda x}.
$$

Thus the maximum is exponentially distributed with rate $2\lambda$:

$$
\boxed{f_S(x)=2\lambda e^{-2\lambda x}\mathbf1_{\{x>0\}}.}
$$

There is no atom at zero, by letting $x\downarrow0$ in the tail. This is the [infinite-horizon crossing probability for Brownian motion with negative drift](../../../../../../../infinite-horizon-crossing-probability-for-brownian-motion-with-negative-drift.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Paper 27](../../../../paper-27-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
