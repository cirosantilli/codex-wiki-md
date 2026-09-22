<h1 id="19/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Using the same cylindrical-shell [volume](../../../../../../volume.md),

$$
\boxed{L=2\pi h\int_0^a r^2v(r)\,dr
=2\pi h\int_0^a r^3\omega(r)\,dr}.
$$

For unit [density](../../../../../../density.md), this is the axial [angular momentum](../../../../../../angular-momentum.md). To bound it, apply the integral [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) to $f(r)=\sqrt r\,v(r)$ and $g(r)=r^{3/2}$:

$$
\left(\int_0^ar^2v(r)\,dr\right)^2
\leq\left(\int_0^arv(r)^2\,dr\right)\left(\int_0^ar^3\,dr\right)
=\frac{K}{\pi h}\frac{a^4}{4}.
$$

Multiplication by $(2\pi h)^2$ gives $L^2\leq\pi ha^4K$. Since the chamber's [volume](../../../../../../volume.md) is $V=\pi a^2h$, this is precisely

$$
\boxed{K\geq\frac{L^2}{Va^2}}.
$$

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [19](../../../19.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
