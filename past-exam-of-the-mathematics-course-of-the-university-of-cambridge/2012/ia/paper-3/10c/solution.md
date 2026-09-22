<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

For fixed $u\in(0,1)$, $x=1-u\in(0,1)$ and

$$
\frac{\partial y}{\partial v}=-\frac{1-u}{(1-uv)^2}<0.
$$

As $v$ runs from zero to one, $y$ decreases continuously from one to zero. Thus the map is onto the open unit square and is one-to-one, with smooth inverse

$$
u=1-x,\qquad v=\frac{1-y}{1-(1-x)y}.
$$

Its denominator is positive in the open square. This is a [rational square diffeomorphism](../../../../../rational-square-diffeomorphism.md). Its [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\frac{\partial(x,y)}{\partial(u,v)}
=(-1)\left(-\frac{1-u}{(1-uv)^2}\right)
=\frac{x}{(1-uv)^2}.
$$

Writing $A=1-(1-x)y$, the inverse relation gives $1-uv=x/A$. Consequently

$$
\boxed{\frac{\partial(x,y)}{\partial(u,v)}=\frac{A^2}{x}.}
$$

The second transformation also maps the open unit square bijectively onto the open unit square: for fixed $w$, $u=(1-t)/(1-wt)$ decreases strictly from one to zero as $t$ goes from zero to one, while $v=1-w$ independently spans $(0,1)$. Its positive [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\frac{\partial(u,v)}{\partial(t,w)}=\frac{1-w}{(1-wt)^2}.
$$

To express this in $x,y$, the composite transformation gives $y=w/[x+(1-x)w]$ and $x=t(1-w)/(1-wt)$. Put $B=1-(1-x^2)y$. Solving these relations gives

$$
w=\frac{xy}{A},\qquad t=\frac{xA}{B},\qquad
1-w=\frac{1-y}{A},\qquad1-wt=\frac{1-y}{B}.
$$

The [chain rule](../../../../../chain-rule.md) for [Jacobian determinants](../../../../../jacobian-determinant.md) therefore gives

$$
\boxed{\frac{\partial(x,y)}{\partial(t,w)}
=\frac{A^2}{x}\frac{B^2}{A(1-y)}
=\frac{AB^2}{x(1-y)}.}
$$

The requested integrand is exactly the reciprocal of this positive determinant. Apply the [change of variables formula](../../../../../change-of-variables-formula.md) using the composite [diffeomorphism](../../../../../diffeomorphism.md):

$$
\boxed{\int_R\frac{x(1-y)}{[1-(1-x)y][1-(1-x^2)y]^2}\,dx\,dy
=\int_0^1\int_0^1 1\,dt\,dw=1.}
$$

Possible singular behavior at the square's boundary does not invalidate the calculation: first integrate over the images of compact interior squares, where all transformations are smooth with nonzero [Jacobian determinant](../../../../../jacobian-determinant.md), and then increase these domains to the full square. Positivity and [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) justify this limit.

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
