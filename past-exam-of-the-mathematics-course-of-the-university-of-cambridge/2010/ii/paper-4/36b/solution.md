<h1 id="36b/solution">Solution</h1>

↑ **Parent:** [36B](../36b.md)

A photon follows a [null geodesic](../../../../../null-geodesic.md), so the parameter called proper time in the question must instead be an [affine parameter](../../../../../affine-parameter.md): proper time is identically zero on a null worldline. Denote this parameter by $\tau$ for [continuity](../../../../../continuous-function.md) with the displayed formulas.

The [geodesic](../../../../../geodesic.md) [Lagrangian](../../../../../lagrangian.md) in the equatorial plane is $\tfrac12(-F\dot t^2+F^{-1}\dot r^2+r^2\dot\phi^2)$. The cyclic coordinates give conserved quantities $E=F\dot t$ and $h=r^2\dot\phi$, proportional to the energy measured at infinity and angular momentum. The null constraint then gives

$$
\boxed{\dot r^2=E^2-\frac{h^2F}{r^2}.}
$$

The overall scale depends on the [affine parameter](../../../../../affine-parameter.md), while $b=h/E$ is the invariant impact parameter. For $u=1/r$, we have $\dot r=-h\,du/d\phi$, giving

$$
\boxed{(u')^2=b^{-2}-u^2+r_su^3.}
$$

At zeroth order choose the direction of the orbit so that $u_0=\sin\phi/b$. Then $r\sin\phi=b$, a straight line at distance $b$ from the origin. Differentiating the orbit equation gives $u''+u=\tfrac32r_su^2$. To first order,

$$
u=\frac{\sin\phi}{b}
+\frac{r_s}{4b^2}(3+\cos2\phi)
$$

solves this equation; the homogeneous first-order correction can be absorbed into the choice of asymptotic direction and impact parameter. It also satisfies the first integral to this order: the terms $2u_0'u_1'+2u_0u_1-u_0^3$ cancel.

Near the incoming asymptote its zero is at $\phi=-r_s/b+O(r_s^2/b^2)$, and near the outgoing asymptote at $\phi=\pi+r_s/b+O(r_s^2/b^2)$. Thus the excess angular change over a straight trajectory is

$$
\boxed{\Delta\phi=\frac{2r_s}{b}=\frac{4GM}{c^2b}}
$$

to first order. Solar light-deflection measurements and [gravitational lensing](../../../../../gravitational-lensing.md) provide observational evidence for this effect. The perturbation requires $r_s/b\ll1$.

## ↑ Ancestors (10)

1. [36B](../36b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
