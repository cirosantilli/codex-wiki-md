<h1 id="12c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [canonical momenta](../../../../../../canonical-momentum.md) are $p_x=m\dot x$, $p_y=m\dot y+qBx$, $p_z=m\dot z$. The [Legendre transform in mechanics](../../../../../../legendre-transform-in-mechanics.md) gives

$$
\boxed{H=\frac{p_x^2+(p_y-qBx)^2+p_z^2}{2m}+qEy.}
$$

[Hamilton's equations](../../../../../../hamilton-s-equations.md) are

$$
\dot x=p_x/m,\quad\dot y=(p_y-qBx)/m,\quad\dot z=p_z/m,\qquad\dot p_x=qB\dot y,\quad\dot p_y=-qE,\quad\dot p_z=0.
$$

Thus $\ddot x=\Omega\dot y$, $\ddot y=-\Omega\dot x-qE/m$, and $\ddot z=0$, where $\Omega=qB/m$. The signs also follow from $\mathbf E=-E\mathbf e_y$ and $\mathbf B=B\mathbf e_z$.

For $Bq\ne0$, put $v_d=-E/B$, $a=v_{x0}-v_d$, $b=v_{y0}$. The motion is

$$
\boxed{\begin{aligned}x(t)&=x_0+v_dt+\frac{a\sin\Omega t+b(1-\cos\Omega t)}\Omega,\\y(t)&=y_0+\frac{a(\cos\Omega t-1)+b\sin\Omega t}\Omega,\\z(t)&=z_0+v_{z0}t.\end{aligned}}
$$

Differentiation verifies both equations and all initial conditions. The centre of the circular motion has the [electric drift](../../../../../../electric-drift-in-crossed-uniform-fields.md) [velocity](../../../../../../velocity.md) $-E\mathbf e_x/B$. For $B=0$, take $x=x_0+v_{x0}t$, $y=y_0+v_{y0}t-qEt^2/(2m)$ and the same $z$. For $q=0$, the particle moves freely.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12C](../../12c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
