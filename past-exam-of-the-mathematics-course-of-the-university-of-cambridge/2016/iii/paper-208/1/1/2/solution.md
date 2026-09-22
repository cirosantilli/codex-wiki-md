<h1 id="1/1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the spectral questions take the unique [weakly stationary process](../../../../../../../weakly-stationary-process.md) solving the equation, as is customary for a stable [autoregressive moving-average model](../../../../../../../autoregressive-moving-average-model.md). The equation alone also admits nonstationary solutions differing by $C4^{-t}$, for which a [spectral density of a stationary process](../../../../../../../spectral-density-of-a-stationary-process.md) need not exist. Let $B$ be the [backshift operator](../../../../../../../backshift-operator.md). Since the autoregressive root is $4$, the stationary solution is causal and

$$
X_t=\frac{1-3B}{1-B/4}\eta_t.
$$

Using the convention $\gamma(h)=\int_{-\pi}^{\pi}e^{ih\lambda}f(\lambda)\,d\lambda$, the [spectral density of a stationary process](../../../../../../../spectral-density-of-a-stationary-process.md) is

$$
\boxed{f_X(\lambda)=\frac1{2\pi}\frac{|1-3e^{-i\lambda}|^2}{|1-e^{-i\lambda}/4|^2}
=\frac1{2\pi}\frac{10-6\cos\lambda}{17/16-(\cos\lambda)/2}.}
$$

The stationary mean is zero, since $\mu-\mu/4=0$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 208](../../../../paper-208-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
