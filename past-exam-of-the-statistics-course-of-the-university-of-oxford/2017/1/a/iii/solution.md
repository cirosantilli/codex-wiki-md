<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a [Bernoulli distribution](../../../../../bernoulli-distribution.md) with fixed $0<p<1$, the [mean](../../../../../expected-value-split.md) and [variance](../../../../../variance-split.md) are $p$ and $p(1-p)$. The [odds](../../../../../odds.md) transformation $g(x)=x/(1-x)$ has [derivative](../../../../../derivative.md) $g'(x)=(1-x)^{-2}$. Applying the [delta method](../../../../../delta-method.md) from part (ii),

$$
\boxed{\frac{\overline X}{1-\overline X}\mathrel{\dot\sim}
N\!\left(\frac p{1-p},\frac{p}{n(1-p)^3}\right).}
$$

More precisely, $\sqrt n\{\overline X/(1-\overline X)-p/(1-p)\}$ converges to a [normal distribution](../../../../../normal-distribution.md) of [mean](../../../../../expected-value-split.md) zero and [variance](../../../../../variance-split.md) $p/(1-p)^3$, after defining the statistic arbitrarily on $\overline X=1$. That exceptional [event](../../../../../event.md) has [probability](../../../../../probability.md) $p^n\to0$, so this extension does not change the limit. The unextended ratio is undefined there and has no finite exact [variance](../../../../../variance-split.md) if interpreted as infinite. At $p=0$ it is zero almost surely; at $p=1$ the denominator is always zero. This is the [delta method for Bernoulli odds](../../../../../delta-method-for-bernoulli-odds.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
