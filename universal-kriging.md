# Universal kriging

↑ **Parent:** [Kriging](kriging.md)

[Universal kriging](universal-kriging.md) allows an unknown [regression](regression-analysis.md) drift:

$$
\mathbb E[Z]=X\beta,\qquad \mathbb E[Z_0]=x_0^T\beta.
$$

The [design matrix](design-matrix.md) $X$ has full column rank, its entries and $x_0$ are known, and the [regression coefficients](regression-coefficient.md) $\beta$ are unknown. For example, rows $(1,s_i)$ and target row $(1,s_0)$ allow a linear spatial trend. Requiring $w^TZ$ to have zero [bias](bias-of-an-estimator.md) for every $\beta$ gives $X^Tw=x_0$. With known [positive-definite matrix](positive-definite-matrix.md) observation [covariance matrix](covariance-matrix.md) $\Sigma$, the minimizing weights solve

$$
\begin{pmatrix}\Sigma&X\\X^T&0\end{pmatrix}
\begin{pmatrix}w\\\eta\end{pmatrix}
=\begin{pmatrix}c\\x_0\end{pmatrix},
$$

where $\eta$ is a vector of [Lagrange multipliers](lagrange-multiplier.md). Equivalently, the [generalized least squares](generalized-least-squares.md) estimate and prediction are

$$
\widehat\beta=(X^T\Sigma^{-1}X)^{-1}X^T\Sigma^{-1}z,
\qquad
\widehat Z_0=x_0^T\widehat\beta+c^T\Sigma^{-1}(z-X\widehat\beta).
$$

The first term is the estimated trend alone; the second predicts the correlated [regression residuals](regression-residual.md). With $q=x_0-X^T\Sigma^{-1}c$, the error [variance](variance-split.md) is

$$
s_{\mathrm{UK}}^2=v_0-c^T\Sigma^{-1}c
+q^T(X^T\Sigma^{-1}X)^{-1}q.
$$

The last, nonnegative term accounts for estimating the specified drift coefficients. Merely inserting a fitted drift into [simple kriging](simple-kriging.md) and keeping its known-[mean](expected-value-split.md) error [variance](variance-split.md) would omit this term. For a [Gaussian random field](gaussian-random-field.md), the same expressions arise by integrating over drift coefficients in a diffuse [prior distribution](prior-probability.md) limit; this is an additional inferential interpretation, not an assumption required by the linear optimization.[§2.7, pp. 27–28, equations (2.38)–(2.42)](gaussian-processes-for-machine-learning-by-carl-edward-rasmussen-and-christopher-k-i-williams.md)

## ↑ Ancestors (8)

1. [Kriging](kriging.md)
2. [Geostatistics](geostatistics.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Best linear unbiased estimator](best-linear-unbiased-estimator.md)
- [Kriging](kriging.md)
- [Ordinary kriging](ordinary-kriging.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/6/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/6/e/solution.md)
- [Universal kriging](universal-kriging.md)
