# Best affine state estimate

↑ **Parent:** [State estimation](state-estimation.md)

A [best affine state estimate](best-affine-state-estimate.md) minimizes [mean squared error](mean-squared-error.md) among estimates $a+Cy$ formed from the available observation [vector](vector.md) $y$. With finite second moments and invertible observation [covariance matrix](covariance-matrix.md), it is

$$
\widehat x=\mathbb E[x]+\operatorname{Cov}(x,y)\operatorname{Cov}(y)^{-1}(y-\mathbb E[y]).
$$

This follows from the [orthogonal projection](orthogonal-projection.md) of centered state components onto the [linear span](linear-span.md) of centered observation components. For [Jointly Gaussian](multivariate-normal-distribution.md) state and observation it equals the [conditional expectation](conditional-expectation.md); for general laws a nonlinear estimate can have lower [mean squared error](mean-squared-error.md).

## ↑ Ancestors (5)

1. [State estimation](state-estimation.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Best affine state estimate](best-affine-state-estimate.md)
- [Kalman filter](kalman-filter.md)
- [Scalar Gaussian Kalman recursion](scalar-gaussian-kalman-recursion.md)
