<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

The [laplace transform](../../../../../laplace-transform.md) is $\widehat f(p)=\int_0^\infty e^{-pt}f(t),dt$, and inversion is

$$
f(t)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}e^{pt}\widehat f(p),dp,
$$

where the vertical [Bromwich contour](../../../../../bromwich-contour.md) lies to the right of all singularities. For $t>0$ it is closed leftwards, and for $t<0$ rightwards, where the exponential decays.

Transforming the PDE and imposing boundedness as $x\to\infty$ gives

$$
U(x,p)=\frac1{p(p+1)}+\frac{p-1}{p(p+1)}e^{-x\sqrt{p/D}},
$$

with the square root cut conventionally along $(-\infty,0]$. Therefore

$$
u(x,t)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}e^{pt}U(x,p),dp.
$$

There are poles at $p=0,-1$ (with cancellation assessed in the complete expression) and a [branch point](../../../../../branch-point.md) at $0$; close left for $t>0$ and wrap the cut while including the relevant residues.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
