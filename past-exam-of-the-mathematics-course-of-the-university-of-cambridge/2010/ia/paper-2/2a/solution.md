<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

The first-order [chain rule](../../../../../chain-rule.md), with $x,y$ regarded as functions of $u,v$, is

$$
g_u=x_uf_x+y_uf_y,\qquad g_v=x_vf_x+y_vf_y.
$$

Apply the [product rule](../../../../../product-rule.md) when differentiating the first identity in $v$, and apply the [chain rule](../../../../../chain-rule.md) to $f_x,f_y$. Equality of mixed [partial derivatives](../../../../../partial-derivative.md) for a $C^2$ function gives

$$
g_{uv}=x_ux_vf_{xx}+(x_uy_v+x_vy_u)f_{xy}
+y_uy_vf_{yy}+x_{uv}f_x+y_{uv}f_y.
$$

**Thus $\boxed{H=x_{uv},\ K=y_{uv}}$.** These terms record the second derivatives of the coordinate transformation, not of $f$.

For the given transformation,

$$
x_u=v,\quad x_v=u,\quad y_u=\frac1v,\quad y_v=-\frac u{v^2},
\quad x_{uv}=1,\quad y_{uv}=-\frac1{v^2}.
$$

The mixed-derivative coefficient is zero, while $x_ux_v=x$, $y_uy_v=-y^2/x$, and $1/v^2=y/x$. The required [partial differential equation](../../../../../partial-differential-equation-split.md) is therefore exactly $g_{uv}=0$. Integrating first in $u$ and then in $v$ on a coordinate rectangle gives

$$
\boxed{g(u,v)=A(u)+B(v),}
$$

where $A,B$ are arbitrary twice continuously differentiable functions. The [Jacobian determinant](../../../../../jacobian-determinant.md) of the transformation is $-2u/v$, so this calculation uses patches with $u,v\ne0$. On a positive-quadrant patch we can take $u=\sqrt{xy}$ and $v=\sqrt{x/y}$, obtaining

$$
\boxed{f(x,y)=A(\sqrt{xy})+B(\sqrt{x/y}).}
$$

Changing branches merely redefines the arbitrary functions.

For completeness, the original equation also makes sense in quadrants with $xy<0$, where that particular real square-root transformation is unavailable. Multiplying the equation by $x$ gives

$$
(x\partial_x)^2f-(y\partial_y)^2f=0.
$$

On any quadrant with $xy\ne0$, put $a=\log|x|$, $b=\log|y|$; then set $\xi=a+b$, $\eta=a-b$. The equation becomes $4f_{\xi\eta}=0$. Thus an equivalent general local answer on every such quadrant is

$$
\boxed{f(x,y)=\Phi(\log|xy|)+\Psi(\log|x/y|).}
$$

Here $\Phi,\Psi$ are arbitrary $C^2$ functions on the relevant intervals. If a solution is required across $y=0$, its quadrant expressions must extend with matching derivatives; on that line the equation itself imposes $xf_{xx}(x,0)+f_x(x,0)=0$, so its trace is $a_0\log|x|+b_0$ on each interval with $x\ne0$. The displayed coordinate transformations do not assert invertibility at $y=0$.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
