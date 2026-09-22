<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a bound orbit let $E<0$ be the specific energy and $L$ the specific angular momentum. Introduce the dimensionless radius suggested in the question,

$$
x=-\frac{\mu}{b\Phi(r)}
=\frac{b+\sqrt{b^2+r^2}}b,
\qquad
r^2=b^2x(x-2).
$$

The radial energy equation becomes

$$
\dot x^2
=\frac{-2E(x-x_-)(x_+-x)}{b^2(x-1)^2},
$$

where $x_-$ and $x_+$ are the two [turning points](../../../../../../turning-point.md). Comparing coefficients gives

$$
x_-+x_+=2-\frac{\mu}{bE}.
$$

The time from periapsis to apoapsis is

$$
\begin{aligned}
\frac{T_r}{2}
&=\frac b{\sqrt{-2E}}
\int_{x_-}^{x_+}
\frac{x-1}{\sqrt{(x-x_-)(x_+-x)}}\,dx\\
&=\frac{\pi b}{\sqrt{-2E}}
\left(\frac{x_-+x_+}{2}-1\right)
=\frac{\pi\mu}{(-2E)^{3/2}}.
\end{aligned}
$$

Thus the radial [orbital period](../../../../../../orbital-period.md) is

$$
\boxed{T_r=\frac{2\pi GM}{(-2E)^{3/2}}}.
$$

It depends on $E$ but not on $L$, which is the defining isochrone property.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
