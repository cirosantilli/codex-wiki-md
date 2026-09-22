<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the population identity, write $X=\min(T,C)$, $V=\mathbf1_{\{T\leq C\}}$, and $G(t)=\mathbb P(C\geq t)$. Assume [independent censoring](../../../../../../independent-censoring.md), with $f_T(t)=h(t)S(t)$. Then

$$
\mathbb EV=\int_0^\infty f_T(t)G(t)dt,
$$

while the [Tonelli theorem](../../../../../../tonelli-theorem.md) and the [cumulative hazard function](../../../../../../cumulative-hazard-function.md) give

$$
\mathbb EH(X)=\mathbb E\int_0^\infty h(t)\mathbf1_{\{X\geq t\}}dt
=\int_0^\infty h(t)S(t)G(t)dt=\mathbb EV.
$$

This is [mean accumulated hazard under independent censoring](../../../../../../mean-accumulated-hazard-under-independent-censoring.md), proving $\mathbb E[V-H(X)]=0$. For the fitted [martingale residual](../../../../../../martingale-residual.md) $Y=V-\widehat H(X)$,

$$
\boxed{\mathbb EY=-\mathbb E[\widehat H(X)-H(X)],\qquad
|\mathbb EY|\leq\mathbb E|\widehat H(X)-H(X)|.}
$$

Hence its [expectation](../../../../../../expected-value.md) is approximately zero when the fitted hazard error at the observed time is small in mean. This spells out the required sense of a good estimate; pointwise consistency alone does not control a divergent tail. In particular, a [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) with zero final survival gives infinite transformed times there and cannot supply finite residuals without a tail restriction. Neither exact finite-sample zero mean nor validity under [informative censoring](../../../../../../informative-censoring.md) is being assumed.

To check an omitted explanatory variable $Z$, plot the [martingale residuals](../../../../../../martingale-residual.md) against $Z$ or compare groupwise mean residuals, using a smooth trend or appropriate uncertainty intervals. Under a correct conditional survival model and conditionally [independent censoring](../../../../../../independent-censoring.md), $\mathbb E[Y\mid Z]$ should be approximately zero. A systematic positive trend indicates more observed failures than the fitted accumulated hazard predicts; a negative trend indicates fewer. Such patterns suggest adding $Z$, a nonlinear term or an interaction and reassessing the fit. The bounded-above, often long negative tail of [martingale residuals](../../../../../../martingale-residual.md) means that the diagnostic is a mean-pattern check, not a requirement for symmetric Gaussian residuals.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
