# Likelihood-ratio test for a normal variance

↑ **Parent:** [Likelihood-ratio test](likelihood-ratio-test.md)

For an independent [normal distribution](normal-distribution.md) sample with unknown mean, test $\sigma^2=\sigma_0^2$ against unrestricted positive variance. Put $q=\sum_i(x_i-\bar x)^2/\sigma_0^2$ and assume $n\geq2$. Profiling the mean and variance gives the [likelihood ratio](likelihood-ratio.md) $\lambda(q)=(q/n)^{n/2}e^{(n-q)/2}$ for a nondegenerate sample. Its logarithmic derivative $\tfrac12(n/q-1)$ changes sign at $n$, so small ratios select a lower and an upper tail.

Under the [null hypothesis](null-hypothesis.md), [Cochran's theorem](cochran-s-theorem.md) gives $Q\sim\chi_{n-1}^2$. The exact size-$\alpha$ cutoffs $0<q_1<n<q_2$ therefore satisfy

$$
F_{n-1}(q_1)+1-F_{n-1}(q_2)=\alpha,\qquad n\log(q_2/q_1)=q_2-q_1.
$$

The second equation makes the two boundary ratios equal. Rejection on $q\leq q_1$ or $q\geq q_2$ is consequently the exact [likelihood-ratio test](likelihood-ratio-test.md), and its tails need not have equal probability. For a large sample, the [Wilks theorem](wilks-theorem.md) instead calibrates $W=-2\log\lambda$ by $\chi_1^2$. A [Bartlett correction for a normal variance with unknown mean](bartlett-correction-for-a-normal-variance-with-unknown-mean.md) improves this asymptotic calibration; it is unnecessary when using the exact $Q$ distribution.

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

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2023/1/c/i/solution.md)
