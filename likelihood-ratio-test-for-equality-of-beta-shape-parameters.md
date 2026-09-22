# Likelihood-ratio test for equality of beta shape parameters

↑ **Parent:** [Likelihood-ratio test](likelihood-ratio-test.md)

Take two independent [statistical samples](statistical-sample.md) from [beta distributions](beta-distribution.md) with parameters $(\theta,1)$ and $(\tau,1)$, of positive sizes $n,m$. Put $A=-\sum_i\log X_i$, $B=-\sum_j\log Y_j$, and $T=A/(A+B)$. To test the [null hypothesis](null-hypothesis.md) $\theta=\tau$, divide the maximized common-rate [likelihood function](likelihood-function.md) by the unrestricted maximum to obtain the displayed [likelihood ratio](likelihood-ratio.md). Indeed the unrestricted fitted rates are $n/A,m/B$, and the common fitted rate is $(n+m)/(A+B)$; substitution cancels the exponential factors.

Under the [null hypothesis](null-hypothesis.md), $A$ and $B$ have independent [gamma distributions](gamma-distribution.md) with a common rate. [Beta-gamma independence](beta-gamma-independence.md) gives $T\sim\operatorname{Beta}(n,m)$. The [derivative](derivative.md) of $\log(T^n(1-T)^m)$ changes sign at $n/(n+m)$, so the exact [critical region](rejection-region.md) of size $\alpha$ is $T<k_1$ or $T>k_2$, with $k_1<n/(n+m)<k_2$. Its cutoffs satisfy

$$
k_1^n(1-k_1)^m=k_2^n(1-k_2)^m,\qquad
F_{n,m}(k_1)+1-F_{n,m}(k_2)=\alpha.
$$

Here $F_{n,m}$ is the [beta distribution](beta-distribution.md) [cumulative distribution function](cumulative-distribution-function.md). Equal [likelihood ratios](likelihood-ratio.md) at the cutoffs do not generally mean equal tail probabilities. Increasing the ratio threshold continuously adds positive [null distribution](null-distribution.md) mass on both sides, proving uniqueness for $0<\alpha<1$.

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

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2021/1/b/i/solution.md)
