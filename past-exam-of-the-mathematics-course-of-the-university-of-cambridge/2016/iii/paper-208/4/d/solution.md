<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use $v=\sigma^2$ as the [variance](../../../../../../variance-split.md) parameter, with prior density relative to $d\mu\,dv$. Let $\bar x=n^{-1}\sum x_i$ and $S=\sum(x_i-\bar x)^2$. Multiplying the prior by the [likelihood function](../../../../../../likelihood-function.md) gives the unnormalized [Bayesian posterior](../../../../../../bayesian-posterior.md)

$$
\boxed{\pi(\mu,v\mid x)\propto v^{-n/2-1}\exp\left[-\frac{S+n(\mu-\bar x)^2}{2v}\right],\qquad v>0.}
$$

The printed request for an “improper posterior” should not be read as a claim that this posterior is always improper. Although the prior is improper, integrating over $\mu$ gives a marginal kernel $v^{-(n+1)/2}e^{-S/(2v)}$, which is integrable exactly when $n>1$ and $S>0$. Under these usual nondegenerate-data conditions it is a proper posterior. If those conditions fail, the displayed kernel is improper and there is no posterior probability distribution for a sampler to target.

Completing the square and using the [inverse-gamma distribution](../../../../../../inverse-gamma-distribution.md) give the full conditionals

$$
\boxed{\mu\mid v,x\sim N(\bar x,v/n),\qquad v\mid\mu,x\sim\operatorname{IG}\left(\frac n2,\frac{S+n(\mu-\bar x)^2}{2}\right).}
$$

The [inverse-gamma distribution](../../../../../../inverse-gamma-distribution.md) convention is density proportional to $v^{-\alpha-1}e^{-\beta/v}$. Equivalently the precision satisfies

$$
\boxed{\tau=1/v\mid\mu,x\sim\operatorname{Gamma}\left(\frac n2,\frac{S+n(\mu-\bar x)^2}{2}\right),}
$$

using shape and rate, as in the question.

A [Gibbs sampler](../../../../../../gibbs-sampler.md) starts from $v^{(0)}>0$ and alternates

$$
\mu^{(k+1)}\sim N(\bar x,v^{(k)}/n),\qquad
\tau^{(k+1)}\sim\operatorname{Gamma}\left(n/2,\tfrac12\sum_i(x_i-\mu^{(k+1)})^2\right),\qquad
v^{(k+1)}=1/\tau^{(k+1)}.
$$

This is the [normal mean-variance posterior with a log-uniform variance prior](../../../../../../normal-mean-variance-posterior-with-a-log-uniform-variance-prior.md). For a marginal check, $v\mid x\sim\operatorname{IG}((n-1)/2,S/2)$: integrating out $\mu$ reduces the shape by $1/2$. This marginal shape is different from the full-conditional shape $n/2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
