<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $h=\Delta x$. A one-dimensional [Taylor expansion](../../../../../../taylor-expansion.md) gives

$$
u(x+h)-2u(x)+u(x-h)
=h^2u_{xx}(x)+\frac{h^4}{12}u_{xxxx}(x)+O(h^6).
$$

Adding the three coordinate directions shows that the exact solution has stencil defect

$$
L_hu-h^2f
=\frac{h^4}{12}(u_{x_1x_1x_1x_1}+u_{x_2x_2x_2x_2}+u_{x_3x_3x_3x_3})+O(h^6)
=O(h^4).
$$

This is the local defect of the [seven-point Dirichlet Laplacian](../../../../../../seven-point-dirichlet-laplacian.md). Its inverse has max-norm size $O(h^{-2})$: this follows from the [discrete maximum principle](../../../../../../discrete-maximum-principle.md), for example by comparison with the grid restriction of $x_1(1-x_1)+x_2(1-x_2)+x_3(1-x_3)$, whose stencil is $-6h^2$. Therefore the grid error is $O(h^2)$.

The question writes this error as $O(h^{p+1})$, so

$$
\boxed{p+1=2,\qquad p=1.}
$$

In the more usual terminology, the [finite difference method](../../../../../../finite-difference-method.md) is second-order accurate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
