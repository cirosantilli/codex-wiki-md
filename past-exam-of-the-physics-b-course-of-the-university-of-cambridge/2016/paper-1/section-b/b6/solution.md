<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

The [method of images](../../../../../method-of-images.md) replaces induced charges or currents on a boundary by fictitious sources outside the physical region, chosen to satisfy that boundary's conditions. For example, a point charge $q$ a height $d$ above a grounded conducting plane has an image $-q$ at the reflected point. The sum has zero potential on the plane, and the electrostatic uniqueness theorem identifies it with the physical solution in the upper half-space. Images do not describe a second physical charge below the metal.

For the superconducting plane, use the different [boundary condition](../../../../../boundary-condition.md) **$B_z=0$ at its surface**: [magnetic flux](../../../../../magnetic-flux.md) cannot enter the ideal bulk. Choose the real ring moment $\mathbf m=m\widehat z$, where $m=I\pi R^2$, at $z=h$. Its image has moment $-m\widehat z$ at $z=-h$. This [superconducting plane image dipole](../../../../../superconducting-plane-image-dipole.md) makes the normal fields cancel at $z=0$, while their tangential fields add. The image is a computational continuation; the physical field inside the plane is zero. The original sketch shows the dipole-scale field, appropriate to $h\gg R$; the fine field close to the ring wire is outside that approximation.

<a id="section-b/b6/image-original-dipole-scale-field-above-a-flux-excluding-plane-with-the-opposite-image-moment-shown-schematically"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1-superconductor-field.png)

**[Figure 2](#section-b/b6/image-original-dipole-scale-field-above-a-flux-excluding-plane-with-the-opposite-image-moment-shown-schematically). Original dipole-scale field above a flux-excluding plane, with the opposite image moment shown schematically**.

In the vacuum region the [magnetic scalar potential](../../../../../magnetic-scalar-potential.md) is

$$
\phi_m(\rho,z)=\frac m{4\pi}\left[\frac{z-h}{(\rho^2+(z-h)^2)^{3/2}}-\frac{z+h}{(\rho^2+(z+h)^2)^{3/2}}\right],\qquad \mathbf B=-\mu_0\nabla\phi_m.
$$

At the surface $z=0$, it reduces to $-mh/[2\pi(\rho^2+h^2)^{3/2}]$. Its tangential derivative therefore gives

$$
\boxed{\mathbf B(a,0)=-\frac{3\mu_0mha}{2\pi(a^2+h^2)^{5/2}}\widehat{\boldsymbol\rho}=-\frac{3\mu_0IR^2ha}{2(a^2+h^2)^{5/2}}\widehat{\boldsymbol\rho}.}
$$

Both $B_z$ and $B_\phi$ vanish there; the sign is inward radially for the chosen positive moment. The expression is the leading dipole result, not an exact finite-ring formula at arbitrary $R/h$.

For the [force](../../../../../force-split.md), calculate the external image field on the axis near the real dipole:

$$
B_{{\rm im},z}(z)=-\frac{\mu_0m}{2\pi(z+h)^3}.
$$

Differentiate this field with the image location held fixed, then evaluate at $z=h$. The [dipole levitation force above a superconducting plane](../../../../../dipole-levitation-force-above-a-superconducting-plane.md) is

$$
F_z=m\left.\frac{\partial B_{{\rm im},z}}{\partial z}\right|_{z=h}=\frac{3\mu_0m^2}{32\pi h^4}=\boxed{\frac{3\pi\mu_0I^2R^4}{32h^4}},
$$

directed upward. Differentiating a substituted separation $2h$ while moving both dipoles in the [force](../../../../../force-split.md) derivative would incorrectly double the result.

To levitate ring [mass](../../../../../mass.md) $M$, balance this [force](../../../../../force-split.md) against $Mg$:

$$
\boxed{I_{\rm lev}=\sqrt{\frac{32Mgh^4}{3\pi\mu_0R^4}}.}
$$

A light, thin wire and the smallest practical gap reduce current. At fixed gap and wire cross-section $s$, $M=2\pi R s\rho_w$ gives $I_{\rm lev}\propto h^2\sqrt{s\rho_w}/R^{3/2}$, favouring a larger ring until the dipole-limit constraint on $R/h$ matters. There is no unique least current without geometric and material constraints. As a geometrically consistent order-of-magnitude example, take $R=1\,\mathrm{mm}$, $h=10\,\mathrm{mm}$, wire radius $50\,\mathrm{\mu m}$ and an assumed metallic-scale [density](../../../../../density.md) $\rho_w=6.0\times10^3\,\mathrm{kg\,m^{-3}}$. Then $M=2.96\times10^{-7}\,\mathrm{kg}$ and **$I_{\rm lev}\simeq2.8\times10^2\,\mathrm A$**. The large value reflects the weak $h^{-4}$ [force](../../../../../force-split.md) in the stipulated far-field geometry. Uniformly shrinking this geometrical example reduces current as size to the [power](../../../../../power.md) $3/2$, but increases required [electric current density](../../../../../current-density.md); arbitrarily thin wire is therefore not a free optimization.

This balance estimate is not a verified superconducting design. The actual wire must carry that current without quenching, its self-field counts toward the limit, the plane must remain in its assumed flux-excluding state, and leads or supports add load. Transport critical-current measurements specify [temperature](../../../../../temperature-split.md), applied field and the [voltage](../../../../../voltage.md) criterion rather than a material-independent limiting current.[NBS SP 260-91, Section 7 and Table 3, field/temperature-dependent critical-current specification](../../../../../standard-reference-materials-critical-current-measurements-on-an-nbti-superconducting-wire-standard-reference-material-by-a-f-clark-and-others.md)

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
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
