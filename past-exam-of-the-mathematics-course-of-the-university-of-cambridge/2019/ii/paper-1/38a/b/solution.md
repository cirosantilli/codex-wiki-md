<h1 id="38a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Away from the rim's $O(h)$ edge region, the geometry and uniform injection have no radial scale other than the factor required by continuity. It is therefore consistent to take $w=w(z)$. Regularity at $r=0$ then lets the continuity equation integrate to

$$
u(r,z)=-\frac r2w'(z).
$$

The [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) and prescribed normal velocities are

$$
w(0)=V,\quad w'(0)=0,\qquad
w(h)=0,\quad w'(h)=0.
$$

Since $p$ is independent of $z$, the radial equation implies that $w'''$ is constant. The four boundary conditions give

$$
w(z)=V\left[1-3\left(\frac zh\right)^2+2\left(\frac zh\right)^3\right],
$$

and hence

$$
u(r,z)=\frac{3Vr}{h}\frac zh\left(1-\frac zh\right).
$$

Using $w'''=12V/h^3$ in $p_r=\mu u_{zz}$ gives

$$
p_r=-\frac{6\mu Vr}{h^3}.
$$

Taking the pressure at the rim to be atmospheric, $p(R)=p_0$, produces the [porous-plate lubrication cushion](../../../../../../porous-plate-lubrication-cushion.md) pressure

$$
\boxed{p(r)-p_0=\frac{3\mu V}{h^3}(R^2-r^2).}
$$

The upward pressure force balances the disc's weight:

$$
W=\int_0^R[p(r)-p_0],2\pi r\,dr
=\frac{3\pi\mu VR^4}{2h^3}.
$$

Since $\varepsilon=h/R$,

$$
\boxed{W=\frac{3\pi\mu VR}{2\varepsilon^3}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38A](../../38a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
