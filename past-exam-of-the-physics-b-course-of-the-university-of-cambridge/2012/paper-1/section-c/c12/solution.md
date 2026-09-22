<h1 id="section-c/c12/solution">Solution</h1>

↑ **Parent:** [C12](../c12.md)

Measure $\theta$ from the upward vertical, let $\mathbf e_3$ point from the support along the [symmetry](../../../../../symmetry-physics.md) axis, and use the support as the reference point for all [moments of inertia](../../../../../moment-of-inertia.md). Choose $\mathbf e_2=(\widehat{\mathbf z}-\cos\theta\mathbf e_3)/\sin\theta$ and $\mathbf e_1=\mathbf e_2\times\mathbf e_3$. These form an instantaneous principal-axis frame; its transverse axes need not spin with marks painted on the body. The three infinitesimal [Euler angles](../../../../../euler-angles.md) rotations add as vectors:

$$
\boldsymbol\omega=\dot\theta\mathbf e_1+\dot\phi\widehat{\mathbf z}+\dot\chi\mathbf e_3.
$$

Resolving the vertical direction gives

$$
\boxed{\boldsymbol\omega=(\dot\theta,\dot\phi\sin\theta,\dot\phi\cos\theta+\dot\chi),\qquad
\mathbf J=(I_1\dot\theta,I_1\dot\phi\sin\theta,I_3[\dot\phi\cos\theta+\dot\chi]).}
$$

A convention matters here: in genuinely material-fixed transverse axes, the first two components are rotated by the spin angle $\chi$. For one conventional choice they are $\dot\theta\cos\chi+\dot\phi\sin\theta\sin\chi$ and $-\dot\theta\sin\chi+\dot\phi\sin\theta\cos\chi$. Since $I_1=I_2$, that rotation changes neither [kinetic energy](../../../../../kinetic-energy.md) nor the axial and vertical conserved momenta. The simplified displayed components use the instantaneous transverse frame just defined.[§3.5.2, angular-velocity decomposition and body-frame components; §3.6, symmetric-top conserved momenta](../../../../../classical-dynamics-by-david-tong/the-motion-of-rigid-bodies.md)

For a frictionless fixed support, the support does no work and gravity is conservative, so the total [energy](../../../../../energy-split.md) is constant. The [heavy symmetric top Lagrangian](../../../../../heavy-symmetric-top-lagrangian.md) is

$$
\mathcal L=\frac{I_1}{2}(\dot\theta^2+\dot\phi^2\sin^2\theta)
+\frac{I_3}{2}(\dot\chi+\dot\phi\cos\theta)^2-mgh\cos\theta.
$$

The two [cyclic coordinates](../../../../../cyclic-coordinate.md) $\chi,\phi$ give

$$
p_\chi=J_3=I_3(\dot\chi+\dot\phi\cos\theta),\qquad
p_\phi=J_z=I_1\dot\phi\sin^2\theta+J_3\cos\theta.
$$

Equivalently, gravitational [torque](../../../../../torque.md) has no component along the vertical or [symmetry](../../../../../symmetry-physics.md) axis. Eliminate $\dot\phi=(J_z-J_3\cos\theta)/(I_1\sin^2\theta)$ and the axial spin from $E=T+V$:

$$
\boxed{E=\frac{I_1}{2}\dot\theta^2+U_{\rm eff}(\theta),\qquad
U_{\rm eff}=\frac{(J_z-J_3\cos\theta)^2}{2I_1\sin^2\theta}
+mgh\cos\theta+\frac{J_3^2}{2I_3}.}
$$

This is the [heavy symmetric top reduction](../../../../../heavy-symmetric-top-reduction.md) at fixed $J_3,J_z$. A constant inclination must satisfy the reduced [equation of motion](../../../../../equation-of-motion.md) $I_1\ddot\theta=-U_{\rm eff}'$, not merely have zero instantaneous [velocity](../../../../../velocity.md). Differentiation at fixed conserved momenta gives, for $0<\theta<\pi$ and $\Omega=\dot\phi$,

$$
U_{\rm eff}'=\sin\theta\,[J_3\Omega-I_1\Omega^2\cos\theta-mgh].
$$

Therefore [uniform precession of a heavy symmetric top](../../../../../uniform-precession-of-a-heavy-symmetric-top.md) requires

$$
\boxed{I_1\cos\theta\,\Omega^2-J_3\Omega+mgh=0.}
$$

For a prescribed upward inclination $0<\theta<\pi/2$, real [precession](../../../../../precession.md) rates exist only if the quadratic [discriminant](../../../../../discriminant.md) is nonnegative:

$$
\Omega_\pm=\frac{J_3\pm\sqrt{J_3^2-4I_1mgh\cos\theta}}{2I_1\cos\theta},\qquad
\boxed{|J_3|_{\min}(\theta)=2\sqrt{I_1mgh\cos\theta}.}
$$

For positive spin the absolute-value sign can be dropped. The two roots are the slow and fast branches and coalesce at the threshold. The familiar upright-limit critical magnitude is $2\sqrt{I_1mgh}$; strict inequality gives [gyroscopic stabilization of an inverted symmetric top](../../../../../gyroscopic-stabilization-of-an-inverted-symmetric-top.md). This limiting stability condition should not be confused with a positive minimum over every possible inclination. As $\theta$ approaches $\pi/2$ from below, the fixed-inclination threshold approaches zero. At the horizontal angle $\Omega=mgh/J_3$ for $J_3\ne0$; below the horizontal the quadratic admits real solutions even at $J_3=0$. The stated minimum therefore needs the inclination convention made explicit.

## ↑ Ancestors (14)

1. [C12](../c12.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
