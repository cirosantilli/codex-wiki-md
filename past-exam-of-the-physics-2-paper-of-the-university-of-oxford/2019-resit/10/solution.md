<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

In the [Huygens-Fresnel principle](../../../huygens-fresnel-principle.md) construction, after a time $\Delta t$ the incident disturbance advances $v_1\Delta t$ while the secondary disturbance in the second medium advances $v_2\Delta t$. The two right triangles share the segment along the interface. Hence

$$
\frac{\sin\theta_1}{\sin\theta_2}=\frac{v_1}{v_2}=\frac{n_2}{n_1},\qquad
\boxed{\theta_2=\arcsin\!\left(\frac{n_1}{n_2}\sin\theta_1\right).}
$$

Here both [angles](../../../angle.md) are measured from the [normal vector](../../../normal-vector.md), and $v_j=c/n_j$ are [phase velocities](../../../phase-velocity.md). This is [Snell's law](../../../snell-s-law.md). For $n_1>n_2$, no real transmitted [angle](../../../angle.md) exists when

$$
\boxed{\theta_1>\theta_c=\arcsin(n_2/n_1).}
$$

This is [total internal reflection](../../../total-internal-reflection.md); equality is the limiting grazing geometry. The statement concerns an ideal transparent interface, not material absorption or losses at a nearby second boundary.

Let $\beta$ be the internal [angle](../../../angle.md) to the [optical axis](../../../optical-axis.md) in the straight [step-index optical fiber](../../../step-index-optical-fiber.md). At its flat entrance, [Snell's law](../../../snell-s-law.md) gives $\sin\theta_i=n_1\sin\beta$. At the side wall a [meridional ray](../../../meridional-ray.md) has [angle of incidence](../../../angle-of-incidence.md) $\pi/2-\beta$. The limiting [total internal reflection](../../../total-internal-reflection.md) condition is $\cos\beta=n_2/n_1$. Thus the [optical fiber acceptance angle](../../../optical-fiber-acceptance-angle.md) satisfies

$$
\boxed{\sin\theta_{i,\max}=\sqrt{n_1^2-n_2^2}\equiv\mathrm{NA},\qquad
\theta_{i,\max}=\arcsin\sqrt{n_1^2-n_2^2}.}
$$

The [numerical aperture](../../../numerical-aperture.md) expression assumes the square root is at most one for air; otherwise all forward launch [angles](../../../angle.md) are admitted by this ideal ray test. Strictly confined [meridional rays](../../../meridional-ray.md) lie inside the limiting cone.

For $n_1=1.48$ and $n_2=1.46$, $\mathrm{NA}=0.242487$ and $\theta_{i,\max}=14.0334^\circ$. A [light ray](../../../light-ray.md) at internal [angle](../../../angle.md) $\beta$ travels distance $L/\cos\beta$ along a guide of axial length $L$. In the nondispersive approximation its [travel time](../../../travel-time.md) is $t=n_1L/(c\cos\beta)$. Therefore

$$
\begin{aligned}
t_{\max}&=\frac{n_1^2L}{cn_2}=5.00438\,\mu\mathrm s,\\
t_{\mathrm{half}}&=\frac{n_1L}{c\sqrt{1-\sin^2(\theta_{i,\max}/2)/n_1^2}}
=4.95365\,\mu\mathrm s,
\end{aligned}
\qquad
\boxed{\Delta t\simeq50.7\,\mathrm{ns}.}
$$

Here $L=1000\,\mathrm m$ and $c=299792458\,\mathrm{m\,s^{-1}}$; using $3.00\times10^8\,\mathrm{m\,s^{-1}}$ gives $5.001\,\mu\mathrm s$ and $4.950\,\mu\mathrm s$. The halving applies to the external launch [angle](../../../angle.md), not to $\beta$. For actual short pulses the [group refractive index](../../../group-refractive-index.md) $n_{\mathrm g}$ replaces the prefactor $n_1$ in $t=n_{\mathrm g}L/(c\cos\beta)$; the source supplies no [optical dispersion](../../../dispersion-optics.md) data. The difference calculated here is geometrical [intermodal dispersion](../../../intermodal-dispersion.md) in a nondispersive [geometrical optics](../../../geometrical-optics-split.md) model.

Bending lowers the outer-wall [angle of incidence](../../../angle-of-incidence.md), allowing a previously guided [light ray](../../../light-ray.md) to escape into the cladding. To calculate a definite [meridional ray bend threshold](../../../meridional-ray-bend-threshold.md), continue the on-axis launch assumption and take a [meridional ray](../../../meridional-ray.md) in the plane of the circular bend. Its initial internal [angle](../../../angle.md) to the centreline tangent obeys $\sin\beta=\sin10^\circ/n_1$. Its straight path has distance $b_{\mathrm{ray}}=R\cos\beta$ from the bend centre. At the outer wall of radius $R+r$, elementary right-triangle geometry gives

$$
\sin i_{\mathrm{out}}=\frac{R\cos\beta}{R+r}.
$$

At the loss threshold, this equals $n_2/n_1$. Solving for the centreline radius gives

$$
\boxed{R_c=\frac{n_2r}{n_1\cos\beta-n_2}
=\frac{n_2r}{\sqrt{n_1^2-\sin^2 10^\circ}-n_2}
=14.93\,\mathrm{mm}.}
$$

For this launch, $R<R_c$ violates the [total internal reflection](../../../total-internal-reflection.md) condition at the outer wall; $R=R_c$ is the limiting case. A real [optical fiber](../../../optical-fiber.md) has gradual bend loss governed by its [electromagnetic wave](../../../electromagnetic-wave-split.md) modes, rather than a universal abrupt cutoff.

**Launch dependence.** The final sentence does not separately specify the entry position or orientation of the bend relative to the incident [light ray](../../../light-ray.md). For a planar launch displaced by $u$ from the centreline toward the outer wall, replace the numerator of $\sin i_{\mathrm{out}}$ by $(R+u)\cos\beta$. For example, a launch at the inner edge, $u=-r$, instead gives

$$
R_{c,\mathrm{inner}}=r\frac{n_1\cos\beta+n_2}{n_1\cos\beta-n_2}=29.96\,\mathrm{mm}.
$$

Thus $14.93\,\mathrm{mm}$ is the result for the stated on-axis continuation; it is not an entry-independent threshold. No missing figure is needed for these explicitly specified ray models.

## ↑ Ancestors (11)

1. [10](../10.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
