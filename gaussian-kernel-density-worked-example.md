# Gaussian kernel density worked example

↑ **Parent:** [Kernel density estimation](kernel-density-estimation.md)

Take the realized [statistical sample](statistical-sample.md) $(-1,0,1)$, the [Gaussian density kernel](gaussian-density-kernel.md) $\phi(u)=(2\pi)^{-1/2}e^{-u^2/2}$ and [smoothing bandwidth](smoothing-bandwidth.md) $h=1/2$. Then

$$
\widehat f(x)=\frac23\bigl[\phi(2x+2)+\phi(2x)+\phi(2x-2)\bigr].
$$

At $x=0$, the three contributions are $0.03599398$, $0.26596152$, and $0.03599398$, because $\phi(0)=0.39894228$ and $\phi(2)=e^{-2}/\sqrt{2\pi}=0.05399097$. Their sum is

$$
\widehat f(0)=\frac{2(1+2e^{-2})}{3\sqrt{2\pi}}=0.33794948\ldots.
$$

This is a [probability density function](probability-density-function.md) value, not the [probability](probability.md) of observing exactly zero. Each of the three component curves has area $1/3$, despite having a different height at zero.

Let $\Phi$ be the [cumulative distribution function](cumulative-distribution-function.md) of the [standard normal distribution](standard-normal-distribution.md). The fitted [probability](probability.md) of the interval $[-1/2,1/2]$ is its area under the [kernel density estimator](kernel-density-estimation.md):

$$
\begin{aligned}
\int_{-1/2}^{1/2}\widehat f(x)\,dx
&=\frac13\sum_{a\in\{-1,0,1\}}\bigl[\Phi(1-2a)-\Phi(-1-2a)\bigr]\\
&=\frac{[\Phi(3)-\Phi(1)]+[\Phi(1)-\Phi(-1)]+[\Phi(-1)-\Phi(-3)]}{3}\\
&=\frac{0.15730536+0.68268949+0.15730536}{3}=0.33243340\ldots.
\end{aligned}
$$

The shaded area in the diagram is this fitted [probability](probability.md). Its agreement to a few digits with $1/3$ is incidental: the [empirical measure](empirical-measure.md) gives this interval mass $1/3$ exactly, whereas [kernel density estimation](kernel-density-estimation.md) redistributes that mass into neighboring intervals.

## ↑ Ancestors (9)

1. [Kernel density estimation](kernel-density-estimation.md)
2. [Kernel for density estimation](kernel-for-density-estimation.md)
3. [Density estimation](density-estimation.md)
4. [Nonparametric statistics](nonparametric-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
