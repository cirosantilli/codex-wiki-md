<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [central limit theorem](../../../../../../central-limit-theorem.md) states that for independent identically distributed variables with finite [mean](../../../../../../expected-value.md) $m$ and positive finite [variance](../../../../../../variance-split.md) $v$,

$$
\frac{\sum_{i=1}^nY_i-nm}{\sqrt{nv}}\xrightarrow{d}N(0,1).
$$

Applying it to the exponential gaps gives

$$
\frac{\lambda T_n-n}{\sqrt n}\xrightarrow{d}N(0,1),\qquad
\boxed{T_n\approx N\left(\frac n\lambda,\frac n{\lambda^2}\right).}
$$

Invert the approximate central probability $\mathbb P(-1.96\leq(\lambda T_n-n)/\sqrt n\leq1.96)\simeq0.95$. For an observed positive total $T_n$, an approximate 95% [confidence interval](../../../../../../confidence-interval.md) is

$$
\boxed{\left[\frac{n-1.96\sqrt n}{T_n},\frac{n+1.96\sqrt n}{T_n}\right]\cap(0,\infty).}
$$

Equivalently its endpoints are $\widehat\lambda(1\pm1.96/\sqrt n)$, with a nonpositive lower endpoint replaced by the parameter boundary. This is a large-$n$ approximation; the exact gamma law of $T_n$ permits an exact interval if needed. It is a two-sided parameter interval, not a 95th-percentile annual loss estimate.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
