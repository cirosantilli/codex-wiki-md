<h1 id="grouped-nelson-aalen-event-count-identity">Grouped Nelson–Aalen event-count identity</h1>

↑ **Parent:** [Event-count identity for Nelson–Aalen cumulative hazards](event-count-identity-for-nelson-aalen-cumulative-hazards.md)

Suppose everyone enters observation at zero and has one event or [censoring](censoring-statistics.md) time. At distinct recorded time $t_j$, let $n_j$ observations terminate, of which $d_j$ are events, and use the pre-time [risk set](risk-set.md) size $r_j=\sum_{k\geq j}n_k$. For the grouped [Nelson–Aalen estimator](nelson-aalen-estimator.md), $\widehat H(t_j)=\sum_{k\leq j}d_k/r_k$. Exchanging sums gives $\sum_j n_j\widehat H(t_j)=\sum_k(d_k/r_k)\sum_{j\geq k}n_j=\sum_kd_k$. The unweighted sum over distinct times generally does not have this property. Processing each observation separately after breaking ties also restores the corresponding unweighted identity on the resulting artificial time grid.

## ↑ Ancestors (7)

1. [Event-count identity for Nelson–Aalen cumulative hazards](event-count-identity-for-nelson-aalen-cumulative-hazards.md)
2. [Nelson–Aalen estimator](nelson-aalen-estimator.md)
3. [Survival analysis](survival-analysis-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-38/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-46/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-41/4/c/solution.md)
