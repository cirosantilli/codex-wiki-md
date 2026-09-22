# Kriging

↑ **Parent:** [Geostatistics](geostatistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kriging)

[Kriging](kriging.md) predicts an unobserved value of a spatial [random field](random-field.md) by combining observations according to their [covariances](covariance.md). [Nearest-neighbor interpolation](nearest-neighbor-interpolation.md) uses the closest sample; [kriging](kriging.md) also asks how strongly each sample is related to the target and how much information the samples share with one another. Two nearby, highly correlated samples need not provide twice the information of one. The different forms of [kriging](kriging.md) depend on whether the [mean](expected-value-split.md) is known, an unknown constant, or an unknown [regression](regression-analysis.md) drift.

Write $Z=(Z(s_1),\ldots,Z(s_n))^T$ for the observation [random vector](random-vector.md), $z$ for its realized values, and $Z_0=Z(s_0)$ for the prediction target. Assume finite [second moments](second-moment.md), and define

$$
\Sigma_{ij}=\operatorname{Cov}(Z(s_i),Z(s_j)),\qquad
c_i=\operatorname{Cov}(Z(s_i),Z_0),\qquad
v_0=\operatorname{Var}(Z_0).
$$

Here $\Sigma$ is the observation [covariance matrix](covariance-matrix.md), assumed to be a [positive-definite matrix](positive-definite-matrix.md) in the formulas below. A [covariance function](covariance-function.md) supplies its entries and the target [covariance](covariance.md) vector $c$. For a second-order stationary [random field](random-field.md), the [covariogram](covariogram.md) $C(h)$ depends on displacement, and the [semivariogram](semivariogram.md) satisfies $\gamma(h)=C(0)-C(h)$. The [intrinsically stationary random field](intrinsically-stationary-random-field.md) formulation permits [kriging](kriging.md) using a [semivariogram](semivariogram.md) even when a stationary [covariogram](covariogram.md) is unavailable; the finite [covariance](covariance.md) formulation below is a convenient important case.

For a [linear combination](linear-combination.md) $w^TZ$ predicting $Z_0$ with zero [bias](bias-of-an-estimator.md), the error [variance](variance-split.md) equals its [mean squared error](mean-squared-error.md):

$$
Q(w)=\mathbb E[(w^TZ-Z_0)^2]
=v_0-2w^Tc+w^T\Sigma w.
$$

[Ordinary kriging](ordinary-kriging.md) and [universal kriging](universal-kriging.md) minimize this [quadratic form](quadratic-form-split.md) subject to their [mean](expected-value-split.md) constraints. Their optimality is among the specified linear predictors with zero [bias](bias-of-an-estimator.md) under the chosen [statistical model](statistical-model-split.md); [covariance](covariance.md) information alone does not establish optimality among arbitrary nonlinear predictors. The [Gaussian random field](gaussian-random-field.md) interpretation supplies additional conclusions in [simple kriging](simple-kriging.md).

The reported error [variance](variance-split.md) assumes a chosen [covariance function](covariance-function.md), its [statistical parameters](statistical-parameter.md), observation locations, and a [mean](expected-value-split.md) structure. It omits uncertainty in fitted [covariance](covariance.md) parameters and does not validate the trend. A repeated-sampling [mean squared error](mean-squared-error.md) need not equal the error [variance](variance-split.md) conditional on each realized data vector.[chapter 2, equations (2.23)–(2.24), and §2.3 on covariance parameters](gaussian-processes-for-machine-learning-by-carl-edward-rasmussen-and-christopher-k-i-williams.md)

In 1963, [Georges Matheron](georges-matheron.md) presented [kriging](kriging.md) for estimating average ore grades in mining panels from weighted samples taken inside and outside a panel. This setting in [geostatistics](geostatistics.md) explains why prediction targets can be averages over regions as well as values at points.[Matheron, Principles of geostatistics, 1963, p. 1246 introduction and pp. 1259–1261, Kriging](principles-of-geostatistics-by-georges-matheron.md)

**Table of contents**

- [Universal kriging](universal-kriging.md)
- [Ordinary kriging](ordinary-kriging.md)
- [Simple kriging](simple-kriging.md)

## ↑ Ancestors (7)

1. [Geostatistics](geostatistics.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Geostatistics](geostatistics.md)
- [Kriging](kriging.md)
- [Ordinary kriging](ordinary-kriging.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/6/d/solution.md)
- [Simple kriging](simple-kriging.md)
