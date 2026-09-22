<h1 id="36d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the constant density $\rho_0$,

$$
m(r)=4\pi\int_0^r\rho_0s^2\,ds
=\frac{4\pi}{3}\rho_0r^3.
$$

The definition of $m$ then gives

$$
\frac1{\mu^2}=1-\frac{2m(r)}r
=1-\frac{8\pi}{3}\rho_0r^2.
$$

Substitution in the [Tolman–Oppenheimer–Volkoff equation](../../../../../../tolman-oppenheimer-volkoff-equation.md) yields

$$
\boxed{
\frac{dP}{dr}
=-\frac{4\pi r}
{1-\frac{8\pi}{3}\rho_0r^2}
\left(P+\frac{\rho_0}{3}\right)(P+\rho_0).}
$$

The minus sign follows both from the stated TOV equation and from the outward decrease of pressure; a version of the requested intermediate formula without that sign is a typographical error.

Set

$$
a=\frac{8\pi\rho_0}{3}.
$$

Separating variables gives

$$
\frac{dP}{(P+\rho_0/3)(P+\rho_0)}
=-\frac{4\pi r\,dr}{1-ar^2}.
$$

Since

$$
\frac1{(P+\rho_0/3)(P+\rho_0)}
=\frac{3}{2\rho_0}
\left(\frac1{P+\rho_0/3}-\frac1{P+\rho_0}\right),
$$

integration and the surface condition $P(R)=0$ give

$$
\frac{P(r)+\rho_0/3}{P(r)+\rho_0}
=\frac13
\sqrt{\frac{1-ar^2}{1-aR^2}}.
$$

Writing

$$
M=m(R)=\frac{4\pi}{3}\rho_0R^3,
\qquad
a=\frac{2M}{R^3},
$$

one obtains the pressure of the [Interior Schwarzschild metric](../../../../../../interior-schwarzschild-metric.md):

$$
P(r)=\rho_0
\frac{\sqrt{1-2Mr^2/R^3}-\sqrt{1-2M/R}}
{3\sqrt{1-2M/R}-\sqrt{1-2Mr^2/R^3}}.
$$

In particular, the [central pressure of a constant-density relativistic star](../../../../../../central-pressure-of-a-constant-density-relativistic-star.md) is

$$
P(0)=\rho_0
\frac{1-\sqrt{1-2M/R}}
{3\sqrt{1-2M/R}-1}.
$$

It diverges when

$$
3\sqrt{1-\frac{2M}{R}}=1,
$$

or equivalently

$$
\boxed{M=\frac{4R}{9}.}
$$

This is the limiting equality case of [Buchdahl's theorem](../../../../../../buchdahl-s-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [36D](../../36d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
