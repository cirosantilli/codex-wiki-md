<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For independent [binomial distributions](../../../../../../binomial-distribution.md) in the two trial arms, the estimate of the [log risk ratio](../../../../../../log-risk-ratio.md) is

$$
\widehat\ell=\log\frac{1/12}{4/10}=\log\frac5{24}=-1.5686.
$$

The [delta method](../../../../../../delta-method.md) gives $\operatorname{Var}(\log\widehat p)\simeq(1-p)/(np)$; replacing $p$ by the [sample proportion](../../../../../../sample-proportion.md) gives $1/d-1/n$, where $d$ is the event count. Adding the independent arm contributions therefore gives

$$
\widehat{\operatorname{Var}}(\widehat\ell)
=\left(\frac11-\frac1{12}\right)+\left(\frac14-\frac1{10}\right)
=\frac{16}{15}=1.0667.
$$

The [standard error](../../../../../../standard-error.md) is $\sqrt{16/15}=1.0328$. Using the stipulated normal quantile two, the approximate [confidence interval](../../../../../../confidence-interval.md) is

$$
\boxed{\widehat\ell\pm2\operatorname{SE}(\widehat\ell)
=(-3.6342,\ 0.4970).}
$$

The point estimate of the [risk ratio](../../../../../../risk-ratio.md) is $5/24\simeq0.208$, corresponding to approximately 79% lower mortality risk in the transfusion arm. Exponentiating the endpoints gives an approximate 95% [confidence interval](../../../../../../confidence-interval.md) for the [risk ratio](../../../../../../risk-ratio.md) of $(0.0264,1.6437)$. It includes one, so the trial is compatible with no difference as well as substantial benefit or some harm. **The point estimate favours transfusion, but the data are too imprecise to establish a difference at the 5% level.** These are large-sample approximations, especially rough with only one event in an arm. A frequentist [confidence interval](../../../../../../confidence-interval.md) describes repeated-sampling coverage, not a 95% posterior [probability](../../../../../../probability.md) for this fixed parameter.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
