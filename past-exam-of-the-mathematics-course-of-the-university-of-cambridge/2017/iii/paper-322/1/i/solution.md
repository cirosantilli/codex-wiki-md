<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For this [stellar population](../../../../../../stellar-population.md), let $m=M/M_\odot$ denote initial [mass](../../../../../../mass.md) in units of the [solar mass](../../../../../../solar-mass.md), and let $\tau=t/\mathrm{Gyr}$ denote present [stellar age](../../../../../../stellar-age.md). Constant formation of equal numbers of [stars](../../../../../../star.md) per unit time makes the [stellar age](../../../../../../stellar-age.md) a [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $[0,10]$ Gyr, so $Y=\tau/10$ is uniform on $[0,1]$. The normalized [initial mass function](../../../../../../initial-mass-function.md) has [probability density function](../../../../../../probability-density-function.md) $f(m)=0.1m^{-2}$ for $m>0.1$, since $\int_{0.1}^\infty m^{-2}dm=10$. Consequently

$$
\boxed{Y(t)=\frac{t}{10\,\mathrm{Gyr}},\qquad X(M)=\frac{\int_m^\infty u^{-2}du}{\int_{0.1}^\infty u^{-2}du}=\frac{0.1}{m}.}
$$

These formulae have the stated age and mass domains; outside them the relevant cumulative fractions saturate at zero or one. The [probability integral transform](../../../../../../probability-integral-transform.md) makes $X$ uniform on $[0,1]$: $m=0.1/X$ gives $f(m)|dm/dX|=1$. The time-independent [initial mass function](../../../../../../initial-mass-function.md) and constant number formation rate give [independence](../../../../../../independent-random-variables.md) of $X$ and $Y$. All fractions here count objects, including [white dwarfs](../../../../../../white-dwarf.md), using the stipulated [stellar evolution](../../../../../../stellar-evolution.md) law.

A [red giant](../../../../../../red-giant.md) has

$$
\frac9m<\tau<\frac{10}m,\qquad 0\leq\tau\leq10.
$$

Thus the [mass](../../../../../../mass.md) boundaries are $m=9/\tau$ and $m=10/\tau$ for positive $\tau$. Equivalently, for $0.9<m<1$ the [red giant](../../../../../../red-giant.md) region runs from $9/m$ to the age cap $10$, and for $m\geq1$ it runs from $9/m$ to $10/m$. There are no [red giants](../../../../../../red-giant.md) with $m\leq0.9$. Boundaries have zero [probability](../../../../../../probability.md) and their endpoint convention does not affect the fractions. In the uniform $(X,Y)$ square the [red giant](../../../../../../red-giant.md) region is $9X<Y<10X$, with [triangle](../../../../../../triangle.md) vertices $(0,0)$, $(1/10,1)$ and $(1/9,1)$. The [white dwarf](../../../../../../white-dwarf.md) region is the [triangle](../../../../../../triangle.md) $0<X<Y/10$.

<a id="1/i/image-mass-age-regions-and-their-uniform-coordinate-images"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-322-population-regions.png)

**[Figure 1](#1/i/image-mass-age-regions-and-their-uniform-coordinate-images). Mass-age regions and their uniform-coordinate images**. The right panel magnifies the evolved part of the unit square. All of the remaining region at larger X is main sequence.

At fixed $Y=y$, define the conditional [probabilities](../../../../../../probability.md) of a [red giant](../../../../../../red-giant.md), [white dwarf](../../../../../../white-dwarf.md) and [main sequence](../../../../../../main-sequence.md) star by $g(y)$, $w(y)$ and $s(y)$. Their interval widths are

$$
g(y)=\frac{y}{90},\qquad w(y)=\frac{y}{10}=9g(y),\qquad s(y)=1-\frac y9.
$$

[Integration](../../../../../../integral.md) over the [uniform distribution](../../../../../../continuous-uniform-distribution.md) of age gives the individual-star fractions

$$
\boxed{p_G=\int_0^1g(y)dy=\frac1{180},\qquad p_W=\int_0^1w(y)dy=\frac1{20}.}
$$

The systems form a [coeval binary population](../../../../../../coeval-binary-population.md): the two [binary star](../../../../../../binary-star.md) components have the same age. Their masses are independent, so $(X_1,X_2,Y)$ has uniform [probability density function](../../../../../../probability-density-function.md) on $[0,1]^3$ and their states have [conditional independence](../../../../../../conditional-independence.md) given $Y$. Unconditional independence of their states would be incorrect: older systems make both evolved states more likely. The [law of total probability](../../../../../../law-of-total-probability.md) now gives

$$
\boxed{p_{\geq1G}=\int_0^1\bigl[1-(1-g(y))^2\bigr]dy=\frac1{90}-\frac1{24300}=\frac{269}{24300}.}
$$

The subtraction removes the double counting of systems containing two [red giants](../../../../../../red-giant.md).

## ↑ Ancestors (11)

1. [I](../i.md)
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
