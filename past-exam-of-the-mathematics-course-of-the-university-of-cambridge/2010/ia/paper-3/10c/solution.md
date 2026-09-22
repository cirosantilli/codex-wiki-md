<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

For a one-to-one continuously differentiable change of variables with nonzero [Jacobian determinant](../../../../../jacobian-determinant.md) in the interior, the [change of variables formula](../../../../../change-of-variables-formula.md) is

$$
\int_R f(x,y)\,dx\,dy=\int_{\widetilde R}f(x(u,v),y(u,v))\left|\det\frac{\partial(x,y)}{\partial(u,v)}\right|du\,dv.
$$

The absolute value is necessary even if the transformation reverses orientation.

The original region is the first-quadrant area between the hyperbola and circle, above the horizontal-axis segment. More explicitly,

$$
0\leq y\leq\frac1{\sqrt2},\qquad \sqrt{1+y^2}\leq x\leq\sqrt{2-y^2}.
$$

Its vertices are $(1,0)$, $(\sqrt2,0)$ and $(\sqrt{3/2},1/\sqrt2)$. Under the [squared-radius difference substitution](../../../../../squared-radius-difference-substitution.md), the inverse is

$$
x=\sqrt{\frac{u+v}{2}},\qquad y=\sqrt{\frac{u-v}{2}},
$$

and the image is the triangle $1\leq v\leq u\leq2$, with vertices $(1,1),(2,1),(2,2)$.

<a id="10c/image-circular-hyperbolic-integration-region-and-its-triangular-image"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-3-change-of-variables.png)

**[Figure 2](#10c/image-circular-hyperbolic-integration-region-and-its-triangular-image). Circular-hyperbolic integration region and its triangular image**.

The forward [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\det\begin{pmatrix}2x&2y\\2x&-2y\end{pmatrix}=-8xy.
$$

It is nonzero in the interior; the zero on $y=0$ lies on a measure-zero boundary, so the integral formula applies by taking interior limits. Since $x^5y-xy^5=xyuv$ and $4x^2y^2=u^2-v^2$, the inverse-Jacobian factor cancels $xy$, giving

$$
I=\frac18\int_1^2\int_1^u uv\,e^{u^2-v^2}\,dv\,du.
$$

Integrating in $v$ first and then $u$,

$$
I=\frac1{16}\int_1^2u\bigl(e^{u^2-1}-1\bigr)\,du=\frac1{32}(e^3-1)-\frac3{32}.
$$

Therefore

$$
\boxed{I=\frac{e^3-4}{32}.}
$$

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
