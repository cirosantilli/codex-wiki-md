# Lincoln-Petersen estimator

↑ **Parent:** [Closed-population capture-recapture model](closed-population-capture-recapture-model.md)

The [Lincoln-Petersen estimator](lincoln-petersen-estimator.md) is the [ratio estimator](ratio-estimator.md) obtained by matching the observed overlap to its [hypergeometric](hypergeometric-distribution.md) [expected value](expected-value-split.md). It is defined when $R>0$. To distinguish that ratio from the exact [integer](integer-split.md) maximization, consecutive positive [likelihoods](likelihood-function.md) satisfy

$$
\frac{L(N+1)}{L(N)}
=\frac{(N+1-M)(N+1-C)}{(N+1)(N+1-M-C+R)}.
$$

This comparison is valid for $N\geq M+C-R$. For the toy counts, the numerator minus the denominator is $500-5(N+1)$. Thus the [likelihood function](likelihood-function.md) increases up to ninety-nine, ties at ninety-nine and one hundred, then decreases for every larger [integer](integer-split.md). This independently establishes the global [maximum-likelihood estimates](maximum-likelihood-estimator.md), beyond the plotting window. The adjacent-ratio method is given in [Guiteras, §8](https://web.mit.edu/14.380/www/handouts/hypergeometric.pdf).

## ↑ Ancestors (9)

1. [Closed-population capture-recapture model](closed-population-capture-recapture-model.md)
2. [Capture-recapture model](capture-recapture-model.md)
3. [Mark and recapture](mark-and-recapture.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Capture-recapture model](capture-recapture-model.md)
- [Chapman estimator](chapman-estimator.md)
- [Closed-population capture-recapture model](closed-population-capture-recapture-model.md)
- [Lincoln-Petersen estimator](lincoln-petersen-estimator.md)
- [Mark and recapture](mark-and-recapture.md)
