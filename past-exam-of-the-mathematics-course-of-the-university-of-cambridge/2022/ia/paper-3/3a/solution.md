<h1 id="3a/solution">Solution</h1>

↑ **Parent:** [3A](../3a.md)

Set

$$
u=\frac{x}{y},\qquad v=xy.
$$

Because the region lies in the [positive quadrant](../../../../../positive-quadrant.md), its four inequalities become

$$
1\leq u\leq\alpha,\qquad 1\leq v\leq\alpha.
$$

Thus this [change of variables](../../../../../change-of-variables-formula.md) sends $D$ to a rectangle in the $uv$-plane. Its [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\frac{\partial(u,v)}{\partial(x,y)}
=
\begin{vmatrix}
1/y&-x/y^2\\
y&x
\end{vmatrix}
=\frac{2x}{y}=2u,
$$

so

$$
dx\,dy=\frac{du\,dv}{2u}.
$$

Since $x^2=uv$, the [double integral](../../../../../double-integral.md) is

$$
\begin{aligned}
\iint_Dx^2\,dx\,dy
&=\int_1^\alpha\int_1^\alpha
uv\,\frac{du\,dv}{2u}\\
&=\frac12\left(\int_1^\alpha du\right)
\left(\int_1^\alpha v\,dv\right)\\
&=\boxed{\frac{(\alpha-1)(\alpha^2-1)}4}.
\end{aligned}
$$

## ↑ Ancestors (10)

1. [3A](../3a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
