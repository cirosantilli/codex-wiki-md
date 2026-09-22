<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At each distinct event time $t_j$, let $d_j$ events occur among $r_j$ people in the [risk set](../../../../../../risk-set.md). The [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) is

$$
\widehat S(t)=\prod_{t_j\leq t}\left(1-\frac{d_j}{r_j}\right);
$$

censorings remove people from later risk sets but create no factor.

[Left truncation](../../../../../../left-truncation.md), or delayed entry, means that an individual is observed only after surviving to an entry time. A registry assembled from patients alive when a clinic opens is a practical example. Adapt Kaplan–Meier by admitting each person to the risk set only at their entry time.

[Period survival analysis](../../../../../../period-survival-analysis.md) is useful when recent prognosis is desired but complete long-term follow-up of a recent diagnosis cohort is unavailable. For a chosen calendar year, intersect every patient's observed follow-up with that year. Express the surviving pieces on the time-since-diagnosis scale, treat the beginning of the calendar window as delayed entry and its end as right censoring, and apply Kaplan–Meier with those entry and exit times.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
