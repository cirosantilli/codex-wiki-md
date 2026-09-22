<h1 id="kaplan-meier-estimator-with-delayed-entry">Kaplan–Meier estimator with delayed entry</h1>

↑ **Parent:** [Kaplan–Meier estimator](kaplan-meier-estimator.md)

For independently [left-truncated](left-truncation.md) and [right-censored](right-censoring.md) [survival data](survival-data.md), let $E_i$ and $Y_i$ be entry and exit times on the same clock. At each distinct event time $t_j$, the [risk set](risk-set.md) is $R_j=\{i:E_i<t_j\le Y_i\}$, with size $r_j$, and $d_j$ events occur. The [Kaplan–Meier estimator](kaplan-meier-estimator.md) is

$$
\widehat S(t)=\prod_{t_j\le t}\left(1-\frac{d_j}{r_j}\right).
$$

Before entry a subject contributes neither an event nor time at risk. Thus adding observed entrants can increase successive [risk sets](risk-set.md); pretending that all subjects were observed from time zero distorts the estimated [hazard function](hazard-function.md). The estimator identifies the [survival function](survival-function.md) over ages covered by observation; normalization from birth requires observation arbitrarily close to time zero or additional knowledge of earlier survival.

## ↑ Ancestors (6)

1. [Kaplan–Meier estimator](kaplan-meier-estimator.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Greenwood formula](greenwood-formula.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/5/b/i/solution.md)
