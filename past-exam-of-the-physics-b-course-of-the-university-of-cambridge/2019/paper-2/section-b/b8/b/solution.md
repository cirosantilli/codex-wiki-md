<h1 id="section-b/b8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a slender [elastic beam](../../../../../../elastic-beam.md) undergoing small bending, cross-sections remain approximately plane and perpendicular to the centreline. At distance $z$ from the [neutral axis](../../../../../../neutral-axis.md), longitudinal [strain](../../../../../../strain.md) is $\epsilon_{xx}=-z\kappa$, where $\kappa$ is [curvature](../../../../../../curvature.md). [Linear elasticity](../../../../../../linear-elasticity.md) gives $\sigma_{xx}=E\epsilon_{xx}$, so the [bending moment](../../../../../../bending-moment.md) has magnitude

$$
M=EI\kappa,\qquad I=\int_A z^2\,dA.
$$

Here $I$ is the second moment of cross-sectional [area](../../../../../../surface-area.md), not a [mass](../../../../../../mass.md) [moment of inertia](../../../../../../moment-of-inertia.md). For width $b$ and depth $h$ in the bending direction, $I=bh^3/12$. The cubic depth dependence explains why a deep beam resists bending more effectively than the same material spread sideways.

For a uniform beam with transverse [displacement](../../../../../../displacement.md) $y(x)$, $\kappa\simeq y''$ and bending [energy](../../../../../../energy-split.md) is $\tfrac12\int EI(y'')^2dx$. Balancing transverse load $q(x)$ yields the [Euler-Bernoulli beam equation](../../../../../../euler-bernoulli-beam-equation.md) $EIy''''=q$ under a consistent sign convention. Supports specify values of deflection, slope, moment or shear; the equation alone does not fix the response.

Now apply a compressive end load $P>0$. A small deflection shortens the axial projection by $\tfrac12\int(y')^2dx$, so the total [potential energy](../../../../../../potential-energy.md) relative to the straight configuration is

$$
\Pi[y]=\frac12\int_0^\ell\left[EI(y'')^2-P(y')^2\right]dx.
$$

Its stationary equation is

$$
EIy''''+Py''=0.
$$

For pinned ends, $y(0)=y(\ell)=0$ and the end moments vanish, so $y''(0)=y''(\ell)=0$. The candidate shapes $y=A\sin(n\pi x/\ell)$ require $P=EI(n\pi/\ell)^2$. The first loss of stability is consequently

$$
\boxed{P_{\mathrm{cr}}=\frac{\pi^2EI}{\ell^2}\quad\text{for a pinned–pinned strut}.}
$$

At smaller $P$, the quadratic [energy](../../../../../../energy-split.md) is positive; beyond this threshold the straight configuration no longer minimizes it. End restraint changes the threshold: clamped–clamped gives $4\pi^2EI/\ell^2$ and clamped–free gives $\pi^2EI/(4\ell^2)$, equivalently an effective-length correction. A column buckles in the direction of smaller flexural rigidity. Euler buckling is a geometric instability within elastic response; yielding or crushing can occur first for a short thick strut. Large deflections, shear deformation and imperfections require refinements of the ideal slender-beam model.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
