<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

[Elasticity](../../../../../elasticity-physics-split.md) describes recoverable deformation. For small displacements $\mathbf u(\mathbf x)$, the [infinitesimal strain tensor](../../../../../infinitesimal-strain-tensor.md) is the symmetric part of the displacement gradient,

$$
\boxed{\epsilon_{ij}=\frac12(\partial_i u_j+\partial_j u_i).}
$$

Its diagonal entries describe extension, while its off-diagonal entries describe shear. The engineering shear strain is $\gamma_{xy}=2\epsilon_{xy}$; the antisymmetric part of the displacement gradient is a small rigid rotation, not elastic strain.

The [stress tensor](../../../../../cauchy-stress-tensor.md) specifies the [force](../../../../../force-split.md) per unit area on each oriented plane: $\mathbf t(\widehat{\mathbf n})=\boldsymbol\sigma\widehat{\mathbf n}$. Positive normal stress is tensile in the convention used here; tangential traction gives [shear stress](../../../../../shear-stress.md). In the absence of internal couples, angular-momentum balance makes the [stress tensor](../../../../../cauchy-stress-tensor.md) symmetric. Force balance gives $\nabla\cdot\boldsymbol\sigma+\mathbf f=0$ in static equilibrium, where $\mathbf f$ is body [force](../../../../../force-split.md) per unit volume.

[Linear elasticity](../../../../../linear-elasticity.md) relates stress and strain. A homogeneous isotropic solid needs two independent elastic constants:

$$
\boxed{\sigma_{ij}=\lambda\epsilon_{kk}\delta_{ij}+2G\epsilon_{ij}.}
$$

Here $G$ is the [shear modulus](../../../../../shear-modulus.md) and $\lambda$ is the other [Lamé parameter](../../../../../lame-parameter.md). For uniaxial loading, [Young's modulus](../../../../../young-s-modulus.md) is $E=\sigma_{xx}/\epsilon_{xx}$, with lateral contraction described by [Poisson's ratio](../../../../../poisson-s-ratio.md) $\nu=-\epsilon_{yy}/\epsilon_{xx}$. The [bulk modulus](../../../../../bulk-modulus.md) is $K=-p/(\Delta V/V)$ for a small hydrostatic compression. The relations between these constants are

$$
\boxed{E=2G(1+\nu)=3K(1-2\nu),\qquad K=\lambda+\frac{2G}{3}.}
$$

Stable isotropic elastic [strain energy density](../../../../../strain-energy-density.md) requires $G>0$ and $K>0$, implying $-1<\nu<1/2$. The incompressible limit is approached as $\nu\to1/2$. Anisotropic crystals generally need more constants; the isotropic relations should not be imposed on arbitrary directions in such a crystal.

The elastic [energy density](../../../../../energy-density.md) is $w=\boldsymbol\sigma:\boldsymbol\epsilon/2$. In the isotropic linear model this becomes $\lambda(\operatorname{tr}\boldsymbol\epsilon)^2/2+G\boldsymbol\epsilon:\boldsymbol\epsilon$. The quadratic form explains why reversible loading stores [energy](../../../../../energy-split.md) and unloading can return it, unlike plastic deformation or a dissipative hysteresis cycle.

For a slender beam described by the [Euler-Bernoulli beam equation](../../../../../euler-bernoulli-beam-equation.md), plane sections approximately remain plane. A fibre a distance $y$ from the neutral axis has axial strain $-y\kappa$, where $\kappa$ is curvature, and stress $-Ey\kappa$. Integrating its moment about the neutral axis gives, with consistent signs,

$$
\boxed{M=EI_A\kappa,\qquad I_A=\int_A y^2\,dA.}
$$

$I_A$ is a [second moment of area](../../../../../second-moment-of-area.md), with units of length to the fourth power; it is not a mass [moment of inertia](../../../../../moment-of-inertia.md). For a rectangular section of width $b$ and thickness $h$, $I_A=bh^3/12$, explaining the strong dependence of bending stiffness on thickness. For small transverse deflection $w(x)$, curvature is approximately $w''$, and the [Euler-Bernoulli beam equation](../../../../../euler-bernoulli-beam-equation.md) is $EI_Aw''''=q(x)$ with a suitable load-sign convention. A cantilever of length $\ell$ under end load $F$ has tip deflection $F\ell^3/(3EI_A)$ and largest bending stress of magnitude $F\ell c/I_A$, where $c$ is the furthest distance from the neutral axis.

In [torsion of a solid circular shaft](../../../../../torsion-of-a-solid-circular-shaft.md), a cross-section rotated by angle $\theta(x)$ has shear strain $r\theta'(x)$. Therefore

$$
\tau(r)=Gr\theta',\qquad \boxed{\mathcal T=GJ\theta',\quad J=\int_A r^2\,dA=\frac{\pi a^4}{2}.}
$$

Here $J$ is the [polar second moment of area](../../../../../polar-second-moment-of-area.md). A uniform shaft of length $\ell$ under constant torque twists by $\mathcal T\ell/(GJ)$, and its largest shear stress is $\mathcal T a/J$. Noncircular sections can warp, so replacing their torsional stiffness by $G$ times their polar area moment is not generally valid. Both bending and torsion formulas presume small, elastic deformations; exceeding the elastic limit can produce permanent deformation or fracture.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
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
