# Missingness overlap from marginal and complete-case counts

↑ **Parent:** [Missing data](missing-data.md)

For $N$ observations, let $m_X$ and $m_Y$ count missing values of two [variables](variable-mathematics.md), and let $n_{XY}$ count observations on which both are available. The number missing at least one variable is $N-n_{XY}$. Applying the [inclusion-exclusion principle](inclusion-exclusion-principle.md) to the two missing-value [sets](set-split.md) gives the displayed number missing both. The disjoint counts are consequently $m_X-m_{XY}$ missing only $X$, $m_Y-m_{XY}$ missing only $Y$, $m_{XY}$ missing both, and $n_{XY}$ complete cases. Their nonnegativity is a necessary consistency check on the supplied totals.

This identifies an aggregate missingness pattern without reconstructing individual records. It does not identify a [missing-data mechanism](missing-data-mechanism.md), establish [missing completely at random](missing-completely-at-random.md), or justify treating a substantive response such as an explicit unknown category as a missing observation. Counts from different cohorts cannot be inserted into the identity without first establishing a common denominator.

## ↑ Ancestors (5)

1. [Missing data](missing-data.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-digital-social-research-statistics-core-course-of-the-university-of-oxford/2018/2/solution.md)
