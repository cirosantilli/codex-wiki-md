<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Einstein tensor](../../../../einstein-tensor.md) and its contractions are

$$
G_{\mu\nu}=R_{\mu\nu}-\frac12g_{\mu\nu}R,\qquad
R_{\mu\nu}=R^\alpha{}_{\mu\alpha\nu},\qquad
R=g^{\mu\nu}R_{\mu\nu}.
$$

To match the supplied [Ricci tensor](../../../../ricci-tensor.md) components, use the [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) convention

$$
R^\rho{}_{\sigma\mu\nu}
=\partial_\nu\Gamma^\rho_{\mu\sigma}
-\partial_\mu\Gamma^\rho_{\nu\sigma}
+\Gamma^\rho_{\nu\lambda}\Gamma^\lambda_{\mu\sigma}
-\Gamma^\rho_{\mu\lambda}\Gamma^\lambda_{\nu\sigma}.
$$

This convention also fixes the sign used for [geodesic deviation](../../../../geodesic-deviation.md) above. In [vacuum](../../../../vacuum.md), tracing the [Einstein field equations](../../../../einstein-field-equations-split.md) gives $-R+4\Lambda=0$. Substitution therefore yields **$R_{\mu\nu}=\Lambda g_{\mu\nu}$**.

Differentiate the angular field equation to obtain

$$
-2A'-rA''=2\Lambda r,\qquad
\frac{A'}r+\frac{A''}2=-\Lambda.
$$

Consequently $R_{00}=\Lambda A=\Lambda g_{00}$ and $R_{11}=-\Lambda/A=\Lambda g_{11}$. The other angular component follows from $R_{33}=\sin^2\theta\,R_{22}$. Thus the single angular equation implies all the displayed [vacuum](../../../../vacuum.md) equations wherever this coordinate chart is regular.

Integrating $(rA)'=1-\Lambda r^2$ gives $A=1+C/r-\Lambda r^2/3$. Match $g_{tt}\simeq1+2\Phi$ with the [Newtonian gravitational potential](../../../../newtonian-gravitational-potential.md) $\Phi=-GM/r$ in the weak-field overlap region to identify $C=-2GM$. Hence the [Schwarzschild-de Sitter spacetime](../../../../schwarzschild-de-sitter-spacetime.md) has

$$
\boxed{A(r)=1-\frac{2GM}{r}-\frac{\Lambda r^2}{3}\quad(c=1).}
$$

Negative $\Lambda$ instead gives the [Schwarzschild--anti-de Sitter black hole](../../../../schwarzschild-anti-de-sitter-black-hole.md) case. This matching fixes the normalization locally; a spacetime with nonzero $\Lambda$ is not asymptotically flat.

For [timelike geodesics](../../../../timelike-geodesic.md) in the [orbital plane](../../../../orbital-plane.md), take [proper time](../../../../proper-time.md) as parameter and use $L=(A\dot t^2-\dot r^2/A-r^2\dot\phi^2)/2$. The [cyclic coordinates](../../../../cyclic-coordinate.md) give $A\dot t=k$ and $r^2\dot\phi=h$; the angular [canonical momentum](../../../../canonical-momentum.md) is $-h$ in this signature. The [four-velocity](../../../../four-velocity.md) normalization $2L=1$ then gives

$$
\boxed{\dot r^2=k^2-A(r)\left(1+\frac{h^2}{r^2}\right).}
$$

Here $k$ is conserved [Killing energy](../../../../killing-energy.md) per unit rest [mass](../../../../mass.md) in the chosen time normalization, and $h$ is conserved [angular momentum](../../../../angular-momentum.md) per unit rest [mass](../../../../mass.md). There is no general interpretation of $k$ as [energy](../../../../energy-split.md) measured at an asymptotically flat infinity when $\Lambda\ne0$.

For radial motion $h=0$, differentiation gives $2\dot r\ddot r=-A'\dot r$. The radial [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) extends the resulting expression through a [turning point](../../../../turning-point.md) where division by $\dot r$ would fail. Thus

$$
\boxed{\ddot r=-\frac{A'}2=-\frac{GM}{r^2}+\frac{\Lambda r}{3}\quad(c=1).}
$$

This is the proper-time second [derivative](../../../../derivative.md) of the [areal radius](../../../../areal-radius.md), not a nonzero [four-acceleration](../../../../four-acceleration.md) of the freely falling particle. Positive $\Lambda$ contributes an outward term; negative $\Lambda$ reinforces inward attraction. Restoring units in the slow-motion, weak-field [Newtonian limit](../../../../newtonian-limit.md) gives

$$
\boxed{\frac{d^2r}{dt^2}\simeq-\frac{GM}{r^2}+\frac{\Lambda c^2r}{3},\qquad
\Phi=-\frac{GM}{r}-\frac{\Lambda c^2r^2}{6}.}
$$

The extra term describes the gravitational effect of a [cosmological constant](../../../../cosmological-constant.md), not drag or a contact force. The approximation requires $GM/(rc^2)\ll1$, $|\Lambda|r^2\ll1$ and [speed](../../../../speed.md) much less than $c$.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
