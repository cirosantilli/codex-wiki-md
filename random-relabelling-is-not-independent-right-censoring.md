# Random relabelling is not independent right censoring

↑ **Parent:** [Independent censoring](independent-censoring.md)

Suppose the recorded durations retain an [exponential distribution](exponential-distribution.md) of rate $\theta$, but an independent fraction $q$ are relabelled as failures and the rest as [right-censored](right-censoring.md). Applying the ordinary [survival likelihood](survival-likelihood.md) gives $\widehat\theta=d/\sum_i y_i\to q\theta$, rather than $\theta$. A censoring flag chosen independently of the recorded duration does not establish [independent censoring](independent-censoring.md) of a latent failure time. Genuine simulation instead draws an event time and an independent censoring time and records their minimum.

## ↑ Ancestors (7)

1. [Independent censoring](independent-censoring.md)
2. [Censoring (statistics)](censoring-statistics.md)
3. [Survival analysis](survival-analysis-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-37/1/solution.md)
