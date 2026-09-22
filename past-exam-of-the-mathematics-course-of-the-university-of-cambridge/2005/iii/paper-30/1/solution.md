<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $X=1+T$ and $Y=X^p-1$, so that $\phi(f)=f(Y)$. The essential integrality statement for the [Frobenius substitution on cyclotomic power series](../../../../../frobenius-substitution-on-cyclotomic-power-series.md) is the decomposition into a [finite free module](../../../../../finite-free-module.md):

$$
R=\bigoplus_{i=0}^{p-1}X^i\phi(R).
$$

To prove it, reduce modulo $p$. Since $Y\equiv T^p$, grouping the coefficients of a [formal power series](../../../../../formal-power-series.md) according to their exponents modulo $p$ gives the unique expression $\sum_{j=0}^{p-1}T^jh_j(T^p)$. The change from $1,T,\ldots,T^{p-1}$ to $1,X,\ldots,X^{p-1}$ is a triangular [matrix](../../../../../matrix.md) with diagonal entries $1$, so this is also a [basis](../../../../../basis.md) over $\mathbb F_p[[T^p]]$. Lift these $p$ coefficient series to $R$, subtract their contribution from $f$, divide the remaining error by $p$, and repeat. The sums of the successive lifts converge in the finer of the [topologies on integral formal power series](../../../../../topologies-on-integral-formal-power-series.md), because $R$ is complete in that topology. This proves existence of the decomposition over $R$. A relation among its summands reduces to the zero relation modulo $p$, forcing each coefficient series to be divisible by $p$. Repetition forces divisibility by every power of $p$, hence every coefficient series is zero. This proves uniqueness and, in particular, [injectivity](../../../../../injective-function.md) of $\phi$.

For $f=\sum_{i=0}^{p-1}X^i\phi(f_i)$, define

$$
\boxed{S(f)=f_0.}
$$

This is a $\mathbb Z_p$-[linear map](../../../../../linear-map.md). To calculate the average over [roots of unity](../../../../../root-of-unity.md), work over $\mathcal O=\mathbb Z_p[\zeta_p]$. The substitutions $T\mapsto\zeta X-1$ are legitimate: their constant terms are topologically nilpotent, so the defining coefficient sums converge in $\mathcal O$. Since $(\zeta X)^p=X^p$, each $\phi(f_i)$ is unchanged by the substitution. The sums of the powers of the [roots of unity](../../../../../root-of-unity.md) are $p$ for $i=0$ and zero for $1\leq i<p$. Consequently

$$
\sum_{\zeta\in\mu_p}f(\zeta X-1)=p\phi(f_0).
$$

Thus the average is integral and belongs to $\phi(R)$, and the constructed [Coleman trace operator](../../../../../coleman-trace-operator.md) has the required property. [Injectivity](../../../../../injective-function.md) of $\phi$ forces uniqueness of any map satisfying that property. Finally, the decomposition of $\phi(g)$ has $f_0=g$ and all other coefficients zero, giving **$S\circ\phi=\mathrm{id}_R$**.

We will also use the [trace](../../../../../matrix-trace.md) of multiplication by $h$ on this [finite free module](../../../../../finite-free-module.md). After extending scalars to split the conjugates, that [trace](../../../../../matrix-trace.md) is the sum just computed. Hence

$$
\operatorname{Tr}_{R/\phi(R)}(h)=p\phi(S(h)).
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
