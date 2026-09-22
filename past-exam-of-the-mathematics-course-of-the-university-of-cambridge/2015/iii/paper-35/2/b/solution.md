<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The event and nonevent cell counts are $(a,b)=(30,60)$ and $(c,d)=(20,40)$. Thus the estimated [odds ratio](../../../../../../odds-ratio.md) and [log odds ratio](../../../../../../log-odds-ratio.md) are

$$
\widehat{\operatorname{OR}}=\frac{30/60}{20/40}=1,
\qquad \widehat\ell=\log1=0.
$$

For [independent](../../../../../../independent-random-variables.md) binomial groups, the [delta method](../../../../../../delta-method.md) gives

$$
\widehat{\operatorname{Var}}(\widehat\ell)
=\frac1{30}+\frac1{60}+\frac1{20}+\frac1{40}
=\frac18=0.125,
\qquad \operatorname{SE}(\widehat\ell)=\sqrt{0.125}=0.353553\ldots.
$$

Using the permitted [normal approximation](../../../../../../normal-approximation.md) quantile of 2, **the approximate 95% interval is**

$$
\boxed{\widehat\ell=0,\qquad \mathrm{CI}_{\log\mathrm{OR}}=(-0.7071,0.7071).}
$$

The observed odds of death are equal between groups. The [confidence interval](../../../../../../confidence-interval.md) includes zero and allows appreciable effects in either direction; it does not demonstrate equivalence. Exponentiating gives an [odds ratio](../../../../../../odds-ratio.md) interval approximately $(0.493,2.028)$, so the data are compatible with roughly half to twice the death odds for the first treatment relative to the second. The tabulated [standard error](../../../../../../standard-error.md) is rounded.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
