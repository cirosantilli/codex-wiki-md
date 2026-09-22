<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the usual semiparametric [Cox proportional-hazards model](../../../../../cox-proportional-hazards-model.md) with observed [covariates](../../../../../covariate.md) $z_i$:

$$
h_i(t)=h_0(t)e^{\beta^Tz_i}.
$$

The [covariates](../../../../../covariate.md) are implicit in the question's regression fit, even though the displayed data notation only lists exit times and event indicators. Assume entry at a common origin, time-constant [covariates](../../../../../covariate.md), distinct observed times and [independent censoring](../../../../../independent-censoring.md). Write $R_i=\{j:x_j\geq x_i\}$ and $w_j(\beta)=e^{\beta^Tz_j}$. Conditional on a single event at $x_i$ in its [risk set](../../../../../risk-set.md), the chance that individual $i$ supplies it is

$$
\frac{h_0(x_i)w_i(\beta)}{\sum_{j\in R_i}h_0(x_i)w_j(\beta)}
=\frac{w_i(\beta)}{\sum_{j\in R_i}w_j(\beta)}.
$$

The [baseline hazard](../../../../../baseline-hazard.md) cancels. Consequently estimate $\beta$ by maximizing [Cox partial likelihood](../../../../../cox-partial-likelihood.md)

$$
L_C(\beta)=\prod_{i=1}^m\left[\frac{e^{\beta^Tz_i}}{\sum_{j\in R_i}e^{\beta^Tz_j}}\right]^{v_i},
\qquad
\ell_C(\beta)=\sum_i v_i\left[\beta^Tz_i-\log\sum_{j\in R_i}e^{\beta^Tz_j}\right].
$$

For example, the [score and information of Cox partial likelihood](../../../../../score-and-information-of-cox-partial-likelihood.md) follow by differentiation. Define $S_i^{(0)}=\sum_{j\in R_i}w_j$, $S_i^{(1)}=\sum_{j\in R_i}w_jz_j$ and $S_i^{(2)}=\sum_{j\in R_i}w_jz_jz_j^T$. Then

$$
U(\beta)=\sum_i v_i\left(z_i-\frac{S_i^{(1)}}{S_i^{(0)}}\right),
\qquad
I(\beta)=\sum_i v_i\left[\frac{S_i^{(2)}}{S_i^{(0)}}-
\frac{S_i^{(1)}S_i^{(1)T}}{(S_i^{(0)})^2}\right].
$$

When a finite identifiable maximum exists, iterate $\beta\leftarrow\beta+I(\beta)^{-1}U(\beta)$ until convergence. The [Observed Fisher information](../../../../../observed-fisher-information.md) also gives the usual asymptotic coefficient uncertainty. Censored subjects enter the relevant [risk sets](../../../../../risk-set.md), even though they supply no numerator event factor.

After fitting $\widehat\beta$, estimate the [cumulative hazard](../../../../../cumulative-hazard-function.md) of the reference subject by the [Breslow estimator](../../../../../breslow-estimator.md)

$$
\boxed{\widehat H_0(t)=\sum_{i:x_i\leq t}\frac{v_i}{\sum_{j\in R_i}e^{\widehat\beta^Tz_j}}.}
$$

Its jump at an event is the observed event count divided by the total fitted [hazard multiplier](../../../../../hazard-multiplier.md) at risk. The estimate is an integrated [baseline hazard](../../../../../baseline-hazard.md), with hazard represented by a measure placing these jumps at observed event times. If a smooth ordinary hazard function is wanted, smooth these increments with a chosen kernel and bandwidth; differentiating the step function as an ordinary function would incorrectly give zero away from the jumps. The fitted individual [cumulative hazard](../../../../../cumulative-hazard-function.md) is $\widehat H_i(t)=e^{\widehat\beta^Tz_i}\widehat H_0(t)$ over that individual's follow-up. The invariances below concern this [Cox partial likelihood](../../../../../cox-partial-likelihood.md) fit and this [Breslow estimator](../../../../../breslow-estimator.md); they need not hold for a fully parametric proportional-hazards fit or an arbitrarily smoothed hazard estimator.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
