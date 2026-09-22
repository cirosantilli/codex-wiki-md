<h1 id="3c/solution">Solution</h1>

↑ **Parent:** [3C](../3c.md)

For a differentiable scalar function and a differentiable curve, the multivariable [chain rule](../../../../../chain-rule.md) is

$$
\boxed{\frac{d}{dt}f(x(t),y(t))=f_x\frac{dx}{dt}+f_y\frac{dy}{dt}.}
$$

Let $L=x\partial_x-2y\partial_y$. Choose $u=\alpha(x)y$ to be an invariant of the [method of characteristics](../../../../../method-of-characteristics.md). Then $Lu=y\{x\alpha'(x)-2\alpha(x)\}$, so $x\alpha'=2\alpha$ and a convenient choice is **$\alpha(x)=x^2$**. For $v=y/x$, the [chain rule](../../../../../chain-rule.md) gives $Lv=-3v$. Thus, writing the unknown in the new coordinates,

$$
Lf=(Lu)f_u+(Lv)f_v=-3v f_v=6f.
$$

Integrating with $u$ fixed yields

$$
\boxed{f=v^{-2}F(u)=\frac{x^2}{y^2}F(x^2y),\qquad xy\ne0,}
$$

where $F$ is an arbitrary differentiable function on the relevant interval. This gives all local solutions on each patch where the specified change of variables is invertible: its [Jacobian determinant](../../../../../jacobian-determinant.md) is $\partial(u,v)/\partial(x,y)=3y$.

The axes need care because $v$ is undefined at $x=0$ and the Jacobian vanishes at $y=0$. Reparameterizing $F(u)=u^2G(u)$ gives the simpler chart expression

$$
\boxed{f(x,y)=x^6G(x^2y)\quad(x\ne0).}
$$

It is the general solution on either component $x>0$ or $x<0$, including $y=0$ when $G$ is differentiable there. Indeed $(x,u=x^2y)$ is a nonsingular [coordinate chart](../../../../../manifold-chart.md) for $x\ne0$, and the [weighted Euler first-order equation](../../../../../weighted-euler-first-order-equation.md) reduces to $x\partial_xf|_u=6f$.

For a patch crossing $x=0$ with $y\ne0$, the characteristic invariant $w=x\sqrt{|y|}$ instead gives $f=|y|^{-3}K(w)$, with an arbitrary differentiable function on each sign component of $y$. These chart descriptions must agree on overlaps. On the axes the original equation gives $f(x,0)=C_\pm x^6$ and $f(0,y)=D_\pm|y|^{-3}$ on their separate components; a solution defined smoothly through the origin must have $f(0,0)=0$ and compatible smooth limits, in particular $D_\pm=0$. No boundary data select a particular arbitrary function.

## ↑ Ancestors (10)

1. [3C](../3c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
