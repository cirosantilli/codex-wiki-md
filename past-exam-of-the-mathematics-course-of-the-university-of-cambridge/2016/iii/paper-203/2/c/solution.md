<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Compare the hull with the empty hull and the filled unit half-disc $J=\{z\in\mathbb H:|z|\leq1\}$. Their [mapping-out functions of compact H-hulls](../../../../../../mapping-out-function-of-a-compact-h-hull.md) are $g_\varnothing(z)=z$ and $g_J(z)=z+1/z$, the latter also giving the [half-plane capacity of a half-disc](../../../../../../half-plane-capacity-of-a-half-disc.md).

Use one [planar Brownian motion](../../../../../../planar-brownian-motion.md) started at $iy$, with $y>1$. For $x>1$, exiting $\mathbb H\setminus J$ through $(x,\infty)$ entails avoiding $K$, while exiting $\mathbb H\setminus K$ through this interval entails reaching it before exit from the whole half-plane. Thus the tail [harmonic measures](../../../../../../harmonic-measure.md) satisfy

$$
p_J(y,x)\leq p_K(y,x)\leq p_\varnothing(y,x).
$$

For any of these fixed hulls $L$, the [Poisson kernel for the upper half-plane](../../../../../../poisson-kernel-for-the-upper-half-plane.md) gives the exact tail formula

$$
p_L(y,x)=\frac12-\frac1\pi
\arctan\!\frac{g_L(x)-\operatorname{Re}g_L(iy)}{\operatorname{Im}g_L(iy)}
=\frac12-\frac{g_L(x)}{\pi y}+o(y^{-1}).
$$

Subtract from $1/2$, multiply by $\pi y$, and take the limit. The inequalities reverse, yielding **the real boundary bounds**:

$$
\boxed{x\leq g_K(x)\leq x+\frac1x\qquad(x>1).}
$$

Applying this result to the reflected hull $-\overline K$ also gives

$$
x+\frac1x\leq g_K(x)\leq x\qquad(x<-1).
$$

The comparison is of Brownian exit events, so it does not assume that arbitrary conformal maps are pointwise ordered by domain inclusion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
