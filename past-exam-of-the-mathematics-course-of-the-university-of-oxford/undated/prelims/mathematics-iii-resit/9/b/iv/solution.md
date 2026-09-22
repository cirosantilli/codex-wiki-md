<h1 id="9/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For each fixed $\lambda>0$, maximizing the [likelihood function](../../../../../../../likelihood-function.md) over $\mu$ is equivalent to minimizing $A(\mu)=\sum_i|x_i-\mu|$. Order the distinct observations as $x_{(1)}<\cdots<x_{(n)}$ and write $n=2m+1$. Between successive [order statistics](../../../../../../../order-statistic.md), with exactly $k$ observations to the left,

$$
A'(\mu)=k-(n-k)=2k-n.
$$

Thus $A$ decreases up to $x_{(m+1)}$ and increases after it. Its unique [minimum](../../../../../../../minimum-of-a-subset-of-a-total-order.md) is at the [sample median](../../../../../../../sample-median.md):

$$
\boxed{\widehat\mu=x_{(m+1)}.}
$$

At a fixed $\mu$ with $A(\mu)>0$, the [log-likelihood function](../../../../../../../log-likelihood.md) has [derivative](../../../../../../../derivative.md) $n/\lambda-A(\mu)$ and second [derivative](../../../../../../../derivative.md) $-n/\lambda^2<0$, so its unique maximizing rate is $n/A(\mu)$. The maximized [likelihood function](../../../../../../../likelihood-function.md) is $(n/[2eA(\mu)])^n$, which increases when $A(\mu)$ decreases. Hence the joint [maximum-likelihood estimates](../../../../../../../maximum-likelihood-estimator.md) are

$$
\boxed{\widehat\mu=x_{(m+1)},\qquad
\widehat\lambda=\frac{n}{\sum_i|x_i-x_{(m+1)}|}.}
$$

This is [Laplace location and scale maximum likelihood](../../../../../../../laplace-location-and-scale-maximum-likelihood.md), expressed with the reciprocal scale.

**A finite rate [maximum-likelihood estimate](../../../../../../../maximum-likelihood-estimator.md) requires a positive total absolute deviation.** For distinct observations and odd $n\ge3$, that condition holds. For $n=1$, however, $\mu=x_1$ gives $A(\mu)=0$ and $L=\lambda/2\to\infty$ as $\lambda\to\infty$. There is no finite joint [maximum-likelihood estimate](../../../../../../../maximum-likelihood-estimator.md) in the stated parameter space; the formula with zero denominator is not an admissible estimate.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
