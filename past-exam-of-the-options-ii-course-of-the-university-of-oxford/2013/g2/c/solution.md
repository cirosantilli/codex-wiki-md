<h1 id="g2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [surface of revolution](../../../../surface-of-revolution.md) $r(\eta,\zeta)=(\eta,f(\eta)\cos\zeta,f(\eta)\sin\zeta)$, the coordinate tangent [vectors](../../../../vector.md) have squared lengths $1+f'^2$ and $f^2$, and their dot product is zero. Hence its [first fundamental form](../../../../first-fundamental-form.md) is

$$
\boxed{ds^2=A(\eta)d\eta^2+f(\eta)^2d\zeta^2,\qquad A=1+f'^2.}
$$

Use the energy [Lagrangian](../../../../lagrangian.md) $L=A\dot\eta^2+f^2\dot\zeta^2$. Its Euler-Lagrange equations are

$$
2A\ddot\eta+A'\dot\eta^2-2ff'\dot\zeta^2=0,\qquad
\frac d{dt}(2f^2\dot\zeta)=0.
$$

For a meridian $\zeta=\zeta_0$, choose arc length as parameter, so $\dot\eta=1/\sqrt A$. Differentiating gives $2A\ddot\eta+A'\dot\eta^2=0$, while the second equation is automatic. Part (b) makes this path an extremal of length. Thus **every meridian is a [geodesic](../../../../geodesic.md)**.

For a nonconstant parallel $\eta=\eta_0$, choose constant nonzero $\dot\zeta$. The second equation holds, and the first reduces to $f(\eta_0)f'(\eta_0)\dot\zeta^2=0$. Since $f>0$, this is equivalent to

$$
\boxed{f'(\eta_0)=0.}
$$

Conversely that condition makes both equations hold at constant speed, hence supplies a length extremal. Geometrically, a parallel is geodesic exactly at a stationary radius of the surface.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [G2](../../g2.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
