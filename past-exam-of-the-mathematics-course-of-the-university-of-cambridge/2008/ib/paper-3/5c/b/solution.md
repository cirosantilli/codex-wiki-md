<h1 id="5c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the [branch of the complex logarithm](../../../../../../branch-of-the-complex-logarithm.md) with $-\pi<\arg s<\pi$ and write $s^{-1/2}=\exp[-\log s/2]$. Deform the [Bromwich contour](../../../../../../bromwich-contour.md) into a Hankel contour about the negative real axis. The small circle at zero contributes $O(r^{1/2})$ and vanishes; the large closing arcs vanish by the exponential estimates for $t>0$. On the upper lip $s=-r+i0$, $s^{-1/2}=-i/\sqrt r$, while on the lower lip it is $i/\sqrt r$. Keeping the lip orientations in the [Bromwich inversion with a square-root branch cut](../../../../../../bromwich-inversion-with-a-square-root-branch-cut.md) gives

$$
f(t)=\frac1{2\pi i}\int_0^\infty e^{-rt}\left(\frac{i}{\sqrt r}-\frac{-i}{\sqrt r}\right)dr
=\frac1\pi\int_0^\infty r^{-1/2}e^{-rt}dr.
$$

With $r=u^2$, the supplied [Gaussian integral](../../../../../../gaussian-integral.md) evaluates this as $2\pi^{-1}\int_0^\infty e^{-tu^2}du$. Hence

$$
\boxed{\mathcal L^{-1}[s^{-1/2}](t)=\frac1{\sqrt{\pi t}}\quad(t>0).}
$$

The inverse is singular but locally integrable at zero, which is compatible with existence of its [Laplace transform](../../../../../../laplace-transform.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5C](../../5c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
