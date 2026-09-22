<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

For a one-to-one continuously differentiable change of variables with nonzero [Jacobian determinant](../../../../../jacobian-determinant.md), the [change of variables formula](../../../../../change-of-variables-formula.md) rule is

$$
\iint_D F(x,y)\,dx\,dy
=\iint_E F(x(u,v),y(u,v))
\left|\det\frac{\partial(x,y)}{\partial(u,v)}\right|\,du\,dv,
$$

where $E$ is the transformed region and the inverse map covers $D$ once. The absolute value is required even if the coordinate map reverses orientation.

Here $x,y$ are positive. For $u=y/x$, $v=xy$, the inverse is $x=\sqrt{v/u}$ and $y=\sqrt{uv}$. On the first portion of $D$, the bounds give $v\ge1$, $u\le4$ and $v\le u$ because $x\le1$. Together these give $1\le v\le u\le4$; conversely these inequalities imply $1/2\le x\le1$ and the original bounds. On the second portion, they give $u\ge1$, $v\le4$ and $v\ge u$, hence $1\le u\le v\le4$, with the converse following similarly. The two triangles combine into the rectangle **$E=\{1\le u\le4,\ 1\le v\le4\}$**, sharing only the diagonal corresponding to $x=1$.

The Jacobian is

$$
\det\frac{\partial(u,v)}{\partial(x,y)}
=\det\begin{pmatrix}-y/x^2&1/x\\y&x\end{pmatrix}=-\frac{2y}{x}=-2u,
\qquad
\left|\det\frac{\partial(x,y)}{\partial(u,v)}\right|=\frac1{2u}.
$$

Also $xy^3=uv^2$ and $x^2+y^2=v(1+u^2)/u$. The transformed integral consequently factors:

$$
\iint_D\frac{4xy^3}{x^2+y^2}\,dx\,dy
=\int_1^4\int_1^4\frac{2uv}{1+u^2}\,dv\,du
=\left[\frac{v^2}{2}\right]_1^4
\left[\log(1+u^2)\right]_1^4.
$$

Therefore

$$
\boxed{\iint_D\frac{4xy^3}{x^2+y^2}\,dx\,dy=\frac{15}{2}\log\frac{17}{2}.}
$$

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
