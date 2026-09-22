<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $X\sim N(0,\theta^2)$, then $Y=|X|$ has a scaled [half-normal distribution](../../../../../../half-normal-distribution.md) with

$$
G_\theta(y)=2\Phi(y/\theta)-1,
\qquad
g_\theta(y)=\frac2\theta\phi(y/\theta),
\qquad y>0.
$$

Put $c=\Phi^{-1}(3/4)$. The population median is $t_0=\theta c$, and the [asymptotic distribution of a sample median](../../../../../../asymptotic-distribution-of-a-sample-median.md) gives

$$
\boxed{
\sqrt n(T_n-\theta c)
\Longrightarrow
N\left(0,\frac{\theta^2}{16\phi(c)^2}\right)}.
$$

Under $H_0:\theta^2=1$, positivity of the scale means $\theta=1$. If $z_{1-\alpha}$ is the $(1-\alpha)$-quantile of the [standard normal distribution](../../../../../../standard-normal-distribution.md), an asymptotically level-$\alpha$ test rejects for

$$
\boxed{
T_n>c+\frac{z_{1-\alpha}}{4\phi(c)\sqrt n}}.
$$

Larger scale makes the population median $\theta c$ larger, so this is the appropriate one-sided rejection region.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
