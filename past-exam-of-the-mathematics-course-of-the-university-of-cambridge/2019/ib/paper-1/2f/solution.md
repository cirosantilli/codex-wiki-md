<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

A [Laurent series](../../../../../laurent-series.md) about $a$ is an expansion

$$
f(z)=\sum_{n=-\infty}^{\infty}c_n(z-a)^n
$$

that converges to $f$ on an [annulus](../../../../../annulus-mathematics.md) $r<|z-a|<R$.

The [partial fraction decomposition](../../../../../partial-fraction-decomposition.md) is

$$
\frac{10}{(z+2)(z^2+1)}
=\frac2{z+2}+\frac{4-2z}{z^2+1}.
$$

For $0<|z|<1$, expand both denominators by the [geometric series](../../../../../geometric-series.md):

$$
\boxed{f(z)=\sum_{n=0}^{\infty}\frac{(-1)^n}{2^n}z^n
+(4-2z)\sum_{k=0}^{\infty}(-1)^kz^{2k}}.
$$

This is actually a [Taylor series](../../../../../taylor-series.md) at zero, since the apparent puncture at zero contains no singularity.

For $1<|z|<2$, the $z+2$ term still expands in nonnegative powers, while the quadratic term must be expanded in negative powers:

$$
\frac{4-2z}{z^2+1}
=(4z^{-2}-2z^{-1})\frac1{1+z^{-2}}.
$$

Hence

$$
\boxed{f(z)=\sum_{n=0}^{\infty}\frac{(-1)^n}{2^n}z^n
+(4z^{-2}-2z^{-1})\sum_{k=0}^{\infty}(-1)^kz^{-2k}}.
$$

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
