<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $h=\Delta x$, let $C_h$ denote the sum of the four axial shifts, and let $K_h$ denote the sum of the four diagonal shifts. Reading both sides of the PDF stencil gives $M_h\dot U=L_hU$, where $M_h=2I/3+C_h/12$ and $L_h=(-10I/3+2C_h/3+K_h/6)/h^2$. The left-hand stencil acts on the time [derivative](../../../../../../derivative.md); treating it as a scalar multiplier would lose the compact correction.

Write $D=\partial_x^2+\partial_y^2$. [Taylor expansion](../../../../../../taylor-expansion.md) of the symmetric shifts gives

$$
M_h=I+\frac{h^2}{12}D+\frac{h^4}{144}(\partial_x^4+\partial_y^4)+O(h^6),
$$

and

$$
L_h=D+\frac{h^2}{12}D^2+h^4\left[\frac{\partial_x^6+\partial_y^6}{360}
+\frac{\partial_x^4\partial_y^2+\partial_x^2\partial_y^4}{72}\right]+O(h^6).
$$

For the exact diffusion solution $u_t=Du$, subtracting gives

$$
M_hu_t-L_hu=h^4\left[\frac{u_{xxxxxx}+u_{yyyyyy}}{240}
-\frac{u_{xxxxyy}+u_{xxyyyy}}{144}\right]+O(h^6).
$$

The leading coefficient is not identically zero for general smooth data. Thus the normalized local residual is fourth order, and in the question's $h^{p+1}$ convention **$\boxed{p=3}$**. This is the [compact semidiscrete nine-point diffusion](../../../../../../compact-semidiscrete-nine-point-diffusion.md) scheme; its usual spatial [numerical consistency](../../../../../../consistency-of-a-numerical-method.md) order is four, rather than three.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
