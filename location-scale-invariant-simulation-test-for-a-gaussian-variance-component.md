# Location-scale invariant simulation test for a Gaussian variance component

↑ **Parent:** [Variance-component likelihood-ratio test at a boundary](variance-component-likelihood-ratio-test-at-a-boundary.md)

With fixed $X,Z$, compare $N(X\beta,\sigma^2I)$ and $N(X\beta,\sigma^2I+\tau^2ZZ^T)$ by maximizing the ordinary [likelihood function](likelihood-function.md) in both models. Their [likelihood-ratio test statistic](likelihood-ratio-test-statistic.md) is unchanged by $Y\mapsto Xb+cY$, $c>0$, because both maximized log-likelihoods change by the same $-n\log c$. Its null law can therefore be simulated using independent $N(0,I)$ responses. Comparing the observed statistic with simulated statistics by $(1+\#\{T_b\geq T_{obs}\})/(B+1)$ gives a conservative finite-sample Monte Carlo p-value, subject to correctly maximizing both likelihoods.

## ↑ Ancestors (9)

1. [Variance-component likelihood-ratio test at a boundary](variance-component-likelihood-ratio-test-at-a-boundary.md)
2. [Likelihood-ratio test](likelihood-ratio-test.md)
3. [Statistical hypothesis test](statistical-hypothesis-test.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/1/d/solution.md)
