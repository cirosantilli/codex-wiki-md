<h1 id="6/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $q_t=\Pr(dN_+(t)=1\mid\mathcal H_{t-})$. A binary event increment has conditional [variance](../../../../../../variance-split.md) $q_t(1-q_t)$. Since $q_t=Y_+(t)h(t)dt+o(dt)$, its squared mean is of second order, giving

$$
\boxed{\operatorname{Var}(dN_+(t)\mid\mathcal H_{t-})
=Y_+(t)dH(t)+o(dt).}
$$

Treating the predictable [risk set](../../../../../../risk-set.md) size as known given the history, the [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) increment therefore has first-order variance

$$
\boxed{\operatorname{Var}(d\widehat H(t)\mid\mathcal H_{t-})
=\frac{dH(t)}{Y_+(t)}+o(dt),\qquad Y_+(t)>0.}
$$

Substitute $d\widehat H=dN_+/Y_+$ for $dH$ to obtain the estimated increment variance $dN_+/Y_+^2$. Summing these estimated predictable variances gives **the usual [Nelson–Aalen variance estimator](../../../../../../nelson-aalen-variance-estimator.md)**:

$$
\boxed{\widehat{\operatorname{Var}}(\widehat H(t))
=\int_0^t\frac{\mathbf1_{\{Y_+(u)>0\}}}{Y_+(u)^2}\,dN_+(u)
=\sum_{a_j\leq t}\frac1{Y_+(a_j)^2}.}
$$

The martingale $dN_+-Y_+dH$ has orthogonal increments, which justifies accumulating the predictable variances of the estimation error. This is an estimated sampling variance on the observed at-risk range, not a claim of exact finite-sample unbiasedness after the [risk set](../../../../../../risk-set.md) becomes empty. For multiple events at an event time the usual extension replaces the numerator 1 by the event count.

## ↑ Ancestors (11)

1. [3](../3.md)
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
