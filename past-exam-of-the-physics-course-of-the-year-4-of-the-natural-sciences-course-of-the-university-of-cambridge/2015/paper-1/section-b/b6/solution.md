<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

The [electric displacement field](../../../../../electric-displacement-field.md) is $\mathbf D=\epsilon_0\mathbf E+\mathbf P$. A homogeneous linear isotropic dielectric has $\mathbf P=\epsilon_0\chi_e\mathbf E$, so $\mathbf D=\epsilon_0\epsilon_r\mathbf E$. At a free-charge-free interface the normal component of D is continuous, while electrostatics requires continuity of tangential E.

At half immersion the conductor centre lies in the flat air-liquid interface. Set $\phi=C/r$ in both media, with potential zero at infinity. The sphere is an equipotential, and the potential is continuous across the liquid plane. On that plane the radial E field is tangential, so tangential E agrees while both normal D components vanish. Each half-space also satisfies the source-free potential equation. The fields outside the sphere are

$$
\boxed{\mathbf E=\frac C{r^2}\hat{\mathbf r},\qquad
\mathbf D=\begin{cases}\epsilon_0C\hat{\mathbf r}/r^2,&\text{air},\\
\epsilon_0\epsilon_rC\hat{\mathbf r}/r^2,&\text{liquid}.\end{cases}}
$$

Gauss's law for D on a sphere gives $Q=2\pi\epsilon_0(1+\epsilon_r)C$. Therefore

$$
\boxed{C=\frac{Q}{2\pi\epsilon_0(1+\epsilon_r)},\qquad
V=\frac{Q}{2\pi\epsilon_0(1+\epsilon_r)a}.}
$$

The [half-immersed conducting sphere in a dielectric](../../../../../half-immersed-conducting-sphere-in-a-dielectric.md) has radial E lines with equal field strength at equal radius on either side, whereas the D flux density is $\epsilon_r$ times larger in the liquid. The corresponding free surface charge is larger on the lower hemisphere. The unchanged field direction at this particular interface follows from its tangential geometry, not from a claim that [electric fields](../../../../../electric-field-split.md) never refract at dielectric interfaces.

<a id="section-b/b6/image-radial-electric-field-and-unequal-displacement-flux-for-a-half-immersed-conducting-sphere"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1-half-immersed-sphere.png)

**[Figure 7](#section-b/b6/image-radial-electric-field-and-unequal-displacement-flux-for-a-half-immersed-conducting-sphere). Radial electric field and unequal displacement flux for a half-immersed conducting sphere**. Original electrostatic field-line schematic. The illustrated dielectric has relative permittivity three; D-line density, rather than line direction, differs between the media.

The outward [electrostatic pressure](../../../../../electrostatic-pressure.md) is $p_e=\mathbf E\cdot\mathbf D/2$. Integrating its vertical component over the two hemispheres uses $\int_{\rm upper}\cos\theta\,dA=\pi a^2$ and the negative of that integral below. Thus

$$
F_z^{\rm electric}=\frac{\pi a^2\epsilon_0E(a)^2}{2}(1-\epsilon_r),
\qquad
F_{\rm down}=\frac{Q^2(\epsilon_r-1)}{8\pi\epsilon_0(1+\epsilon_r)^2a^2}.
$$

The [force](../../../../../force-split.md) is downward for $\epsilon_r>1$. Initially, buoyancy on the uncharged sphere gives $\rho_\ell gf(4\pi a^3/3)=Mg$. At half immersion the upward buoyancy is therefore $Mg/(2f)$, leaving a required downward electric [force](../../../../../force-split.md) $Mg(1/(2f)-1)$. Equating the two gives

$$
\boxed{Q^2=4\pi\epsilon_0\frac{(\epsilon_r+1)^2}{\epsilon_r-1}
\left(\frac1f-2\right)Mga^2.}
$$

This uses the ideal flat-interface, linear-dielectric model with surface tension and interface deformation neglected. If $\epsilon_r=1$, there is no electric [force](../../../../../force-split.md) of this kind, consistently preventing this mechanism from pulling an initially less-than-half-immersed sphere down to the specified level.

## ↑ Ancestors (13)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
