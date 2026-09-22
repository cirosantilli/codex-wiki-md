<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

Set $U=X/(X+Y)$ and $V=X+Y$. Their inverse [change of variables](../../../../../change-of-variables-formula.md) is $X=UV$, $Y=(1-U)V$, with domain $0<U<1$, $V>0$. The absolute [Jacobian determinant](../../../../../jacobian-determinant.md) of this inverse transformation is

$$
\left|\det\begin{pmatrix}v&u\\-v&1-u\end{pmatrix}\right|=v.
$$

Use the [independence of random variables](../../../../../independent-random-variables.md) to multiply the two original [Gamma distribution](../../../../../gamma-distribution.md) densities. The [change of variables formula](../../../../../change-of-variables-formula.md) then gives the [joint probability density](../../../../../joint-probability-density.md)

$$
f_{U,V}(u,v)=\frac{\theta^{n+m}}{(n-1)!(m-1)!}\,u^{n-1}(1-u)^{m-1}v^{n+m-1}e^{-\theta v},\qquad 0<u<1,\ v>0.
$$

Factor this into two normalized densities:

$$
f_{U,V}(u,v)=\left[\frac{(n+m-1)!}{(n-1)!(m-1)!}u^{n-1}(1-u)^{m-1}\right]\left[\frac{\theta^{n+m}}{(n+m-1)!}v^{n+m-1}e^{-\theta v}\right].
$$

The support is a product domain, and the factors are precisely a [Beta distribution](../../../../../beta-distribution.md) density and a [Gamma distribution](../../../../../gamma-distribution.md) density. Therefore

$$
\boxed{U\sim B(n,m),\qquad V\sim\Gamma(n+m,\theta),\qquad U\text{ and }V\text{ independent}.}
$$

This [beta-gamma independence](../../../../../beta-gamma-independence.md) uses the common rate $\theta$; it is a rate parameter, not the scale parameter $1/\theta$.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
