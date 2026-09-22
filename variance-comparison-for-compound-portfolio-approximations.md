# Variance comparison for compound portfolio approximations

↑ **Parent:** [Heterogeneous individual claims model](heterogeneous-individual-claims-model.md)

Put $Q=\sum_iq_i$, $M=\sum_iq_i\mu_i$, and $A=\sum_iq_i\mathbb EY_i^2$. A [compound Poisson distribution](compound-poisson-distribution.md) with count mean $Q$ and severity law $\sum_i(q_i/Q)F_i$ has [variance](variance-split.md) $V_{\mathrm P}=A$. A [compound binomial distribution](compound-binomial-distribution.md) with $n$ trials, probability $Q/n$, and that same severity law has [variance](variance-split.md) $V_{\mathrm B}=A-M^2/n$. The individual-policy variance is $V=A-\sum_i(q_i\mu_i)^2$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $\sum_i(q_i\mu_i)^2\geq M^2/n$, proving the ordering. Equality of the first two variances requires constant $q_i\mu_i$; it need not imply equality of the distributions. If all probabilities and severity laws are identical, the binomial compound approximation is exactly the individual model.

## ↑ Ancestors (7)

1. [Heterogeneous individual claims model](heterogeneous-individual-claims-model.md)
2. [Aggregate claims model](aggregate-claims-model.md)
3. [Actuarial statistics](actuarial-statistics-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-45/1/solution.md)
