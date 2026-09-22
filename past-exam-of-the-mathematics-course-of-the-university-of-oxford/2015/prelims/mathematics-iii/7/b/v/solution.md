<h1 id="7/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Apply the [central limit theorem](../../../../../../../central-limit-theorem.md) to the [independent and identically distributed random variables](../../../../../../../independent-and-identically-distributed-random-variables.md) $X_i^2$, whose [mean](../../../../../../../expected-value-split.md) and [variance](../../../../../../../variance-split.md) are $\theta$ and $\theta^2$. It gives the approximate [standard normal distribution](../../../../../../../standard-normal-distribution.md)

$$
\frac{\sqrt n(\widehat\theta-\theta)}{\theta}\ \approx\ N(0,1).
$$

The supplied [standard normal quantile](../../../../../../../standard-normal-quantile.md) $c=1.96$ leaves [probability](../../../../../../../probability.md) $0.025$ in each tail. Hence

$$
\mathbb P\left(-1.96<\frac{\sqrt n(\widehat\theta-\theta)}{\theta}<1.96\right)\approx0.95.
$$

Since $\theta>0$, this event is equivalent to

$$
\theta\left(1-\frac{1.96}{\sqrt n}\right)<\widehat\theta<\theta\left(1+\frac{1.96}{\sqrt n}\right).
$$

For $n>1.96^2$, equivalently integer $n\geq4$, both denominators below are positive. Inverting the inequalities gives the approximate $95\%$ [confidence interval](../../../../../../../confidence-interval.md)

$$
\boxed{\left(\frac{\widehat\theta}{1+1.96/\sqrt n},\ \frac{\widehat\theta}{1-1.96/\sqrt n}\right),\qquad c=1.96.}
$$

The approximation is justified for large $n$; positivity at $n\geq4$ by itself does not guarantee accurate coverage. This construction is a [confidence interval from a relative normal pivot](../../../../../../../confidence-interval-from-a-relative-normal-pivot.md): the unknown scale remains inside the pivotal ratio until the inequalities are inverted. Its meaning is that the random interval covers the fixed [statistical parameter](../../../../../../../statistical-parameter.md) $\theta$ with [probability](../../../../../../../probability.md) approximately $0.95$ under repeated sampling.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
