<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a sufficiently smooth function, [Taylor expansion](../../../../../../taylor-expansion.md) of the four neighboring values gives

$$
\Delta_hu=\Delta u+\frac{h^2}{12}(u_{xxxx}+u_{yyyy})+O(h^4).
$$

The reaction term $\lambda u$ is sampled exactly at the grid point. On an exact solution, therefore,

$$
\boxed{(\Delta_h+\lambda)u
=\frac{h^2}{12}(u_{xxxx}+u_{yyyy})+O(h^4).}
$$

The method has **second-order local accuracy for the [partial differential equation](../../../../../../partial-differential-equation-split.md)**. The original printed equations multiply this expression by $h^2$, so their unscaled residual is $O(h^4)$; that scaling does not make the [Laplacian](../../../../../../laplacian.md) approximation fourth order. Resonance and inverse-matrix bounds are separate issues from this local truncation calculation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
