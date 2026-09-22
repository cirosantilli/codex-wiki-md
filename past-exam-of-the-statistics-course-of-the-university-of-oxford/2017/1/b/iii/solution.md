<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $S^2=Q/(n-1)$ and $S=\sqrt{S^2}$, with $n\geq2$. Two exact facts about a [normal sample](../../../../../normal-sample.md) are

$$
\overline X\sim N(\mu,\mu^2/n),\qquad
\frac{(n-1)S^2}{\mu^2}\sim\chi^2_{n-1},
$$

and [independence of the normal sample mean and sample variance](../../../../../independence-of-the-normal-sample-mean-and-sample-variance.md) holds. A [chi-squared distribution](../../../../../chi-squared-distribution.md) with $n-1$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) is a sum of $n-1$ [independent](../../../../../independent-random-variables.md) $\chi^2_1$ variables, each with [mean](../../../../../expected-value-split.md) one and [variance](../../../../../variance-split.md) two. The [central limit theorem](../../../../../central-limit-theorem.md) therefore gives

$$
\sqrt{n-1}(S^2-\mu^2)\xrightarrow dN(0,2\mu^4).
$$

For $g(x)=\sqrt x$, the [derivative](../../../../../derivative.md) at $\mu^2$ is $1/(2\mu)$ because $\mu>0$. The [delta method](../../../../../delta-method.md) gives the [asymptotic normality of a normal sample standard deviation](../../../../../asymptotic-normality-of-a-normal-sample-standard-deviation.md):

$$
\sqrt n(S-\mu)\xrightarrow dN(0,\mu^2/2).
$$

The exact independence of $\overline X$ and $S$ makes their limiting [normal distributions](../../../../../normal-distribution.md) independent. Consequently,

$$
\sqrt n(\widetilde\mu-\mu)
=\frac13\{\sqrt n(\overline X-\mu)+2\sqrt n(S-\mu)\}
\xrightarrow dN\!\left(0,\frac19\left\{\mu^2+4\frac{\mu^2}2\right\}\right).
$$

Thus

$$
\boxed{\sqrt n(\widetilde\mu-\mu)\xrightarrow dN(0,\mu^2/3),\qquad
\widetilde\mu\mathrel{\dot\sim}N\!\left(\mu,\frac{\mu^2}{3n}\right).}
$$

This has the same leading [asymptotic variance](../../../../../asymptotic-variance.md) as $\widehat\mu$. The weights $1/3$ and $2/3$ are those in the [optimal asymptotic combination of a normal sample mean and standard deviation](../../../../../optimal-asymptotic-combination-of-a-normal-sample-mean-and-standard-deviation.md). This does not require $S$ to be an exactly [unbiased estimator](../../../../../unbiased-estimator.md) of $\mu$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
