# White-noise likelihood for a square-integrable shift

↑ **Parent:** [Gaussian white noise](gaussian-white-noise.md)

Generalized [Gaussian white noise](gaussian-white-noise.md) over a real [Hilbert space](hilbert-space-split.md) $H=L^2$ is an [isonormal Gaussian process](isonormal-gaussian-process.md) $W(h)$ with covariance $\langle h,g\rangle_H$. Its law $P_0$ is carried on a larger observation space; the identity is not the covariance of an infinite-dimensional $H$-valued [Gaussian measure](gaussian-measure.md) because it is not a [trace-class operator](trace-class-operator.md). A deterministic signal $h\in H$ defines a translated observation law $P_h$ with [Radon-Nikodym derivative](radon-nikodym-derivative.md)

$$
\frac{dP_h}{dP_0}(m)=\exp\left(W_m(h)-\tfrac12\|h\|_H^2\right).
$$

In an [orthonormal basis](orthonormal-basis.md), $W_m(h)=\sum_jm_jh_j$ is a stochastic series with total [variance](variance-split.md) $\|h\|_H^2$, not an inner product of two $H$-valued observations. The formula follows from the [Cameron-Martin theorem for a Gaussian measure](cameron-martin-theorem-for-a-gaussian-measure.md) in its generalized white-noise version, or from finite-dimensional Gaussian likelihood ratios. On $\mathbb R^2$, generalized noise can be realized on [tempered distributions](tempered-distribution.md); an unweighted global negative [Sobolev space](sobolev-space-split.md) is not automatically a suitable almost-sure support on an unbounded domain. The stochastic series avoids imposing that unsupported regularity.

## ↑ Ancestors (8)

1. [Gaussian white noise](gaussian-white-noise.md)
2. [Gaussian process](gaussian-process.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/3/b/solution.md)
