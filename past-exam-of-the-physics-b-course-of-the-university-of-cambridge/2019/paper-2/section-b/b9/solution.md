<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

**Inertia is a [tensor](../../../../../tensor.md).** For a [rigid body](../../../../../rigid-body-dynamics-split.md), distances between material points are fixed. Write each position relative to the [centre of mass](../../../../../center-of-mass.md) as $\mathbf r$, so its rotational [velocity](../../../../../velocity.md) is $\boldsymbol\omega\times\mathbf r$. Integrating $\mathbf r\times(\boldsymbol\omega\times\mathbf r)$ gives [angular momentum](../../../../../angular-momentum.md)

$$
L_i=I_{ij}\omega_j,\qquad
I_{ij}=\int(r^2\delta_{ij}-r_ir_j)\,dm.
$$

The [rotational kinetic energy](../../../../../rotational-kinetic-energy.md) is

$$
T_{\mathrm{rot}}=\frac12\boldsymbol\omega\cdot\mathbf I\boldsymbol\omega.
$$

The [inertia tensor](../../../../../inertia-tensor.md) is real and symmetric, so [orthogonal](../../../../../orthogonal-vectors.md) [principal axes](../../../../../principal-axis.md) diagonalize it. [Angular momentum](../../../../../angular-momentum.md) is parallel to [angular velocity](../../../../../angular-velocity.md) only along a [principal axis](../../../../../principal-axis.md), or within a subspace of equal principal moments. For translation plus [rotation](../../../../../rotation-mathematics.md) about the [centre of mass](../../../../../center-of-mass.md), $T=Mv_{\mathrm{CM}}^2/2+T_{\mathrm{rot}}$. Moving the reference to a parallel axis adds $M(d^2\mathbf1-\mathbf d\mathbf d^{\mathsf T})$ to the [tensor](../../../../../tensor.md), the [tensor](../../../../../tensor.md) form of the parallel-axis theorem.

**Euler's equations.** The external [torque](../../../../../torque.md) about the [centre of mass](../../../../../center-of-mass.md) obeys $\boldsymbol\tau=(d\mathbf L/dt)_{\mathrm{space}}$. In body axes, the transport rule gives

$$
\boldsymbol\tau=\left(\frac{d\mathbf L}{dt}\right)_{\mathrm{body}}+\boldsymbol\omega\times\mathbf L.
$$

The principal moments are constant in that frame, hence

$$
\boxed{I_1\dot\omega_1+(I_3-I_2)\omega_2\omega_3=\tau_1,}
$$



$$
I_2\dot\omega_2+(I_1-I_3)\omega_3\omega_1=\tau_2,\qquad
I_3\dot\omega_3+(I_2-I_1)\omega_1\omega_2=\tau_3.
$$

These are [Euler's equations](../../../../../euler-s-equations-rigid-body-dynamics.md). With zero [torque](../../../../../torque.md), spatial [angular momentum](../../../../../angular-momentum.md) and [kinetic energy](../../../../../kinetic-energy.md) are conserved, although the body components generally vary. For distinct moments, small perturbations about [rotation](../../../../../rotation-mathematics.md) around the largest or smallest principal moment oscillate, whereas those about the intermediate moment grow. This is the intermediate-axis instability.

**A lamina.** Choose the lamina's plane as $z=0$. Then $I_{xz}=I_{yz}=0$, so the normal is a [principal axis](../../../../../principal-axis.md), and

$$
\boxed{I_z=\int(x^2+y^2)dm=I_x+I_y.}
$$

This perpendicular-axis theorem applies to a planar [mass](../../../../../mass.md) distribution; it is not a general identity for a three-dimensional body. Rotate the in-plane axes to diagonalize the remaining symmetric two-by-two block. For a uniform rectangular lamina with sides $a,b$ and [mass](../../../../../mass.md) $M$, its central principal moments are $I_x=Mb^2/12$, $I_y=Ma^2/12$ and $I_z=M(a^2+b^2)/12$. If $a>b$, then $I_x<I_y<I_z$: torque-free [rotation](../../../../../rotation-mathematics.md) about the long in-plane axis or the normal is stable, while that about the short in-plane axis is unstable. Coincident moments in a square require the degenerate, rather than strict intermediate-axis, case. Under a constraint to rotate only about the normal, the motion reduces to the scalar equation $\tau_z=I_z\dot\omega_z$.

**A [symmetric top](../../../../../symmetric-top.md) without [torque](../../../../../torque.md).** Let $I_1=I_2=I_\perp$ and $I_3=I_\parallel$. Euler's equations reduce to

$$
\dot\omega_3=0,\qquad
\dot\omega_1=-\nu\omega_2,\qquad
\dot\omega_2=\nu\omega_1,
\qquad \nu=\frac{I_\parallel-I_\perp}{I_\perp}\omega_3.
$$

Thus $\omega_1+i\omega_2$ rotates at signed body-frame [frequency](../../../../../frequency.md) $\nu$, while the axial component stays fixed. The symmetry axis has constant angle to fixed spatial [angular momentum](../../../../../angular-momentum.md). Indeed $\mathbf L=I_\perp\boldsymbol\omega+(I_\parallel-I_\perp)\omega_3\mathbf e_3$, so

$$
\dot{\mathbf e}_3=\boldsymbol\omega\times\mathbf e_3
=\frac{\mathbf L}{I_\perp}\times\mathbf e_3.
$$

It precesses in space about $\mathbf L$ with angular speed $L/I_\perp$. This spatial [precession](../../../../../precession.md) and the body-frame [frequency](../../../../../frequency.md) $\nu$ describe different motions and should not be identified.

**A heavy top.** If a [symmetric top](../../../../../symmetric-top.md) is pivoted a distance $\ell$ from its [centre of mass](../../../../../center-of-mass.md), gravity gives [torque](../../../../../torque.md) $\mathbf r_{\mathrm{CM}}\times M\mathbf g$. Here the relevant moments are about the fixed pivot. The axial [angular momentum](../../../../../angular-momentum.md) and the vertical angular-momentum component are conserved, because gravity supplies neither an axial [torque](../../../../../torque.md) nor a [torque](../../../../../torque.md) about the vertical. Using tilt $\theta$, [precession](../../../../../precession.md) angle $\phi$ and [spin](../../../../../spin.md) angle $\psi$, its [Lagrangian](../../../../../lagrangian.md) is

$$
\mathcal L=\frac12I_\perp(\dot\theta^2+\dot\phi^2\sin^2\theta)
+\frac12I_\parallel(\dot\psi+\dot\phi\cos\theta)^2-Mg\ell\cos\theta.
$$

Eliminating the two conserved cyclic momenta leaves one-dimensional motion in an effective tilt potential; bounded oscillation in tilt is [nutation](../../../../../nutation.md). Steady [precession](../../../../../precession.md) at $\dot\phi=\Omega$ and fixed tilt satisfies

$$
I_\perp\Omega^2\cos\theta-L_3\Omega+Mg\ell=0.
$$

For a rapidly spinning top on the slow branch, the first term is small and

$$
\boxed{\Omega\simeq\frac{Mg\ell}{L_3}=\frac{Mg\ell}{I_\parallel\omega_3}.}
$$

Gravity then changes the direction of [angular momentum](../../../../../angular-momentum.md) rather than simply tipping the top straight down. The approximation fails near conditions where [nutation](../../../../../nutation.md) or the fast-precession branch matters; the full equations retain those possibilities.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
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
