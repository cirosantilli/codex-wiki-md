# Poissonized coupon completion time and count

↑ **Parent:** [Coupon collector problem](coupon-collector-problem.md)

For independent coupon labels arriving at rate $\lambda$, [Poisson thinning](poisson-thinning.md) makes the type-specific first arrival times independent exponentials of rates $\lambda p_j$. Completion time is their maximum. Its distribution is $\mathbb P(T<t)=\prod_j(1-e^{-\lambda p_jt})$. The completion count $L$ depends only on the labels and is independent of the exponential interarrival sequence. Therefore $T=\sum_{k\ge1}E_k\mathbf1_{\{L\ge k\}}$ and nonnegative integration gives the displayed identity. Completion count and its expectation do not depend on arrival rate.

## ↑ Ancestors (9)

1. [Coupon collector problem](coupon-collector-problem.md)
2. [Geometric distribution](geometric-distribution.md)
3. [Discrete probability distribution](discrete-probability-distribution-split.md)
4. [Probability distribution](probability-distribution.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/26j/b/solution.md)
