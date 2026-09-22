# Rademacher symmetrization inequality

↑ **Parent:** [Rademacher complexity](rademacher-complexity.md)

For an [i.i.d. sample](independent-and-identically-distributed-random-variables.md) and an integrable [function class](function-class.md) $\mathcal F$,

$$
\mathbb E\sup_{f\in\mathcal F}
\frac1n\sum_{i=1}^n\bigl(f(Z_i)-\mathbb Ef(Z_i)\bigr)
\leq2\mathcal R_n(\mathcal F).
$$

Introduce an independent ghost sample, replace each expectation by its ghost-sample average using [Jensen inequality](jensen-s-inequality.md), and then multiply each paired difference by an independent [Rademacher sign](rademacher-distribution.md). Splitting the resulting supremum into its two sample contributions gives the factor two.

## ↑ Ancestors (6)

1. [Rademacher complexity](rademacher-complexity.md)
2. [Statistical learning theory](statistical-learning-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/31j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/31j/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/31j/c/solution.md)
- [Rademacher excess-risk bound for empirical risk minimization](rademacher-excess-risk-bound-for-empirical-risk-minimization.md)
