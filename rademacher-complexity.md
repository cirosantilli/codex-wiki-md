# Rademacher complexity

↑ **Parent:** [Statistical learning theory](statistical-learning-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rademacher_complexity)

For [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) $Z_1,\ldots,Z_n$ and independent [Rademacher signs](rademacher-distribution.md) $\varepsilon_1,\ldots,\varepsilon_n$, the Rademacher complexity of a [function class](function-class.md) $\mathcal F$ is

$$
\mathcal R_n(\mathcal F)
=\mathbb E_{Z,\varepsilon}\left[
\sup_{f\in\mathcal F}\frac1n\sum_{i=1}^n\varepsilon_i f(Z_i)
\right].
$$

It measures how strongly the class can correlate with independent random signs on a random sample.

**Table of contents**

- [Empirical Rademacher complexity](empirical-rademacher-complexity.md)
- [Rademacher symmetrization inequality](rademacher-symmetrization-inequality.md)
- [Rademacher excess-risk bound for empirical risk minimization](rademacher-excess-risk-bound-for-empirical-risk-minimization.md)
- [Massart finite-class lemma](massart-finite-class-lemma.md)
- [Rademacher bound for bounded weighted indicators](rademacher-bound-for-bounded-weighted-indicators.md)
- [Rademacher complexity of a convex hull](rademacher-complexity-of-a-convex-hull.md)
- [Rademacher contraction lemma](rademacher-contraction-lemma.md)
- [Frobenius norm Rademacher calculation](frobenius-norm-rademacher-calculation.md)
- [Rademacher complexity of quadratic forms](rademacher-complexity-of-quadratic-forms.md)
- [Expected excess-risk bound for empirical risk minimization](expected-excess-risk-bound-for-empirical-risk-minimization.md)

## ↑ Ancestors (5)

1. [Statistical learning theory](statistical-learning-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/31j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/30j/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/30j/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1/31k/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1/31l/a/solution.md)
