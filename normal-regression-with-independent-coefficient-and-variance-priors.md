# Normal regression with independent coefficient and variance priors

↑ **Parent:** [Gaussian conjugacy for a normal linear model](gaussian-conjugacy-for-a-normal-linear-model.md)

In a [normal linear model](normal-linear-model-split.md) $Y\mid b,s\sim N(Xb,sI)$, assign the coefficient [vector](vector.md) $b$ a proper [normal distribution](normal-distribution.md) with fixed positive-definite [covariance matrix](covariance-matrix.md) $D$, independently of the [variance](variance-split.md) $s$, whose [prior distribution](prior-probability.md) is [inverse-gamma distribution](inverse-gamma-distribution.md). [Completing the square](completing-the-square.md) gives

$$
V(s)=(D^{-1}+X^TX/s)^{-1},\qquad
m(s)=V(s)(D^{-1}b_0+X^Ty/s),\qquad
b\mid s,y\sim N(m(s),V(s)).
$$

Multiplying the residual [likelihood function](likelihood-function.md) by the [inverse-gamma distribution](inverse-gamma-distribution.md) density also gives

$$
s\mid b,y\sim\operatorname{InvGamma}\left(a_0+n/2,c_0+\lVert y-Xb\rVert^2/2\right).
$$

These [full conditional distributions](full-conditional-distribution.md) permit a [Gibbs sampler](gibbs-sampler.md). The marginal coefficient [posterior distribution](bayesian-posterior.md) is obtained by [marginalization](marginalization.md) over $s$. Its conditional [mean](expected-value-split.md) and [covariance matrix](covariance-matrix.md) both depend on $s$, so it is generally not a [Student's t-distribution](student-s-t-distribution.md). Even if the columns of $X$ and the prior coordinates make the conditional coefficient components independent, averaging over a shared unknown $s$ need not preserve that [independence](independent-random-variables.md).

A [normal-inverse-gamma prior](normal-inverse-gamma-prior.md) instead scales the conditional coefficient prior [covariance matrix](covariance-matrix.md) by $s$, producing a multivariate [Student's t-distribution](student-s-t-distribution.md) on [marginalization](marginalization.md). It is a different joint [prior distribution](prior-probability.md).

## ↑ Ancestors (8)

1. [Gaussian conjugacy for a normal linear model](gaussian-conjugacy-for-a-normal-linear-model.md)
2. [Normal linear model](normal-linear-model-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2021/3/c/solution.md)
