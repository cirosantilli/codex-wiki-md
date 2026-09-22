<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

For torque-free [rotation](../../../../../rotation-mathematics.md), [angular momentum](../../../../../angular-momentum.md) is fixed in inertial space, but [angular velocity](../../../../../angular-velocity.md) need not point along it. In principal body axes,

$$
I_1\dot\omega_1+(I_3-I_2)\omega_2\omega_3=0
$$

and cyclic permutations. A [symmetric top](../../../../../symmetric-top.md) with transverse moment $A$ and axial moment $C$ has constant $\omega_3$, while $\omega_1+i\omega_2$ rotates in body coordinates at signed [frequency](../../../../../frequency.md) $(C-A)\omega_3/A$. The symmetry axis precesses around the fixed [angular momentum](../../../../../angular-momentum.md) in space at rate $L/A$. These body-frame and space-frame rates describe different motions and need not coincide.

**[Poinsot construction](../../../../../poinsot-s-ellipsoid.md)** expresses the same torque-free motion geometrically. The [energy](../../../../../energy-split.md) [ellipsoid](../../../../../ellipsoid.md) $\sum I_i\omega_i^2=2T$ is fixed in the body. Its normal at the angular-velocity point is parallel to $\mathbf L$, and $\mathbf L\cdot\boldsymbol\omega=2T$ places that point in a fixed plane perpendicular to $\mathbf L$. The [ellipsoid](../../../../../ellipsoid.md) rolls on this invariable plane without slipping: the instantaneous [velocity](../../../../../velocity.md) of its contact point is proportional to $\boldsymbol\omega\times\boldsymbol\omega=0$. The contact curve is the [polhode](../../../../../polhode.md) on the body [ellipsoid](../../../../../ellipsoid.md) and the [herpolhode](../../../../../herpolhode.md) on the plane.[§3.4, Euler equations, stability and Poinsot construction](../../../../../classical-dynamics-by-david-tong.md)

For $I_1<I_2<I_3$, linearization about spin $\Omega$ on the third axis gives

$$
\ddot\omega_1=-\Omega^2\frac{(I_3-I_2)(I_3-I_1)}{I_1I_2}\omega_1.
$$

The extreme-moment axes are stable; the intermediate one is unstable. The [major-axis relaxation theorem](../../../../../major-axis-relaxation-theorem.md) adds weak internal dissipation while retaining negligible external [torque](../../../../../torque.md). At fixed $L$,

$$
T=\sum_i\frac{L_i^2}{2I_i}\geq\boxed{\frac{L^2}{2I_3}.}
$$

[Energy](../../../../../energy-split.md) loss favours [rotation](../../../../../rotation-mathematics.md) about the axis of largest principal moment. Here “major axis” means maximum inertia, not necessarily the body's longest geometric direction. **A perfectly rigid torque-free body does not dissipatively settle**; its [energy](../../../../../energy-split.md) is conserved. Distinguishing stability from relaxation also explains why minimum-inertia [rotation](../../../../../rotation-mathematics.md) can be stable in the ideal rigid model.

**Forced [precession](../../../../../precession.md)** occurs when an external [torque](../../../../../torque.md) changes $\mathbf L$, with $\dot{\mathbf L}=\boldsymbol\tau$. For steady [precession](../../../../../precession.md), $\boldsymbol\tau=\boldsymbol\Omega_p\times\mathbf L$. A rapidly spinning, pivoted heavy [gyroscope](../../../../../gyroscope.md) has $L\simeq C\omega_3$ along its symmetry axis, giving

$$
\boxed{\Omega_p\simeq\frac{Mg\ell}{C\omega_3}.}
$$

The [torque](../../../../../torque.md) is perpendicular to the nearly axial [angular momentum](../../../../../angular-momentum.md), so it mainly changes its direction. For a steady inclined [symmetric top](../../../../../symmetric-top.md), the more complete condition is

$$
A\Omega_p^2\cos\theta-C\omega_3\Omega_p+Mg\ell=0.
$$

It exhibits slow and fast [precession](../../../../../precession.md) branches when real solutions exist. A generic release excites [nutation](../../../../../nutation.md) as well: inclination oscillates instead of staying fixed. Axis constraints and bearing forces must be included when specifying which [angular momentum](../../../../../angular-momentum.md) and pivot are being used.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
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
