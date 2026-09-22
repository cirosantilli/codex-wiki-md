<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the upward direction as $\mathbf e_z$, with polar angle $\theta$ measured from it. The liquid is quiescent at infinity. On a translating clean inviscid bubble, the [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) is $(\mathbf u-U\mathbf e_z)\cdot\mathbf n=0$, and the [stress-free boundary condition](../../../../../../stress-free-boundary-condition.md) is zero tangential traction. The normal traction must balance uniform gas [pressure](../../../../../../pressure.md) and any constant-curvature surface-tension jump.

For a vertical [Stokeslet](../../../../../../stokeslet.md) of strength $F$, the radial [velocity](../../../../../../velocity.md) is $u_r=F\cos\theta/(4\pi\mu r)$. Its traction on a concentric [sphere](../../../../../../sphere.md) is purely normal, so zero tangential traction is automatic. The kinematic condition at $r=a$ gives

$$
\boxed{F=4\pi\mu aU.}
$$

The singularity is only a device for generating the exterior solution; there is no liquid point [force](../../../../../../force.md) inside the actual bubble. The integrated dynamic traction on the bubble is $-F\mathbf e_z$, giving the [clean-bubble Stokes drag](../../../../../../clean-bubble-stokes-drag.md). The upward [buoyancy](../../../../../../buoyancy.md) is $4\pi\rho ga^3/3$, hence [force](../../../../../../force.md) balance gives

$$
\boxed{U=\frac{\rho ga^2}{3\mu}.}
$$

The normal stress also shows that [surface tension](../../../../../../surface-tension.md) is not required for this particular spherical solution. Let the ambient [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) at the bubble centre be $p_c$, so on its surface $p_h=p_c-\rho ga\cos\theta$. Adding the Stokeslet's dynamic normal traction gives

$$
\sigma_{nn}^{\rm total}=-p_c+
\left(\rho ga-\frac{3F}{4\pi a^2}\right)\cos\theta=-p_c,
$$

where the terminal [buoyancy](../../../../../../buoyancy.md) value of $F$ cancels the dipole. This is the [spherical clean bubble without surface tension](../../../../../../spherical-clean-bubble-without-surface-tension.md) balance: **an initially spherical bubble can remain spherical in this ideal steady Stokes solution even when [surface tension](../../../../../../surface-tension.md) is zero**. With uniform [surface tension](../../../../../../surface-tension.md) $\gamma$, choose gas [pressure](../../../../../../pressure.md) $p_b=p_c+2\gamma/a$; with $\gamma=0$, $p_b=p_c$. This proves compatibility of the spherical shape, not stability of arbitrary deformations or validity when inertia matters.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
