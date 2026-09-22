<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

$Y_{j,k}$ is the number in group $k$ still observed and event-free immediately before event time $a_j$: its group-specific [risk set](../../../../../risk-set.md) size. Set $Y_j=Y_{j,0}+Y_{j,1}$. Under the common [hazard function](../../../../../hazard-function.md) and conditional on exactly one event at that time, each at-risk individual has the same infinitesimal event probability. Therefore

$$
\boxed{p(j,k)=\frac{Y_{j,k}}{Y_j}.}
$$

The indicator $g_{\pi(j)}$ records whether the event came from group 1, while $p(j,1)$ is its conditional expectation under equal hazards. Thus $z_j$ is the observed-minus-expected group-1 event count at that time. Under the null these are [martingale differences](../../../../../martingale-difference.md), with conditional [variance](../../../../../variance-split.md)

$$
\operatorname{Var}(z_j\mid\mathcal H_{a_j-})=p_j(1-p_j),
\qquad p_j=Y_{j,1}/Y_j.
$$

The [log-rank statistic](../../../../../log-rank-statistic.md) $z=\sum_jz_j$ has null mean zero. Its predictable variance estimate is $V=\sum_jp_j(1-p_j)$, so **the equal-hazards test uses**

$$
\boxed{Z=\frac{z}{\sqrt V}\ \dot\sim N(0,1),\qquad
\frac{z^2}{V}\ \dot\sim\chi^2_1.}
$$

Use a two-sided large-sample [log-rank test](../../../../../log-rank-test.md) if no direction was prespecified; $V>0$ and adequate information are needed. The variance is the no-ties form. A positive $z$ indicates more group-1 events than expected. [Independent censoring](../../../../../independent-censoring.md) conditional on the model is required for these at-risk event intensities to describe the data.

Under the [proportional hazards model](../../../../../proportional-hazards-model.md), the total instantaneous group-$k$ rate is $Y_{j,k}e^{\beta k}h_0(a_j)$. Conditioning on the next event cancels the [baseline hazard](../../../../../baseline-hazard.md), giving

$$
\boxed{p_\beta(j,k)=\frac{Y_{j,k}e^{\beta k}}
 {Y_{j,0}+Y_{j,1}e^\beta}.}
$$

Keep $z_j$ defined using its null probability $p(j,1)$, as in the question. Its conditional expectation under the alternative is

$$
\boxed{\mathbb E_\beta[z_j\mid\mathcal H_{a_j-}]
=\frac{Y_{j,1}e^\beta}{Y_{j,0}+Y_{j,1}e^\beta}
 -\frac{Y_{j,1}}{Y_j}
=\frac{Y_{j,0}Y_{j,1}(e^\beta-1)}
 {Y_j(Y_{j,0}+Y_{j,1}e^\beta)}.}
$$

It is zero at $\beta=0$, as required, and has the sign of $\beta$ when both groups remain at risk. Replacing $p(j,1)$ inside the definition of $z_j$ with the alternative probability would give a different residual, whose mean would instead be zero under that alternative.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
