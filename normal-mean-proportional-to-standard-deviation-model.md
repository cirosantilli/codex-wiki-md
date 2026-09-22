# Normal mean proportional to standard deviation model

↑ **Parent:** [Curved exponential family](curved-exponential-family.md)

This one-parameter [normal distribution](normal-distribution.md) model has positive [mean](expected-value-split.md) equal to its [standard deviation](standard-deviation.md). It is a [curved exponential family](curved-exponential-family.md): both the linear and quadratic natural parameters depend on the same scalar [statistical parameter](statistical-parameter.md). It combines information about the center and spread, so the [sample mean](sample-mean.md) alone does not use all available [Fisher information](fisher-information-matrix.md).

For a [statistical sample](statistical-sample.md) of size $n$, let $A=\sum_ix_i$ and $B=\sum_ix_i^2$. Up to an additive constant the [log-likelihood function](log-likelihood.md) is $\ell(\mu)=-n\log\mu-B/(2\mu^2)+A/\mu$. Its [score function](informant-function.md) is $(B-A\mu-n\mu^2)/\mu^3$. When $B>0$, the numerator changes from positive to negative at its unique positive root, so the global [maximum-likelihood estimator](maximum-likelihood-estimator.md) is

$$
\widehat\mu=\frac{-A+\sqrt{A^2+4nB}}{2n}.
$$

The all-zero observation vector has zero [probability](probability.md) and is an exceptional case with an unbounded [likelihood function](likelihood-function.md) near zero. Since $\mathbb E A=n\mu$ and $\mathbb E B=2n\mu^2$, the expected [Fisher information](fisher-information-matrix.md) is $I_n(\mu)=3n/\mu^2$. Thus regular [asymptotic normality of a maximum likelihood estimator](asymptotic-normality-of-a-maximum-likelihood-estimator.md) gives $\sqrt n(\widehat\mu-\mu)\xrightarrow dN(0,\mu^2/3)$. The [optimal asymptotic combination of a normal sample mean and standard deviation](optimal-asymptotic-combination-of-a-normal-sample-mean-and-standard-deviation.md) attains the same first-order precision.

## ↑ Ancestors (8)

1. [Curved exponential family](curved-exponential-family.md)
2. [Exponential family](exponential-family-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Optimal asymptotic combination of a normal sample mean and standard deviation](optimal-asymptotic-combination-of-a-normal-sample-mean-and-standard-deviation.md)
- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2017/1/b/i/solution.md)
