<h1 id="1/1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Here the [innovation process](../../../../../../../innovation-process.md) consists of [linear innovations](../../../../../../../linear-innovation-process.md), the linear one-step prediction errors: $\varepsilon_t=X_t-\operatorname{proj}_{\mathcal H_{t-1}}X_t$, where $\mathcal H_{t-1}$ is the closed linear span of the past $X$'s in $L^2$. For [Gaussian processes](../../../../../../../gaussian-process.md) this is also the [conditional expectation](../../../../../../../conditional-expectation.md) prediction error. For general non-Gaussian [strong white noise](../../../../../../../strong-white-noise.md) these two notions can differ.

**The given $\eta_t$ is not the [linear innovation process](../../../../../../../linear-innovation-process.md).** The moving-average factor has its zero at $1/3$, inside the unit disk, and is noninvertible as a causal moving-average filter. The identity

$$
|1-3e^{-i\lambda}|^2=9|1-e^{-i\lambda}/3|^2
$$

is the [moving-average root reflection](../../../../../../../moving-average-root-reflection.md) that places this zero outside the unit disk. Thus the causal invertible representation has innovation [variance](../../../../../../../variance-split.md) $9$, rather than the given [variance](../../../../../../../variance-split.md) $1$.

For an explicit verification, define

$$
\varepsilon_t=\frac{1-3B}{1-B/3}\eta_t
=\eta_t-8\sum_{j\geq1}3^{-j}\eta_{t-j}.
$$

The filter has constant squared modulus $9$, so $\varepsilon$ is [weak white noise](../../../../../../../weak-white-noise.md) with [variance](../../../../../../../variance-split.md) $9$. The new moving-average factor has root $3$ and is invertible, while its autoregressive factor is causal. Hence the past spans of $X$ and $\varepsilon$ agree, and $X_t-\varepsilon_t$ belongs to that past span. Orthogonality of $\varepsilon_t$ to past $\varepsilon$ therefore identifies it as the [linear innovation process](../../../../../../../linear-innovation-process.md). The [variance](../../../../../../../variance-split.md) difference proves that it cannot be $\eta_t$. If the original noise is Gaussian, the new [linear innovations](../../../../../../../linear-innovation-process.md) are independent Gaussian variables; without Gaussianity they need only be [uncorrelated random variables](../../../../../../../uncorrelated-random-variables.md).

## ↑ Ancestors (12)

1. [3](../3.md)
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
