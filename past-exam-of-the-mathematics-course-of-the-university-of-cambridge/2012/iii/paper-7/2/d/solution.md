<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [planar vorticity velocity kernel](../../../../../../planar-vorticity-velocity-kernel.md) has magnitude $(2\pi|z|)^{-1}$. Split its defining [integral](../../../../../../integral.md) into $|x-y|<R$ and $|x-y|\geq R$ for any $R>0$. The singular part is absolutely integrable in two dimensions:

$$
|U[\Omega](x)|
\leq \frac{\|\Omega\|_\infty}{2\pi}
\int_{|z|<R}\frac{dz}{|z|}
+\frac{\|\Omega\|_1}{2\pi R}
=R\|\Omega\|_\infty+\frac{\|\Omega\|_1}{2\pi R}.
$$

In particular $R=1$ proves

$$
\boxed{\|U[\Omega]\|_\infty
\leq\|\Omega\|_\infty+\frac1{2\pi}\|\Omega\|_1.}
$$

When both norms are nonzero, optimization in $R$ also gives $\|U[\Omega]\|_\infty\leq\sqrt{2/\pi}\,\|\Omega\|_1^{1/2}\|\Omega\|_\infty^{1/2}$. If either norm is zero, $\Omega=0$ almost everywhere. Absolute convergence supplies a well-defined velocity at every $x$, with these uniform bounds.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
