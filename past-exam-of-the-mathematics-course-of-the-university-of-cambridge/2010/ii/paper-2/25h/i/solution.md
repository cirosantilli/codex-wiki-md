<h1 id="25h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a regular simple closed plane curve of length $L$ enclosing area $A$, the [planar isoperimetric inequality](../../../../../../planar-isoperimetric-inequality.md) is **$L^2\geq4\pi A$**, with equality precisely for a circle.

The periodic [Wirtinger inequality](../../../../../../wirtinger-inequality.md) states that an absolutely continuous $L$-periodic function $h$ of mean zero with square-integrable derivative satisfies

$$
\int_0^L h^2\,ds\leq\left(\frac L{2\pi}\right)^2\int_0^L(h')^2\,ds,
$$

with equality only for a linear combination of $\sin(2\pi s/L)$ and $\cos(2\pi s/L)$. Parametrize the curve by [arc length](../../../../../../arc-length.md) and translate its position vector $r=(x,y)$ so that both coordinate means vanish. Then $\int|r|^2\leq L^3/(4\pi^2)$, since $|r'|=1$. [Green's theorem](../../../../../../green-theorem.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
A=\frac12\left|\int_0^L(xy'-yx')\,ds\right|
\leq\frac12\left(\int|r|^2\right)^{1/2}\left(\int|r'|^2\right)^{1/2}
\leq\frac{L^2}{4\pi}.
$$

Equality requires a first-harmonic parametrization and equality in Cauchy-Schwarz; its radius vector is a constant multiple of the rotated unit tangent. It is therefore a circle. Conversely, a circle attains equality.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [25H](../../25h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
