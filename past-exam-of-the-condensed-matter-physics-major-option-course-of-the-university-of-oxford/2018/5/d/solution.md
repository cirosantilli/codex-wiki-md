<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a long cylindrical wire carrying axial current $I$, [Ampère's law](../../../../ampere-s-circuital-law.md) gives $B_s=\mu_0I/(2\pi a)$ at its surface. With $a\gg\lambda$, the current resides mainly in a shell of thickness $\lambda$. If “critical” denotes the first equilibrium entry of vortices in an otherwise Meissner wire, set $B_s=B_{c1}$:

$$
\boxed{I_{c,\rm entry}=\frac{2\pi aB_{c1}}{\mu_0},\qquad
\overline J_{c,\rm entry}=\frac{I_c}{\pi a^2}=\frac{2B_{c1}}{\mu_0a}
\simeq\frac{9.5\times10^4}{a[\mathrm m]}\,\mathrm{A\,m^{-2}}.}
$$

The dependence on $a$ is necessary because no numerical radius is supplied. The _local_ surface [current density](../../../../current-density.md) at this entry scale is different:

$$
\boxed{j_{s,\rm entry}\simeq\frac{B_{c1}}{\mu_0\lambda}\sim6.8\times10^{11}\,\mathrm{A\,m^{-2}}.}
$$

Its conversion to the cross-section average is $\overline J\simeq(2\lambda/a)j_s$. Treating the shell [current density](../../../../current-density.md) as uniform over the entire thick wire would overestimate its total current by $a/(2\lambda)$.

**Meaning of a maximum:** in a type-II material, first [vortex](../../../../phase-vortex.md) entry need not be the measured dissipative transport limit. Pinned vortices can sustain greater current, whereas freely moving vortices generate voltage. The [hysteresis](../../../../hysteresis.md) loop indicates pinning, but no geometry-dependent pinning force or transport criterion is given, so a unique practical maximum cannot be deduced solely from $\lambda,\xi$ and $a$.

For comparison, the intrinsic homogeneous Ginzburg–Landau [depairing](../../../../superconducting-depairing-current-density.md) scale follows from $j(q)=\Phi_0q(1-\xi^2q^2)/(2\pi\mu_0\lambda^2)$. Maximizing at $q=1/(\sqrt3\xi)$ gives

$$
\boxed{j_d=\frac{\Phi_0}{3\sqrt3\pi\mu_0\lambda^2\xi}\sim1.8\times10^{12}\,\mathrm{A\,m^{-2}}.}
$$

This is a local, approximately uniform-flow theoretical scale, not the average [current density](../../../../current-density.md) throughout a thick self-field wire. Surface barriers, nonlinear screening, [vortex](../../../../phase-vortex.md) motion and [temperature](../../../../temperature-split.md) determine how that scale relates to its actual critical current. Thus the entry estimate, local shell density and intrinsic [depairing](../../../../superconducting-depairing-current-density.md) limit answer distinct physical criteria; the source's word “maximum” does not supply the missing pinning information.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
