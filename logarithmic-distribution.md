# Logarithmic distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution-split.md)

For $0<\theta<1$, this [probability distribution](probability-distribution-split.md) on positive integers has mass $\mathbb P(X=k)=\theta^k/(k[-\log(1-\theta)])$. The Taylor identity $\sum_{k\geq1}\theta^k/k=-\log(1-\theta)$ proves normalization. Its [expectation](expected-value-split.md) is $-\theta/((1-\theta)\log(1-\theta))$, by summing the [geometric series](geometric-series.md) after multiplying the mass by $k$.

For an independent sample, the [maximum-likelihood estimator](maximum-likelihood-estimator.md) solves the equation making this model mean equal to the [sample mean](sample-mean.md). The model mean is strictly increasing: set $t=-\log(1-\theta)$ to obtain $(e^t-1)/t$, whose derivative is positive for $t>0$. Hence a sample mean greater than one determines a unique interior estimate. Pooling several categories changes the likelihood and generally changes this estimate; the ungrouped sample mean is no longer recoverable from the pooled category counts alone.

## ↑ Ancestors (7)

1. [Discrete probability distribution](discrete-probability-distribution-split.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [O5](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2009/o/o5.md)
