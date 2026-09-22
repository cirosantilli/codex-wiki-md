<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

For $X=x$, the last flip must be the $r$th head. Among the preceding $x+r-1$ flips, exactly $x$ are tails and $r-1$ are heads. There are $\binom{x+r-1}{x}$ choices for their positions, and every resulting sequence has probability $(1-p)^x p^r$. The [negative binomial stopping argument](../../../../../negative-binomial-stopping-argument.md) therefore gives

$$
\boxed{\mathbb P(X=x)=\binom{x+r-1}{x}(1-p)^x p^r},
\qquad x=0,1,\ldots,
$$

so $X$ has the failures-before-the-$r$th-success [negative binomial distribution](../../../../../negative-binomial-distribution.md).

To put the mass function into [exponential family](../../../../../exponential-family-split.md) form, set

$$
\theta=\log(1-p),
\qquad -\infty<\theta<0.
$$

Since $p=1-e^\theta$,

$$
\mathbb P_\theta(X=x)
=\binom{x+r-1}{x}
 \exp\!\left\{\theta x+r\log(1-e^\theta)\right\}
=h(x)\exp\{\theta T(x)-A(\theta)\},
$$

where

$$
\boxed{T(x)=x},
\qquad
\boxed{A(\theta)=-r\log(1-e^\theta)},
\qquad
h(x)=\binom{x+r-1}{x}.
$$

Thus the [natural parameter of an exponential family](../../../../../natural-parameter-of-an-exponential-family.md) is $\theta$, and the [Fisher-Neyman factorization theorem](../../../../../fisher-neyman-factorization-theorem.md) shows that $T(X)=X$ is a [sufficient statistic](../../../../../sufficient-statistic.md). This is the [negative binomial exponential family](../../../../../negative-binomial-exponential-family.md).

The [exponential-family derivative identities](../../../../../exponential-family-derivative-identities.md) now give

$$
\mathbb E[X]=A'(\theta)
=\frac{r e^\theta}{1-e^\theta}
=\boxed{\frac{r(1-p)}p}
$$

and

$$
\operatorname{var}(X)=A''(\theta)
=\frac{r e^\theta}{(1-e^\theta)^2}
=\boxed{\frac{r(1-p)}{p^2}}.
$$

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
