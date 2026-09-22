<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The common-age [conditional probabilities](../../../../../../conditional-probability.md) give

$$
p_{GG}=\int_0^1g^2dy=\frac1{24300},\qquad p_{GW}=\int_0^1 2gw\,dy=\frac{18}{24300},\qquad p_{WW}=\int_0^1 w^2dy=\frac{81}{24300}.
$$

Here $GW$ includes both possible component orders. Hence the [binary star](../../../../../../binary-star.md) fractions have the concise ratio

$$
\boxed{GG:GW:WW=1:18:81.}
$$

As a check on the role of shared age, $p_{GG}=4p_G^2/3$ rather than $p_G^2$. This is [covariance induced by a shared latent variable](../../../../../../covariance-induced-by-a-shared-latent-variable.md): the [red giant](../../../../../../red-giant.md) [indicator random variables](../../../../../../indicator-random-variable.md) have [covariance](../../../../../../covariance.md) equal to the [variance](../../../../../../variance-split.md) of $g(Y)$, namely $1/97200$.

For a [starburst galaxy](../../../../../../starburst-galaxy.md) with age $t$, put $y_b=t/(10\,\mathrm{Gyr})$. There is no age averaging. The component masses remain independent, so the fraction of systems with two [red giants](../../../../../../red-giant.md) is

$$
\boxed{p_{GG}^{\rm burst}=g(y_b)^2=\frac{(t/\mathrm{Gyr})^2}{810000},\qquad 0<t<10\,\mathrm{Gyr}.}
$$

The last comparison is ambiguous in the printed question. Literally, the fraction of individual [red giants](../../../../../../red-giant.md) in the first [galaxy](../../../../../../galaxy-split.md) is $1/180$. Since $p_{GG}^{\rm burst}<1/8100<1/180$, **no allowed starburst age satisfies that literal comparison**. If the intended comparison is instead between systems containing two [red giants](../../../../../../red-giant.md) in the two [galaxies](../../../../../../galaxy-split.md), compare with $p_{GG}=1/24300$; the answer is

$$
\boxed{\frac{10}{\sqrt3}\,\mathrm{Gyr}<t<10\,\mathrm{Gyr}\quad\text{for the two-giant-system comparison}.}
$$

For completeness, the individual [red giant](../../../../../../red-giant.md) fraction in the burst is $g(y_b)=t/(900\,\mathrm{Gyr})$, which exceeds $1/180$ precisely for $5\,\mathrm{Gyr}<t<10\,\mathrm{Gyr}$. This is a third, different comparison; it does not change the computed fraction of two-giant systems.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 322](../../../paper-322-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
