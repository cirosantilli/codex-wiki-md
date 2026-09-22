# Likelihood-ratio test for equality of exponential means

↑ **Parent:** [Likelihood-ratio test](likelihood-ratio-test.md)

For two [independent](independent-random-variables.md) [statistical samples](statistical-sample.md) from [exponential distributions](exponential-distribution.md) with positive [means](expected-value-split.md) $\theta$ and $\mu$, write $A=\sum_{i=1}^nX_i$, $B=\sum_{j=1}^mY_j$ and $T=A/(A+B)$. The unconstrained [maximum-likelihood estimators](maximum-likelihood-estimator.md) are $A/n$ and $B/m$; under equality of the [means](expected-value-split.md) the common fitted [mean](expected-value-split.md) is $(A+B)/(n+m)$. Dividing the constrained maximum [likelihood function](likelihood-function.md) by its unrestricted maximum gives the displayed [likelihood ratio](likelihood-ratio.md). Its maximum is one at $T=n/(n+m)$, so the [likelihood-ratio test](likelihood-ratio-test.md) rejects for sufficiently small values, in either tail of $T$.

Under the [null hypothesis](null-hypothesis.md), the sums have independent [gamma distributions](gamma-distribution.md) with a common rate, so $T\sim\operatorname{Beta}(n,m)$ by [beta sampling by gamma ratios](beta-sampling-by-gamma-ratios.md). This permits exact calibration. For large samples with $n/(n+m)\to\rho\in(0,1)$, the [Wilks theorem](wilks-theorem.md) gives $-2\log\Lambda\xrightarrow d\chi^2_1$. Its upper-tail [probability](probability.md) is the asymptotic [p-value](p-value.md). The one [statistical degree of freedom](statistical-degrees-of-freedom.md) is the difference between the unrestricted and constrained parameter dimensions.

## ↑ Ancestors (8)

1. [Likelihood-ratio test](likelihood-ratio-test.md)
2. [Statistical hypothesis test](statistical-hypothesis-test-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2017/2/c/i/solution.md)
