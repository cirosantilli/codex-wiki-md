<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $s=\sum_{j=1}^n x_j$. The conditional joint [likelihood function](../../../../../../likelihood-function.md) of the observed counts is

$$
L(\theta;\mathbf x)=\prod_{j=1}^n\frac{e^{-\theta}\theta^{x_j}}{x_j!}
=\frac{e^{-n\theta}\theta^s}{\prod_jx_j!}.
$$

The [prior](../../../../../../prior-probability.md) is a [gamma distribution](../../../../../../gamma-distribution.md) with shape two and rate $\lambda$. Multiplication by its density gives the unnormalized [posterior density](../../../../../../posterior-density.md) $\theta^{s+1}e^{-(n+\lambda)\theta}$. Normalizing with the [gamma function](../../../../../../gamma-function.md) yields

$$
\pi(\theta\mid\mathbf x)=\frac{(n+\lambda)^{s+2}}{\Gamma(s+2)}
\theta^{s+1}e^{-(n+\lambda)\theta},\qquad\theta>0.
$$

Thus [Poisson-gamma conjugacy](../../../../../../poisson-gamma-conjugacy.md) gives $\Theta\mid\mathbf x\sim\operatorname{Gamma}(s+2,n+\lambda)$. Conditional on $\Theta$ and the past data, the next count has mean $\Theta$, so the [law of total expectation](../../../../../../law-of-total-expectation.md) gives

$$
\boxed{\mathbb E[X_{n+1}\mid\mathbf x]=\mathbb E[\Theta\mid\mathbf x]=\frac{s+2}{n+\lambda}.}
$$

With $\overline x=s/n$ and [prior](../../../../../../prior-probability.md) mean $m_0=2/\lambda$, this is exactly

$$
\boxed{\frac{s+2}{n+\lambda}
=Z\overline x+(1-Z)m_0,\qquad Z=\frac n{n+\lambda}.}
$$

Here $n\geq1$, $\lambda>0$, and the [credibility factor](../../../../../../credibility-factor.md) increases to one as the number of observed years grows. The denominator uses the [prior](../../../../../../prior-probability.md) rate $\lambda$ and total exposure $n$; it does not add two to the exposure when adding the [prior](../../../../../../prior-probability.md) shape.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
