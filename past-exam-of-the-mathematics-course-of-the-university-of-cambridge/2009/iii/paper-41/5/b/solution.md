<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the individual background [survivor function](../../../../../../survival-function.md) and common excess component by

$$
F_B^{(i)}(t)=\exp\left[-\int_0^t h_B^{(i)}(u)\,du\right],
\qquad
\boxed{F_E(t)=\exp\left[-\int_0^t h_E(u)\,du\right].}
$$

Integrating the additive [hazard function](../../../../../../hazard-function.md) decomposition gives

$$
F^{(i)}(t)=F_B^{(i)}(t)F_E(t),\qquad F_E(t)=\frac{F^{(i)}(t)}{F_B^{(i)}(t)}.
$$

The [relative survivor function](../../../../../../relative-survivor-function.md) therefore compares actual survival with the survival expected from background mortality, and is common across individuals under this model. If $h_E\geq0$, it is the [survivor function](../../../../../../survival-function.md) of a hypothetical process having only the [excess hazard](../../../../../../excess-hazard.md). If excess mortality can be negative, the ratio may exceed one and lacks an ordinary survival-probability interpretation.

To estimate it, let $Y_i(u)$ indicate that individual $i$ is in the [risk set](../../../../../../risk-set.md), let $Y(u)=\sum_iY_i(u)$, and let $N(u)$ count all observed deaths. Assume appropriate [independent censoring](../../../../../../independent-censoring.md). The aggregate event intensity is

$$
\sum_iY_i(u)h^{(i)}(u)
=Y(u)h_E(u)+\sum_iY_i(u)h_B^{(i)}(u).
$$

Consequently the background correction must use the current risk-set average

$$
\overline h_B(u)=\frac{\sum_iY_i(u)h_B^{(i)}(u)}{Y(u)},\qquad
B_R(t)=\int_0^t\overline h_B(u)\,du,
$$

only on the observed range where $Y>0$. Dividing the event count by $Y$ estimates the total hazard there. Subtracting the known average background gives the [offset-adjusted cumulative hazard estimator](../../../../../../offset-adjusted-cumulative-hazard-estimator.md)

$$
\boxed{\widehat H_E(t)=\sum_{t_j\leq t}\frac{d_j}{r_j}-B_R(t).}
$$

Here $d_j$ is the event count at $t_j$ and $r_j=Y(t_j)$; under an untied scheme $d_j=1$. One possible estimate is $\widehat F_{E,\exp}=\exp[-\widehat H_E]$.

A product-limit version retains the full event fraction, which is especially relevant when the excess mortality is not small. Estimate the relative-survival differential equation $dF_E/F_E=-dH_E$ by

$$
\frac{d\widehat F_E(t)}{\widehat F_E(t-)}=-\frac{dN(t)}{Y(t)}+\overline h_B(t)\,dt.
$$

At an event time it multiplies the curve by $1-d_j/r_j$. Between events it solves $\widehat F_E'=\overline h_B\widehat F_E$. Starting at one therefore gives the [risk-set-adjusted relative survivor estimator](../../../../../../risk-set-adjusted-relative-survivor-estimator.md)

$$
\boxed{\widehat F_E(t)=\exp[B_R(t)]\prod_{t_j\leq t}\left(1-\frac{d_j}{r_j}\right)
=\exp[B_R(t)]\widehat S_{\mathrm{KM}}(t).}
$$

The [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) factor accounts for observed all-cause mortality; the continuous multiplier corrects for known background mortality. The exponential cumulative-hazard version instead has event jumps $\exp(-d_j/r_j)$; it is close when event fractions are small but is not identical to this product-limit version.

Even if each [background hazard](../../../../../../background-hazard.md) is small, its accumulated contribution over long follow-up cannot simply be discarded. Nor should the excess contribution be linearized merely because the background is small. Using the known background integral inside the exponential avoids both errors. The average is over the evolving [risk set](../../../../../../risk-set.md): replacing it by an initial-cohort mean, or dividing by an arbitrary average of individual background [survivor functions](../../../../../../survival-function.md), is generally wrong when the [background hazards](../../../../../../background-hazard.md) differ. [Censoring](../../../../../../censoring-statistics.md) and deaths change which individuals contribute to the background correction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
