<h1 id="6/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The history $\mathcal H_{t-}$ contains the information observed strictly before $t$: baseline characteristics, previous events and [censoring](../../../../../../censoring-statistics.md), and therefore which individuals are currently eligible and under observation. Formally it is the pre-$t$ information in the relevant [filtration](../../../../../../filtration-probability-theory.md). The [at-risk process](../../../../../../at-risk-process.md) $Y_i(t)$ is 1 if individual $i$ is observed and event-free immediately before $t$, and 0 otherwise. Let $Y_+(t)=\sum_iY_i(t)$ and write $dH(t)=h(t)dt$ for the [cumulative hazard](../../../../../../cumulative-hazard-function.md) increment.

The [counting-process intensity in survival analysis](../../../../../../counting-process-intensity-in-survival-analysis.md) gives

$$
\boxed{\Pr(dN_i(t)=1\mid\mathcal H_{t-})
=Y_i(t)h(t)dt+o(dt).}
$$

The common conditional [hazard function](../../../../../../hazard-function.md) is assumed to remain applicable after conditioning on the observed history, as under suitable [independent censoring](../../../../../../independent-censoring.md). Summing gives **the conditional mean of the total event increment**:

$$
\boxed{\mathbb E[dN_+(t)\mid\mathcal H_{t-}]
=Y_+(t)dH(t)+o(dt).}
$$

On times with $Y_+(t)>0$, invert this relation to estimate the hazard increment:

$$
\boxed{d\widehat H(t)=\frac{dN_+(t)}{Y_+(t)},\qquad
\widehat H(t)=\int_0^t\frac{\mathbf1_{\{Y_+(u)>0\}}}{Y_+(u)}\,dN_+(u)
=\sum_{a_j\leq t}\frac1{Y_+(a_j)}.}
$$

The last sum is for untied events. This is the [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md); for ties replace 1 by the number of events at that time. No increment can be estimated once the [risk set](../../../../../../risk-set.md) is empty.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [6](../../6.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
