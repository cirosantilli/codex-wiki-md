<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Cox proportional-hazards model](../../../../../../cox-proportional-hazards-model.md) specifies

$$
\boxed{h_i(t)=h_0(t)\exp(\beta^Tz_i),}
$$

where $h_0(t)$ is an unspecified common baseline [hazard](../../../../../../hazard-function.md) and $z_i$ is the individual's [covariate](../../../../../../covariate.md) vector. The [hazard ratio](../../../../../../hazard-ratio.md) for two fixed [covariate](../../../../../../covariate.md) vectors is $\exp[\beta^T(z_i-z_k)]$, constant in time. Assume independent subjects and [independent censoring](../../../../../../independent-censoring.md) conditional on their [covariates](../../../../../../covariate.md), and use the question's absence of tied events.

Let $t_j$ be an event time, $i_j$ its failing subject, and $R_j$ the [risk set](../../../../../../risk-set.md) immediately before that time. In a short interval of length $dt$, the conditional probability that subject $i$ fails, given one failure among those at risk, is

$$
\frac{h_i(t_j)dt+o(dt)}{\sum_{k\in R_j}h_k(t_j)dt+o(dt)}
\longrightarrow\frac{e^{\beta^Tz_i}}{\sum_{k\in R_j}e^{\beta^Tz_k}}.
$$

The baseline [hazard](../../../../../../hazard-function.md) cancels. Multiplying the successive conditional event-identity factors gives the [Cox partial likelihood](../../../../../../cox-partial-likelihood.md) for $\beta$:

$$
\boxed{L_p(\beta)=\prod_j
\frac{e^{\beta^Tz_{i_j}}}{\sum_{k\in R_j}e^{\beta^Tz_k}},\qquad
\ell_p(\beta)=\sum_j\left[\beta^Tz_{i_j}-\log\sum_{k\in R_j}e^{\beta^Tz_k}\right].}
$$

This is a partial [likelihood](../../../../../../likelihood-function.md), not the full survival [likelihood](../../../../../../likelihood-function.md) for the unspecified $h_0$. [Risk sets](../../../../../../risk-set.md) evolve with the observed history; the derivation uses their successive conditional [hazards](../../../../../../hazard-function.md), rather than assuming the [risk sets](../../../../../../risk-set.md) themselves are independent.

Define $w_{jk}(\beta)=e^{\beta^Tz_k}/\sum_{\ell\in R_j}e^{\beta^Tz_\ell}$ and $\bar z_j(\beta)=\sum_{k\in R_j}w_{jk}(\beta)z_k$. For component $r$,

$$
\boxed{\frac{\partial\ell_p}{\partial\beta_r}
=\sum_j\left[z_{i_j,r}-\sum_{k\in R_j}w_{jk}(\beta)z_{k,r}\right].}
$$

Differentiating again gives

$$
\frac{\partial^2\ell_p}{\partial\beta_r\partial\beta_s}
=-\sum_j\left[\sum_{k\in R_j}w_{jk}z_{k,r}z_{k,s}
-\bar z_{j,r}\bar z_{j,s}\right].
$$

Thus the [score and information of Cox partial likelihood](../../../../../../score-and-information-of-cox-partial-likelihood.md) are the sum of event-minus-risk-mean contrasts and the sum of risk-weighted covariance matrices, respectively. The Hessian is negative semidefinite; the [likelihood](../../../../../../likelihood-function.md) is concave, with strict identifiability requiring variation in the relevant risk-set [covariates](../../../../../../covariate.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
