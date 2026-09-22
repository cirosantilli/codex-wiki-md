# Fixed-mean normal variance test

↑ **Parent:** [Neyman-Pearson lemma](neyman-pearson-lemma.md)

For independent $N(0,\sigma^2)$ observations, testing a fixed variance against larger variances uses the sum of squares $S=\sum_iX_i^2$. The [likelihood ratio](likelihood-ratio.md) for any simple larger variance is strictly increasing in $S$. The [Neyman-Pearson lemma](neyman-pearson-lemma.md) therefore gives the displayed rejection rule, where $F_n$ is the [chi-squared distribution](chi-squared-distribution.md) function with $n$ degrees of freedom. Its threshold is independent of the selected larger variance, so it is a [uniformly most powerful test](uniformly-most-powerful-test.md) for the one-sided composite alternative. Its [power function](power-function-of-a-statistical-test.md) is $1-F_n((\sigma_0^2/\sigma^2)F_n^{-1}(1-\alpha))$, increasing continuously from zero to one and equaling $\alpha$ at the null. A known nonzero mean is handled by replacing each observation by its difference from that mean.

## ↑ Ancestors (8)

1. [Neyman-Pearson lemma](neyman-pearson-lemma.md)
2. [Statistical hypothesis test](statistical-hypothesis-test-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2013/o4/c/solution.md)
