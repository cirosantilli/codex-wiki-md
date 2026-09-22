<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Interpret polynomial reproduction as a guarantee for every [polynomial](../../../../../../polynomial-split.md) of degree at most $d$, with the planar grid coordinates fixed by the affine-exact refinement. Constants are unchanged because every stencil sums to one. Linear height functions are unchanged because each stencil's weighted position is its refined grid location. Therefore the [Loop subdivision](../../../../../../loop-subdivision-surface.md) limit reproduces all affine polynomials exactly.

Quadratic data already disprove the next degree. Use extruded data $g_j=j^2$ on a unit-spaced transverse row coordinate $y$. At spacing $h$, both even and odd rules from the induced [subdivision mask](../../../../../../subdivision-mask.md) give the value of $y^2$ at the refined location plus $h^2/4$. For the even stencil this follows from

$$
\frac{(y-h)^2+6y^2+(y+h)^2}{8}=y^2+\frac{h^2}4,
$$

and for the odd stencil from the average of the values at $y-h/2$ and $y+h/2$. Constants are reproduced, so the accumulated vertical displacement over all refinement levels is

$$
\sum_{\ell=0}^\infty\frac{4^{-\ell}}4=\frac13.
$$

The limit is $y^2+1/3$, not the original quadratic graph. Hence

$$
\boxed{d_{\rm exact}=1.}
$$

The word “every” matters: some special higher-degree bivariate polynomials have cancelling second moments and can be reproduced. The conclusion concerns the entire polynomial space, which already fails at degree two.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
