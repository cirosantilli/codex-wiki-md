# Mean bounds after deleting bounded observations

↑ **Parent:** [Complete-case analysis](complete-case-analysis.md)

Suppose $N>d\ge0$ observations lie in $[a,b]$ and have [sample mean](sample-mean.md) $\bar y$. Delete any $d$ observations. The remaining [sample mean](sample-mean.md) obeys

$$
\frac{N\bar y-db}{N-d}\le\bar y_{\mathrm{remaining}}\le\frac{N\bar y-da}{N-d}.
$$

Indeed, the removed sum is between $da$ and $db$; subtract it from the original sum $N\bar y$ and divide by the remaining positive count. If only a rounded mean in $[\ell,u]$ is known, a valid enclosing [interval](interval-mathematics.md) is $[(N\ell-db)/(N-d),(Nu-da)/(N-d)]$, optionally intersected with $[a,b]$. These deterministic bounds do not require [missing at random](missing-at-random.md). They constrain a complete-case summary without claiming that complete-case selection is unbiased for a [target population](target-population.md).

## ↑ Ancestors (6)

1. [Complete-case analysis](complete-case-analysis.md)
2. [Missing data](missing-data.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2020/6/solution.md)
