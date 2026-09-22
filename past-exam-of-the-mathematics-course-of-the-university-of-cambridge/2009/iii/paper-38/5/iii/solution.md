<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For patient $h$, let $Z_h(t)\in\{1,2,3\}$ be the fatigue state at time $t$ years since study entry. Let the [covariate](../../../../../../covariate.md) vector be $z=(s,d,a,g)^T$, representing the sex indicator, arthritis duration in years, HAQ disability score and haemoglobin measurement. Conditional on these [covariates](../../../../../../covariate.md), the [continuous-time multi-state model](../../../../../../continuous-time-multi-state-model.md) has the [Markov property](../../../../../../markov-property.md) and [generator matrix](../../../../../../generator-matrix.md)

$$
Q(z)=\begin{pmatrix}
-q_{12}(z)&q_{12}(z)&0\\
q_{21}(z)&-q_{21}(z)-q_{23}(z)&q_{23}(z)\\
0&q_{32}(z)&-q_{32}(z)
\end{pmatrix}.
$$

Each allowed [transition intensity](../../../../../../transition-intensity.md) has its own [log-linear transition intensity model](../../../../../../log-linear-transition-intensity-model.md), $q_{ij}(z)=\exp(\eta_{ij}+b_{ij}^Tz)$. The zero entries exclude direct instantaneous jumps between mild and severe states, and the diagonals enforce zero row sums.

To express the estimates correctly, the printed intensities are evaluated at the sample [covariate](../../../../../../covariate.md) means $\bar z$, not at $z=0$. Order the allowed transitions as $12,21,23,32$. Their estimates are

$$
\boxed{\widehat q_{ij}(z)=\widehat q_{ij}(\bar z)\exp\{\widehat b_{ij}^T(z-\bar z)\},\qquad
(\widehat q_{12}(\bar z),\widehat q_{21}(\bar z),\widehat q_{23}(\bar z),\widehat q_{32}(\bar z))=(0.2344,0.5509,0.4247,0.5822),}
$$

with rows indexed by that transition order and columns by $s,d,a,g$ in

$$
\widehat B=\begin{pmatrix}
-0.7695&0.001331&0.9913&0.01368\\
-0.3285&-0.01047&-0.3006&-0.002136\\
0.3811&-0.0226&-0.05399&-0.03375\\
0.1712&-0.0264&-1.045&-0.02616
\end{pmatrix}.
$$

Equivalently, the uncentred intercept is $\widehat\eta_{ij}=\log\widehat q_{ij}(\bar z)-\widehat b_{ij}^T\bar z$. The means are not printed, so the displayed rates cannot be treated as numerical zero-covariate intercepts.

The assumptions are independent patients conditional on their [covariates](../../../../../../covariate.md); correctly observed fatigue states; no unmodelled history dependence once current state and [covariates](../../../../../../covariate.md) are known; positive adjacent-state intensities with the specified exponential covariate dependence and no interaction terms; and a noninformative observation and censoring mechanism for the conditional state-process likelihood. With fixed [covariates](../../../../../../covariate.md) the rates are homogeneous in time and [holding times](../../../../../../holding-time.md) are exponential. Covariates updated at visits are treated as piecewise constant between observations, so each such interval has a constant generator, a [piecewise-constant covariate approximation](../../../../../../piecewise-constant-covariate-approximation.md). In particular this is an approximation if a quantity such as duration changes continuously between visits.

For observations $Z_h(t_{hk})=s_{hk}$, conditioning on the initial observed state, the [panel-observed multi-state likelihood](../../../../../../panel-observed-multi-state-likelihood.md) is a product over patients and intervals of

$$
\bigl[e^{(t_{h,k+1}-t_{hk})Q(z_{hk})}\bigr]_{s_{hk},s_{h,k+1}},
$$

where $z_{hk}$ is the covariate value held over that interval. Multiple unobserved jumps within an interval are integrated out by this [transition matrix](../../../../../../stochastic-matrix.md). For example, a mild state followed by a severe state can have positive likelihood despite $q_{13}=0$, because an unobserved moderate state can intervene. The panel observations within a patient are not independent; it is the [Markov property](../../../../../../markov-property.md) that justifies multiplying conditional [transition probabilities](../../../../../../transition-probability.md). The piecewise-constant handling of changing covariates is specified in [the msm model documentation](https://chjackson.github.io/msm/reference/msm.html).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
