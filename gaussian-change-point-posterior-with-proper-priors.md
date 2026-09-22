# Gaussian change-point posterior with proper priors

↑ **Parent:** [Change-point detection](change-point-detection.md)

Take independent proper normal [prior distributions](prior-probability.md) for the two segment means and a proper [inverse-gamma distribution](inverse-gamma-distribution.md) for the common [variance](variance-split.md). A uniform [prior distribution](prior-probability.md) over $m=1,\ldots,n$ may then retain the empty second segment. The [posterior distribution](bayesian-posterior.md) is proper: its [likelihood function](likelihood-function.md) is bounded above by $(2\pi)^{-n/2}v^{-n/2}$, whose integral against $\operatorname{IG}(a_0,b_0)$ is finite for $a_0,b_0>0$. At $m=n$ the second mean has its unchanged proper [prior distribution](prior-probability.md) as its [full conditional distribution](full-conditional-distribution.md). The configuration's [posterior probability](posterior-probability.md) now has the meaningful interpretation of no change inside the observed sample.

**Table of contents**

- [Gaussian change-point Gibbs updates](gaussian-change-point-gibbs-updates.md)

## ↑ Ancestors (5)

1. [Change-point detection](change-point-detection.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/5/solution.md)
