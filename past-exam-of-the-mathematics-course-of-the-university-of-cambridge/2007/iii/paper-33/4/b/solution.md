<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Monotonicity of $f$ gives, for each $n\geq1$,

$$
f(2^{-n})\log2\leq\int_{2^{-n}}^{2^{-(n-1)}}f(t)\frac{dt}{t}.
$$

Hence $\sum_{n\geq1}f(2^{-n})<\infty$; the additional $n=0$ term is finite by continuity at one. Also $f(t)\to0$ as $t\downarrow0$, since a positive limiting lower bound would make the integral diverge.

By [Brownian scaling](../../../../../../brownian-scaling.md), $S_{2^{-n-1}}$ has law $2^{-(n+1)/2}S_1$. Apply the small-value bound for the [Brownian running maximum](../../../../../../brownian-running-maximum.md) to obtain

$$
\begin{aligned}
\mathbb P\left(S_{2^{-n-1}}<2^{-n/2}f(2^{-n})\right)
&=\mathbb P(S_1<\sqrt2 f(2^{-n}))\\
&\leq\frac2{\sqrt\pi}f(2^{-n}).
\end{aligned}
$$

Summing yields **the requested finite [probability](../../../../../../probability.md) sum**. The argument needs no [independence](../../../../../../independent-random-variables.md) of these nested-time events.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
