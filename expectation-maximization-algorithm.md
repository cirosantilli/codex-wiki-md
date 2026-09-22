# Expectation-maximization algorithm

↑ **Parent:** [Latent variable](latent-variable-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Expectation-maximization_algorithm)

The [expectation-maximization algorithm](expectation-maximization-algorithm.md) fits a [latent-variable model](latent-variable-model.md) by alternating a [conditional expectation](conditional-expectation.md) over the [latent variables](latent-variable-split.md) with a maximization over the [statistical parameters](statistical-parameter.md). Its target is the observed-data [likelihood function](likelihood-function.md), although its updates use the simpler complete-data [log-likelihood](log-likelihood.md).[Section 2, printed p. 6, equation (2.17) and the general E-step/M-step definition](maximum-likelihood-from-incomplete-data-via-the-em-algorithm-by-arthur-pentland-dempster-and-others.md)

Write $y$ for the observations, $z$ for the [latent variables](latent-variable-split.md), and $p_\theta(y,z)$ for their joint [probability density function](probability-density-function.md) or [probability mass function](probability-mass-function.md). The observed-data [log-likelihood](log-likelihood.md) is

$$
\ell(\theta)=\log p_\theta(y),\qquad p_\theta(y)=\int p_\theta(y,z)\,dz,
$$

where the [integral](integral-split.md) becomes a sum for discrete $z$. Directly maximizing a [logarithm](logarithm.md) of this sum can be awkward. The [E-step](em-expectation-step.md) instead computes a [conditional distribution](conditional-distribution.md) at the current [statistical parameters](statistical-parameter.md) $\theta^{(t)}$; the [M-step](em-maximization-step.md) uses it to construct a new fit. The attractive idea is to retain uncertainty about the hidden labels while recovering simple [weighted means](weighted-arithmetic-mean.md) and other complete-data updates. The [Known-variance Gaussian mixture EM example](known-variance-gaussian-mixture-em-example.md) shows the mechanism without estimating a [variance](variance-split.md) or [mixture weight](mixture-weight.md).

[Arthur Pentland Dempster](arthur-pentland-dempster.md), [Nan M. Laird](nan-m-laird.md), and [Donald B. Rubin](donald-b-rubin.md) gave the general framework its name in their 1977 paper, which also discusses earlier special-case algorithms.[Section 1, printed pp. 1 and 3: naming of the two steps and earlier special cases](maximum-likelihood-from-incomplete-data-via-the-em-algorithm-by-arthur-pentland-dempster-and-others.md)

**Table of contents**

- [EM expectation step](em-expectation-step.md)
- [EM maximization step](em-maximization-step.md)
- [Known-variance Gaussian mixture EM example](known-variance-gaussian-mixture-em-example.md)
  - [Identical-mean EM trap](identical-mean-em-trap.md)
- [Ordered-rate exponential M-step](ordered-rate-exponential-m-step.md)
- [EM for merged multinomial cells](em-for-merged-multinomial-cells.md)
- [EM for an independent missing normal coordinate](em-for-an-independent-missing-normal-coordinate.md)
- [EM transition-count update on a tree](em-transition-count-update-on-a-tree.md)
- [EM for a missing observation in a Gaussian AR1 process](em-for-a-missing-observation-in-a-gaussian-ar1-process.md)
- [EM likelihood monotonicity](em-likelihood-monotonicity.md)

## ↑ Ancestors (7)

1. [Latent variable](latent-variable-split.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (38)

- [Conditional cure-weight equations for paired Poisson counts](conditional-cure-weight-equations-for-paired-poisson-counts.md)
- [EM algorithm for a censored lognormal competing-risks mixture](em-algorithm-for-a-censored-lognormal-competing-risks-mixture.md)
- [EM algorithm for zero-inflated Poisson regression](em-algorithm-for-zero-inflated-poisson-regression.md)
- [EM for a missing observation in a Gaussian AR1 process](em-for-a-missing-observation-in-a-gaussian-ar1-process.md)
- [EM for an independent missing normal coordinate](em-for-an-independent-missing-normal-coordinate.md)
- [EM for merged multinomial cells](em-for-merged-multinomial-cells.md)
- [EM for zero-inflated negative binomial regression](em-for-zero-inflated-negative-binomial-regression.md)
- [EM likelihood monotonicity](em-likelihood-monotonicity.md)
- [EM transition-count update on a tree](em-transition-count-update-on-a-tree.md)
- [EM update for a single-factor Gaussian model](em-update-for-a-single-factor-gaussian-model.md)
- [Expectation-maximization algorithm](expectation-maximization-algorithm.md)
- [Felsenstein pruning algorithm](felsenstein-pruning-algorithm.md)
- [Known-variance Gaussian mixture EM example](known-variance-gaussian-mixture-em-example.md)
- [Mixture responsibility](mixture-responsibility.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/4/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/6/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/6/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/6/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/1/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-216/4/a/solution.md)
- [Responsibility curve for a two-Gaussian mixture](responsibility-curve-for-a-two-gaussian-mixture.md)
