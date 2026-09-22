<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $0\leq\lambda<c^{-1}$. Since $X$ is centered, the elementary inequality $\log u\leq u-1$ gives

$$
\log\mathbb E e^{\lambda X}
\leq\mathbb E(e^{\lambda X}-1-\lambda X).
$$

On ${X\leq0}$, use $e^u-1-u\leq u^2/2$ for $u\leq0$; on ${X>0}$, expand the [exponential function](../../../../../../exponential-function.md) into its [power series](../../../../../../power-series.md). The hypotheses therefore give

$$
\begin{aligned}
\mathbb E(e^{\lambda X}-1-\lambda X)
&\leq\frac{\lambda^2}{2}\mathbb E X^2
 +\sum_{q=3}^\infty\frac{\lambda^q}{q!}\mathbb E X_+^q\\
&\leq\frac{\sigma^2\lambda^2}{2}
 +\frac{\sigma^2}{2}\sum_{q=3}^\infty\lambda^qc^{q-2}
=\frac{\sigma^2\lambda^2}{2(1-c\lambda)}.
\end{aligned}
$$

This is precisely the [Sub-Gamma random variable in the right tail](../../../../../../sub-gamma-random-variable-in-the-right-tail.md) bound with variance parameter $\sigma^2$ and scale parameter $c$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
