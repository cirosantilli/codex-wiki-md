<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume the two trial arms are independent samples, their cost and survival means have a valid joint [normal approximation](../../../../../../normal-approximation.md), and the supplied [standard errors](../../../../../../standard-error.md) and [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) estimate the joint uncertainty in their mean differences. This could follow from a [central limit theorem](../../../../../../central-limit-theorem.md) for patient-level cost/survival pairs, with finite second moments and suitably handled survival follow-up. The supplied [covariance matrix](../../../../../../covariance-matrix.md) for $(\widehat{\Delta C},\widehat{\Delta E})$ is

$$
\widehat\Sigma=\begin{pmatrix}300^2&0.5(300)(15)\\0.5(300)(15)&15^2\end{pmatrix}
=\begin{pmatrix}90000&2250\\2250&225\end{pmatrix}.
$$

The off-diagonal entry has units pounds times days, and must not be discarded. Independence of trial arms does not mean cost and survival increments are independent: patient-level cost and survival are paired within each arm.

For a proposed ratio $r$, the null assertion is $\Delta C-r\Delta E=0$. Its estimated [variance](../../../../../../variance-split.md) is $90000-4500r+225r^2$. [Fieller's theorem](../../../../../../fieller-s-theorem.md) inverts the associated two-sided normal tests. With $q=\Phi^{-1}(0.975)\approx1.96$, retain $r$ when

$$
(1800-45r)^2\leq q^2(90000-4500r+225r^2).
$$

Expanding gives

$$
(2025-225q^2)r^2+(-162000+4500q^2)r+(3240000-90000q^2)\leq0.
$$

The leading coefficient is positive, since $45>q(15)$; the effect increment is separated from zero at this level. With $q^2=3.841459$, the polynomial is approximately

$$
1160.672r^2-144713.435r+2894268.706.
$$

It is nonpositive between its two real roots. The resulting approximate $95\%$ [Fieller confidence set](../../../../../../fieller-s-theorem.md) is therefore a bounded [confidence interval](../../../../../../confidence-interval.md):

$$
\boxed{\operatorname{ICER}\in[25.02,99.66]\text{ pounds per additional survival day}.}
$$

On the $365$-day life-year scale the endpoints are approximately £9,133 and £36,376. Exact coverage would need an exact pivot with its corresponding critical value; using estimated covariance and a [central limit theorem](../../../../../../central-limit-theorem.md) makes this an asymptotic interval. In other data, a poorly determined denominator can give unbounded or disconnected [Fieller confidence sets](../../../../../../fieller-s-theorem.md), which should not be replaced by an artificially bounded interval.

An alternative is a paired [bootstrap](../../../../../../bootstrapping-statistics.md): independently resample patients within each randomized arm, keeping each patient's cost and survival together; recompute both mean differences and their ratio in each replicate. The $2.5\%$ and $97.5\%$ empirical ratio quantiles give a [percentile bootstrap confidence interval](../../../../../../percentile-bootstrap-confidence-interval.md). The raw paired data are needed to calculate it, so the numerical endpoints cannot be obtained from this summary table alone. Near-zero bootstrap effect increments or sign changes warn that ordinary ratio-percentile intervals may be unreliable; one should retain the joint cost/effect uncertainty or invert a suitable bootstrap test instead.

A simpler first-order alternative is the [delta method](../../../../../../delta-method.md). For $r=\Delta C/\Delta E$, the gradient is $(1/\Delta E,-\Delta C/\Delta E^2)$, giving

$$
\widehat{\operatorname{Var}}(\widehat r)=\frac{90000+40^2(225)-2(40)(2250)}{45^2}=133.333.
$$

The resulting approximate [Wald confidence interval](../../../../../../wald-confidence-interval.md) is $40\pm1.96\sqrt{133.333}=(17.37,62.63)$ pounds per day. Its symmetric first-order form misses the denominator's nonlinear effect, explaining its marked difference from the [Fieller confidence set](../../../../../../fieller-s-theorem.md); it is not the preferred ratio interval here.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
