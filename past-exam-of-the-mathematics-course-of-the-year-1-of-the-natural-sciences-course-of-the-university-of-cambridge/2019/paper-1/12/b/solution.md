<h1 id="12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Integrate by horizontal slices. At a fixed height $0\le z\le H$, the parabolic boundary gives $|x|\le L\sqrt{z/H}$; the other inequality gives $|y|\le b(2-z/H)$. Thus the cross-section is a rectangle of [area](../../../../../surface-area.md)

$$
A(z)=4Lb\sqrt{\frac zH}\left(2-\frac zH\right).
$$

The [volume integral](../../../../../volume-integral.md), followed by [integration by substitution](../../../../../integration-by-substitution.md) $u=z/H$, is

$$
\begin{aligned}
V_{\rm bank}&=\int_0^H A(z)\,dz
=4LbH\int_0^1(2u^{1/2}-u^{3/2})\,du\\
&=4LbH\left(\frac43-\frac25\right)
=\boxed{\frac{56}{15}LbH.}
\end{aligned}
$$

This has units of [volume](../../../../../volume.md). As a check on the geometry, the width decreases with height while the length of the horizontal slice increases from zero to $2L$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
