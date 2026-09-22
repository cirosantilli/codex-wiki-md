<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

For a one-to-one differentiable change of variables $(x,y)\mapsto(u,v)$, the [change of variables formula](../../../../../change-of-variables-formula.md) is

$$
\iint_D f(x,y)\,dx\,dy
=\iint_{D'}f(x(u,v),y(u,v))
\left|\frac{\partial(x,y)}{\partial(u,v)}\right|\,du\,dv,
$$

where

$$
\left|\frac{\partial(x,y)}{\partial(u,v)}\right|
=\frac1{\left|u_xv_y-u_yv_x\right|}.
$$

Here $u=x+y$, $v=x^2+y^2$, and

$$
\frac{\partial(u,v)}{\partial(x,y)}=2(y-x).
$$

At fixed $v$, write $x=\sqrt v\cos\theta$, $y=\sqrt v\sin\theta$ with $0\leq\theta\leq\pi$. Then $u=\sqrt v(\cos\theta+\sin\theta)$, so

$$
D'=\{(u,v):0\leq v\leq1,\ -\sqrt v\leq u\leq\sqrt{2v}\}.
$$

The constant-$v$ curves are semicircles and the constant-$u$ curves are lines $x+y=u$.

The map is two-to-one where $\sqrt v<u<\sqrt{2v}$, because both $(x,y)$ and $(y,x)$ lie in the upper half-disc, and one-to-one elsewhere. Since $|y-x|=\sqrt{2v-u^2}$, accounting for this multiplicity gives

$$
\begin{aligned}
I
&=\int_0^1\left[
\int_{-\sqrt v}^{\sqrt v}\frac{u\,du}{2\sqrt{2v-u^2}}
+2\int_{\sqrt v}^{\sqrt{2v}}\frac{u\,du}{2\sqrt{2v-u^2}}
\right]dv\\
&=\int_0^1\sqrt v\,dv
=\boxed{\frac23}.
\end{aligned}
$$

Directly, symmetry makes $\iint_Dx\,dA=0$, while [polar coordinates](../../../../../polar-coordinates.md) give $\iint_Dy\,dA=\int_0^1r^2dr\int_0^\pi\sin\theta\,d\theta=2/3$.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
