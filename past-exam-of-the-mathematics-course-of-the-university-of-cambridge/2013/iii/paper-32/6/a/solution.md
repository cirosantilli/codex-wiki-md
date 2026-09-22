<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use one row per consecutive at-risk episode, retaining a patient identifier for dependence and an episode number for event order. In calendar time, the intervals are $(\text{start},\text{stop}]$; status is one if the row ends in a headache and zero if it ends in censoring. Patient 001 contributes

| Patient | Next-event episode | Start | Stop | Event | $z$ |
| --- | --- | --- | --- | --- | --- |
| 001 | 1 | 0 | 24.8 | 1 | 0 |
| 001 | 2 | 24.8 | 33.1 | 1 | 0 |
| 001 | 3 | 33.1 | 40.2 | 1 | 0 |
| 001 | 4 | 40.2 | 51.9 | 1 | 0 |
| 001 | 5 | 51.9 | 60.0 | 0 | 0 |

The fifth episode is censored, not a fifth observed headache. All rows retain $z=0$. This [start-stop recurrent-event data layout](../../../../../../start-stop-recurrent-event-data-layout.md) corresponds to the [counting-process intensity in survival analysis](../../../../../../counting-process-intensity-in-survival-analysis.md)

$$
\lambda_i(t\mid\mathcal H_{t-})=Y_i(t)h_0(t)e^{\beta z_i},
$$

where $Y_i(t)$ indicates that the patient is currently observed and eligible for a headache. Fit the [regression coefficient](../../../../../../regression-coefficient.md) by [Cox partial likelihood](../../../../../../cox-partial-likelihood.md) using the resulting [risk sets](../../../../../../risk-set.md), and estimate the baseline cumulative hazard nonparametrically, for example by the [Breslow estimator](../../../../../../breslow-estimator.md). Patient rows are portions of one history, not new independent patients.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
