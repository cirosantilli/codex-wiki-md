# Chernoff information

↑ **Parent:** [Binary hypothesis testing in information theory](binary-hypothesis-testing-in-information-theory.md)

[Chernoff information](chernoff-information.md) measures how quickly repeated independent evidence can distinguish two fixed [probability distributions](probability-distribution.md). Suppose a [statistical hypothesis test](statistical-hypothesis-test.md) observes $n$ [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md), with common law $P$ under one [simple hypothesis](simple-hypothesis.md) and $Q$ under the other. Give the two hypotheses fixed positive [prior probabilities](prior-probability.md), and let $p_n^*$ be the smallest achievable average error probability. For distinct positive [probability mass functions](probability-mass-function.md) on a common [finite alphabet](finite-alphabet.md),

$$
\lim_{n\to\infty}-\frac1n\ln p_n^*=C(P,Q),\qquad
C(P,Q)=-\min_{0\leq s\leq1}\ln\sum_xP(x)^sQ(x)^{1-s}.
$$

Here $\ln$ is the [natural logarithm](natural-logarithm.md), so the [error exponent](error-exponents-in-hypothesis-testing.md) is measured in [nats](nat-unit.md) per observation. This optimal rate is unchanged by choosing different fixed positive [prior probabilities](prior-probability.md); the best decision rule and finite-sample error can still change.[§16.1, Corollary 16.2 and equation (16.2), printed pp. 261–262: fixed-prior Bayesian error exponent](information-theory-from-coding-to-learning-october-2022-draft-by-yury-polyanskiy-and-others.md)

The interpretation is $p_n^*=\exp(-nC(P,Q)+o(n))$: a larger [Chernoff information](chernoff-information.md) means fewer observations are needed at the leading exponential scale. It does not assert the exact finite-sample identity $p_n^*=e^{-nC(P,Q)}$. The [finite-sample Chernoff error bound](finite-sample-chernoff-error-bound.md) and the explicit [Chernoff information for complementary Bernoulli distributions](chernoff-information-for-complementary-bernoulli-distributions.md) make this distinction concrete. This is useful when designing repeated measurements or comparing sensors whose output [probability distributions](probability-distribution.md) differ under two candidate conditions.

For [probability mass functions](probability-mass-function.md) with zero entries, define the affinity for $0<s<1$ and use $C(P,Q)=-\ln\inf_{0<s<1}\sum_xP(x)^sQ(x)^{1-s}$, taking endpoint limits when needed. This avoids an ambiguous $0^0$ convention. Identical laws give $C=0$; disjoint [probability supports](support-of-a-probability-distribution.md) give $C=\infty$, because one observation separates them perfectly. The displayed finite-rate theorem concerns fixed laws with common positive support, not laws that change with $n$ or arbitrarily dependent repeated observations.

**Table of contents**

- [Chernoff affinity](chernoff-affinity.md)
- [Finite-sample Chernoff error bound](finite-sample-chernoff-error-bound.md)
- [Chernoff information for complementary Bernoulli distributions](chernoff-information-for-complementary-bernoulli-distributions.md)
- [Historical source for Chernoff information](historical-source-for-chernoff-information.md)

## ↑ Ancestors (6)

1. [Binary hypothesis testing in information theory](binary-hypothesis-testing-in-information-theory.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Chernoff affinity](chernoff-affinity.md)
- [Chernoff information](chernoff-information.md)
- [Chernoff information for complementary Bernoulli distributions](chernoff-information-for-complementary-bernoulli-distributions.md)
- [Error exponents in hypothesis testing](error-exponents-in-hypothesis-testing.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-224/2/b/solution.md)
