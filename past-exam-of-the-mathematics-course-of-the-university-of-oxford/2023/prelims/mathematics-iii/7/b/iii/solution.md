<h1 id="7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [central limit theorem](../../../../../../../central-limit-theorem.md) gives

$$
\frac Yn\ \mathrel{\dot\sim}\ N\!\left(\frac1\theta,\frac1{n\theta^2}\right),\qquad
\sqrt n\left(\frac{\theta Y}n-1\right)\ \mathrel{\dot\sim}\ N(0,1).
$$

Write $z=z_{1-\alpha/2}$ for the indicated [standard normal quantile](../../../../../../../standard-normal-quantile.md). Inverting the approximate [pivot](../../../../../../../pivotal-quantity.md) inequality and substituting $Y/n=1/\hat\theta$ gives the approximate [confidence interval](../../../../../../../confidence-interval.md)

$$
\boxed{\left[\hat\theta\left(1-\frac z{\sqrt n}\right),\quad
\hat\theta\left(1+\frac z{\sqrt n}\right)\right]\cap(0,\infty).}
$$

Its coverage is approximately $1-\alpha$ for large $n$. The intersection respects the positive rate parameter; asymptotically the lower endpoint is positive. This is an asymptotic interval, not an exact finite-sample [confidence interval](../../../../../../../confidence-interval.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
