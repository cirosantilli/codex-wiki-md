<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In [polar coordinates](../../../../../../../polar-coordinates.md), set

$$
u(x,y)=\left(\log\frac1{\sqrt{x^2+y^2}}\right)^{1/4}
$$

away from the origin, assigning any value at the origin. This is unbounded as $r=\sqrt{x^2+y^2}\downarrow0$. It belongs to $L^2(U)$ because

$$
\int_0^{1/2}r\left(\log\frac1r\right)^{1/2},dr<\infty.
$$

Moreover

$$
|\nabla u|^2=\frac1{16r^2}\left(\log\frac1r\right)^{-3/2},
$$

and hence

$$
\int_U|\nabla u|^2
=\frac{\pi}{8}\int_0^{1/2}\frac{dr}{r(\log(1/r))^{3/2}}<\infty.
$$

**Thus $u\in H^1(U)$ but $u\notin L^\infty(U)$, exhibiting the [failure of first-order Sobolev embedding into Linfinity in two dimensions](../../../../../../../failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions.md).**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
