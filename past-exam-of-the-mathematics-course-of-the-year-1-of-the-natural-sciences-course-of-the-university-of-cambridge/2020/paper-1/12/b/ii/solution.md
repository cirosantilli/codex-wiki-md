<h1 id="12/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In [spherical coordinates](../../../../../../spherical-coordinate-system.md), the [cone](../../../../../../cone-geometry.md) condition forces $z\ge0$ and becomes $0\le\vartheta\le\alpha$. The unit [ball](../../../../../../ball-mathematics.md) gives $0\le\rho\le1$. Hence

$$
V=\int_0^{2\pi}\int_0^\alpha\int_0^1\rho^2\sin\vartheta\,d\rho\,d\vartheta\,d\varphi
=\boxed{\frac{2\pi}{3}(1-\cos\alpha).}
$$

For an independent calculation in [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md), the lower boundary is $z=r\cot\alpha$ and the upper boundary is $z=\sqrt{1-r^2}$. They meet at $r=\sin\alpha$, since $r^2\cot^2\alpha=1-r^2$. Thus

$$
\begin{aligned}
V&=2\pi\int_0^{\sin\alpha}r\left(\sqrt{1-r^2}-r\cot\alpha\right)\,dr\\
&=\frac{2\pi}{3}\left[1-\cos^3\alpha-\sin^3\alpha\cot\alpha\right]
=\frac{2\pi}{3}(1-\cos\alpha).
\end{aligned}
$$

The equality uses $\sin^3\alpha\cot\alpha=\sin^2\alpha\cos\alpha$. The positive [cosine](../../../../../../cosine.md) on the stated range removes any square-root sign ambiguity.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [12](../../../12.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
