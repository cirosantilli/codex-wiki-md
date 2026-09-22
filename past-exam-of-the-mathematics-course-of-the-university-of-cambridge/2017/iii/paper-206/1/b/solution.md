<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed known $r>0$, take the [natural parameter of an exponential family](../../../../../../natural-parameter-of-an-exponential-family.md)

$$
\theta=\log\frac{\lambda}{r+\lambda}<0,\qquad b(\theta)=-r\log(1-e^\theta).
$$

The [negative binomial distribution](../../../../../../negative-binomial-distribution.md) has [log-likelihood](../../../../../../log-likelihood.md)

$$
\log f(y)=y\theta-b(\theta)+\log\Gamma(y+r)-\log\Gamma(r)-\log\Gamma(y+1).
$$

Thus this is a [negative binomial exponential family](../../../../../../negative-binomial-exponential-family.md), with [dispersion parameter](../../../../../../dispersion-parameter.md) $\phi=1$ in the convention of part (a). The carrier contains the [Gamma function](../../../../../../gamma-function.md) and depends on the fixed size $r$, which need not be an integer. Differentiating the [cumulant function of an exponential family](../../../../../../cumulant-function-of-an-exponential-family.md) gives

$$
b'(\theta)=\frac{re^\theta}{1-e^\theta}=\lambda,\qquad b''(\theta)=\frac{re^\theta}{(1-e^\theta)^2}=\lambda+\frac{\lambda^2}{r}.
$$

Therefore

$$
\boxed{\mathbb E Y=\lambda,\qquad \operatorname{Var}(Y)=\lambda+\lambda^2/r.}
$$

The size $r$ controls [overdispersion](../../../../../../overdispersion.md) relative to a [Poisson distribution](../../../../../../poisson-distribution.md); it is different from the unit [dispersion parameter](../../../../../../dispersion-parameter.md) used by this fixed-size [generalized linear model](../../../../../../generalized-linear-model.md). Another common convention applies to the scaled response $Z=Y/r$: then $b(\theta)=-\log(1-e^\theta)$ and $\phi=1/r$. Keeping track of the response scale prevents confusing these two representations. At $\lambda=0$ the law is concentrated at zero and is obtained as a boundary limit, rather than by a finite [natural parameter of an exponential family](../../../../../../natural-parameter-of-an-exponential-family.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
