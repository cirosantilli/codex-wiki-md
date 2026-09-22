# Weighted central limit theorem with negligible maximum weight

↑ **Parent:** [Central limit theorem](central-limit-theorem.md)

Let $X_k$ be [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with [expected value](expected-value-split.md) zero, [variance](variance-split.md) one, and a [moment-generating function](moment-generating-function.md) finite in a neighborhood of zero. Each row of deterministic real weights $a_{n,k}$ is finite. If $\max_k|a_{n,k}|\to0$ and $\sum_ka_{n,k}^2\to v<\infty$, then the weighted sums converge in [distribution](distribution-mathematical-analysis.md) to a [normal distribution](normal-distribution.md) with mean zero and variance $v$; $v=0$ denotes the constant zero.

By the [quadratic expansion of a cumulant-generating function](quadratic-expansion-of-a-cumulant-generating-function.md), write $K(u)=u^2/2+r(u)$ with $r(u)=o(u^2)$. For a fixed real $t$, put $\eta_n=\sup_{0<|u|\leq |t|\max_k|a_{n,k}|}|r(u)|/u^2$, with the supremum taken as zero if its range is empty. Then $\eta_n\to0$ and

$$
\left|\sum_kr(ta_{n,k})\right|\leq\eta_nt^2\sum_ka_{n,k}^2\longrightarrow0.
$$

Thus the log [moment-generating function](moment-generating-function.md) of the sum tends to $vt^2/2$. The [convergence theorem for moment-generating functions](convergence-theorem-for-moment-generating-functions.md) proves the conclusion. The supremum is the step that makes the remainder estimate uniform across the row; a separate little-o assertion for each term would not justify summing an increasing number of terms.

## ↑ Ancestors (7)

1. [Central limit theorem](central-limit-theorem.md)
2. [Convergence of random variables](convergence-of-random-variables-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2017/2/b/iii/solution.md)
