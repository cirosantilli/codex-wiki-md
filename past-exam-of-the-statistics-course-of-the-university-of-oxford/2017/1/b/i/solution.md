<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $A=\sum_i x_i$, $B=\sum_i x_i^2$ and $M_2=B/n$. The [normal distribution](../../../../../normal-distribution.md) model gives

$$
L(\mu)=(2\pi)^{-n/2}\mu^{-n}\exp\!\left\{-\frac{B-2\mu A+n\mu^2}{2\mu^2}\right\},\qquad\mu>0,
$$

and, up to a constant independent of $\mu$, its [log-likelihood function](../../../../../log-likelihood.md) is

$$
\ell(\mu)=-n\log\mu-\frac{B}{2\mu^2}+\frac A\mu.
$$

The [score function](../../../../../informant-function.md) and its zero equation are

$$
\ell'(\mu)=\frac{B-A\mu-n\mu^2}{\mu^3},\qquad
n\mu^2+A\mu-B=0.
$$

For $B>0$, this [quadratic equation](../../../../../quadratic-equation.md) has exactly one positive root, giving the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md)

$$
\boxed{\widehat\mu=\frac{-A+\sqrt{A^2+4nB}}{2n}
=\frac{-\overline X+\sqrt{\overline X^{\,2}+4M_2}}2.}
$$

The numerator $B-A\mu-n\mu^2$ of the [score function](../../../../../informant-function.md) is positive between its negative and positive roots and negative above its positive root. Thus the [likelihood function](../../../../../likelihood-function.md) increases up to $\widehat\mu$ and decreases afterwards: this is its unique global maximum on $(0,\infty)$. Also, $\ell(\mu)\to-\infty$ at both ends. The all-zero observation vector has [probability](../../../../../probability.md) zero; on that exceptional vector $L(\mu)\propto\mu^{-n}$ and there is no attained maximum.

The second [derivative](../../../../../derivative.md) and the relevant [moments](../../../../../moment.md) are

$$
\ell''(\mu)=\frac n{\mu^2}-\frac{3B}{\mu^4}+\frac{2A}{\mu^3},\qquad
\mathbb E_\mu A=n\mu,\qquad
\mathbb E_\mu B=n(\mu^2+\mu^2)=2n\mu^2.
$$

Therefore the expected [Fisher information](../../../../../fisher-information-matrix.md) is

$$
I_n(\mu)=-\mathbb E_\mu\ell''(\mu)=\frac{3n}{\mu^2}.
$$

The [support of a probability distribution](../../../../../support-of-a-probability-distribution.md) is the whole [real line](../../../../../real-line.md), independent of the positive [statistical parameter](../../../../../statistical-parameter.md). The [law of large numbers](../../../../../law-of-large-numbers.md) gives $\overline X\to\mu$ and $M_2\to2\mu^2$ in [probability](../../../../../probability.md), so the displayed [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is a [consistent estimator](../../../../../consistency-statistics.md). The regular [asymptotic normality of a maximum likelihood estimator](../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) now yields

$$
\boxed{\sqrt n(\widehat\mu-\mu)\xrightarrow dN(0,\mu^2/3),\qquad
\widehat\mu\mathrel{\dot\sim}N\!\left(\mu,\frac{\mu^2}{3n}\right).}
$$

Thus the requested leading [asymptotic variance](../../../../../asymptotic-variance.md) on the unscaled estimator's scale is $\mu^2/(3n)$. The [normal mean proportional to standard deviation model](../../../../../normal-mean-proportional-to-standard-deviation-model.md) provides a reusable version of this calculation.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
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
