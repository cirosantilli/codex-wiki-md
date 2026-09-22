<h1 id="12/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $c=\cos\phi$ and $s=\sin\phi$. The needed coefficient [derivatives](../../../../../derivative.md) are $c_x=s^2/r$, $s_x=-sc/r$, $c_y=-sc/r$ and $s_y=c^2/r$. Apply the [product rule](../../../../../product-rule.md) to both terms of $f_x=cg_r-(s/r)g_\phi$ and use the [chain rule](../../../../../chain-rule.md) for the [derivatives](../../../../../derivative.md) of $g$. Collecting terms gives

$$
\boxed{f_{xx}=c^2g_{rr}-\frac{2sc}{r}g_{r\phi}+\frac{2sc}{r^2}g_\phi
+\frac{s^2}{r}g_r+\frac{s^2}{r^2}g_{\phi\phi}.}
$$

Similarly, differentiating $f_y=sg_r+(c/r)g_\phi$ gives

$$
\boxed{f_{yy}=s^2g_{rr}+\frac{2sc}{r}g_{r\phi}-\frac{2sc}{r^2}g_\phi
+\frac{c^2}{r}g_r+\frac{c^2}{r^2}g_{\phi\phi}.}
$$

On addition, both the mixed [partial derivative](../../../../../partial-derivative.md) terms and the first angular [derivative](../../../../../derivative.md) terms cancel. Using $s^2+c^2=1$, the [Laplacian](../../../../../laplacian.md) in [polar coordinates](../../../../../polar-coordinates.md) is

$$
\boxed{\nabla^2f=g_{rr}+\frac1r g_r+\frac1{r^2}g_{\phi\phi},\qquad r>0.}
$$

## ↑ Ancestors (13)

1. [D](../d.md)
2. [12](../../12.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
