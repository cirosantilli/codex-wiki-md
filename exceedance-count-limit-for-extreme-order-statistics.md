# Exceedance count limit for extreme order statistics

↑ **Parent:** [Order statistic](order-statistic.md)

For [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md), suppose normalized [sample maxima](sample-maximum.md) have limiting [distribution function](cumulative-distribution-function.md) $G$. At a threshold $a_nx+b_n$ with $G(x)>0$, the exceedance count has limiting [Poisson distribution](poisson-distribution.md) with parameter $-\log G(x)$. The $r$th largest observation lies below the threshold exactly when at most $r-1$ observations strictly exceed it, including in samples with ties. Summing the first $r$ limiting Poisson probabilities gives the displayed limit for every fixed positive integer $r$. The equivalence follows from $F(a_nx+b_n)^n\to G(x)$ and $-\log(1-p)\sim p$ as $p\downarrow0$.

## ↑ Ancestors (6)

1. [Order statistic](order-statistic.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/3/solution.md)
