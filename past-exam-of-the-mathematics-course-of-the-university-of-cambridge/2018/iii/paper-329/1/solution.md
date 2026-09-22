<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $r=|\mathbf x|$ and take $\mu$ to be the dynamic viscosity. The [Papkovich–Neuber representation](../../../../../papkovich-neuber-representation.md) of a homogeneous [Stokes flow](../../../../../stokes-flow-split.md) uses a [harmonic](../../../../../harmonic-function.md) vector potential $\boldsymbol\Phi$ and [harmonic](../../../../../harmonic-function.md) scalar potential $\chi$:

$$
\boxed{2\mu\mathbf u=\nabla(\mathbf x\cdot\boldsymbol\Phi+\chi)-2\boldsymbol\Phi,
\qquad p=\nabla\cdot\boldsymbol\Phi,\qquad
\nabla^2\boldsymbol\Phi=0,\quad\nabla^2\chi=0.}
$$

These formulas give [incompressibility](../../../../../incompressible-flow.md) because $\nabla^2(\mathbf x\cdot\boldsymbol\Phi)=2\nabla\cdot\boldsymbol\Phi$, and give $\mu\nabla^2\mathbf u=\nabla p$, the [Stokes equation](../../../../../stokes-equation.md) away from forcing.

For a point force represented by a [Dirac delta distribution](../../../../../dirac-delta-function.md), rotational covariance and the [Linearity of Stokes flow](../../../../../linearity-of-stokes-flow.md) suggest a vector monopole proportional to $\mathbf F/r$: $1/r$ is a [harmonic function](../../../../../harmonic-function.md) outside the origin, and its slow decay gives the required nonzero resultant force. Take

$$
\boldsymbol\Phi=-\frac{\mathbf F}{4\pi r},\qquad\chi=0.
$$

Substitution gives the [Stokeslet](../../../../../stokeslet.md) velocity and pressure:

$$
\boxed{\mathbf u=\frac1{8\pi\mu}\left[\frac{\mathbf F}{r}
+\frac{(\mathbf F\cdot\mathbf x)\mathbf x}{r^3}\right],
\qquad p=\frac{\mathbf F\cdot\mathbf x}{4\pi r^3}.}
$$

The normalization follows from the [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md). Differentiating the velocity gives the [rate of strain and vorticity of a Stokeslet](../../../../../rate-of-strain-and-vorticity-of-a-stokeslet.md):

$$
\boxed{e_{ij}=\frac{\mathbf F\cdot\mathbf x}{8\pi\mu r^3}
\left(\delta_{ij}-3\frac{x_ix_j}{r^2}\right),\qquad
\boldsymbol\omega=\nabla\times\mathbf u=\frac{\mathbf F\times\mathbf x}{4\pi\mu r^3}.}
$$

Here $e_{ij}=(\partial_i u_j+\partial_j u_i)/2$. Thus $\sigma_{ij}=-p\delta_{ij}+2\mu e_{ij}=-3(\mathbf F\cdot\mathbf x)x_ix_j/(4\pi r^5)$. On a sphere enclosing the origin, its outward traction integrates to $-\mathbf F$, so $\nabla\cdot\boldsymbol\sigma+\mathbf F\delta(\mathbf x)=0$ in the distributional sense. All displayed fields away from the point force have $r>0$.

For a [sphere in a uniform straining Stokes flow](../../../../../sphere-in-a-uniform-straining-stokes-flow.md), centre the sphere at the origin and write the ambient velocity as $\mathbf E\mathbf x$, with $\mathbf E^T=\mathbf E$ and $\operatorname{tr}\mathbf E=0$. [Faxén's first law](../../../../../faxen-s-first-law.md) and [Faxén's rotational law](../../../../../faxen-s-rotational-law.md) give zero translation and rotation. To impose the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md), use the decaying [harmonic](../../../../../harmonic-function.md) dipole and quadrupole potentials

$$
\boldsymbol\Phi=A\frac{\mathbf E\mathbf x}{r^3},\qquad
\chi=B\frac{Q}{r^5},\qquad Q=\mathbf E:\mathbf x\mathbf x.
$$

Trace freedom makes $Q/r^5$ harmonic, and each component of $\mathbf E\mathbf x/r^3$ is [harmonic](../../../../../harmonic-function.md). The [Papkovich–Neuber representation](../../../../../papkovich-neuber-representation.md) gives

$$
2\mu\mathbf u'=-3A\frac{Q\mathbf x}{r^5}
+B\left[\frac{2\mathbf E\mathbf x}{r^5}-\frac{5Q\mathbf x}{r^7}\right].
$$

At $r=a$, the coefficient of $\mathbf E\mathbf x$ must give $\mathbf u'=-\mathbf E\mathbf x$, while the extra radial term must vanish. Hence $B=-\mu a^5$ and $A=5\mu a^3/3$, giving the complete disturbance

$$
\boxed{\mathbf u'=-\frac{a^5}{r^5}\mathbf E\mathbf x
-\frac{5a^3}{2r^5}\left(1-\frac{a^2}{r^2}\right)Q\mathbf x,
\qquad p'=-\frac{5\mu a^3}{r^5}Q.}
$$

The total velocity vanishes on the sphere and tends to the imposed strain at infinity. This field has no [Stokeslet](../../../../../stokeslet.md) or [rotlet](../../../../../rotlet.md) contribution, consistent with a [force-free](../../../../../force-free.md), [torque-free](../../../../../torque-free.md) sphere. Its leading far field is the radial [stresslet](../../../../../force-dipole-flow.md) $-5a^3Q\mathbf x/(2r^5)$.

Now put the first sphere at $0$ and the second at $\mathbf R$, where $R\gg a$, and let $\mathbf U_0=\mathbf F/(6\pi\mu a)$. The first sphere's leading disturbance is its [Stokeslet](../../../../../stokeslet.md). The [rate-of-strain tensor](../../../../../strain-rate-tensor.md) and [vorticity](../../../../../vorticity.md) incident on the second sphere are

$$
\mathbf E_2=\frac{3a}{4R^3}(\mathbf U_0\cdot\mathbf R)
(\mathbf I-3\widehat{\mathbf R}\widehat{\mathbf R}),\qquad
\boldsymbol\omega_2=\frac{3a}{2R^3}\mathbf U_0\times\mathbf R.
$$

The second sphere translates with the local flow and rotates with half its local [vorticity](../../../../../vorticity.md). Its [force-free](../../../../../force-free.md) and [torque-free](../../../../../torque-free.md) conditions therefore remove any reflected force or torque monopole. The incident strain produces the [stresslet](../../../../../force-dipole-flow.md) just obtained. Since

$$
\mathbf E_2:\mathbf R\mathbf R=-\frac{3a}{2R}(\mathbf U_0\cdot\mathbf R),
$$

its velocity at the first centre, using the relative vector $-\mathbf R$, is

$$
\mathbf u'_2(-\mathbf R)
=\frac{5a^3}{2R^5}(\mathbf E_2:\mathbf R\mathbf R)\mathbf R
=-\frac{15a^4}{4R^6}(\mathbf U_0\cdot\mathbf R)\mathbf R.
$$

[Faxén's first law](../../../../../faxen-s-first-law.md) then gives the [self-mobility correction from a distant force-free sphere](../../../../../self-mobility-correction-from-a-distant-force-free-sphere.md):

$$
\boxed{\mathbf U=\mathbf U_0-\frac{15a^4}{4R^6}(\mathbf U_0\cdot\mathbf R)\mathbf R
+O(U_0a^5/R^5).}
$$

Finite-size terms and further reflections are beyond the leading order retained in this [method of reflections for Stokes flow](../../../../../method-of-reflections-for-stokes-flow.md).

Only the imposed force does work, so the [viscous dissipation](../../../../../viscous-dissipation.md) is $\mathcal D=\mathbf F\cdot\mathbf U$. With $\zeta=6\pi\mu a$, define $\varepsilon_R=a/R$ and $\gamma=15a^4/(4R^6)$. At fixed $\mathbf F$,

$$
\mathcal D=\zeta\left[U_0^2-\gamma(\mathbf U_0\cdot\mathbf R)^2\right]
+O(\zeta U_0^2\varepsilon_R^5),
$$

so the leading change is negative when $\mathbf U_0\cdot\mathbf R\ne0$. The direction is held fixed in taking $\varepsilon_R\to0$.

The [fixed-force comparison of minimum viscous dissipation](../../../../../fixed-force-comparison-of-minimum-viscous-dissipation.md) distinguishes the prescribed force from prescribed boundary velocity. Indeed,

$$
U^2=U_0^2-2\gamma(\mathbf U_0\cdot\mathbf R)^2
+O(U_0^2\varepsilon_R^5),
$$

and hence

$$
\boxed{\mathcal D-\zeta U^2=\zeta\gamma(\mathbf U_0\cdot\mathbf R)^2
+O(\zeta U_0^2\varepsilon_R^5)>0\quad\text{to leading order}.}
$$

At the actual reduced velocity, adding the second sphere increases the dissipation relative to an isolated translating sphere at that same velocity, exactly as required by the [Minimum-dissipation theorem for Stokes flow](../../../../../minimum-dissipation-theorem-for-stokes-flow.md). One can extend the two-sphere velocity rigidly into the second sphere, adding zero strain and producing an admissible trial field in the domain without it. The reflected angular velocity of the first sphere contributes only a higher-order squared rotational power to this comparison.

Finally hold the second sphere's angular velocity at zero. [Faxén's rotational law](../../../../../faxen-s-rotational-law.md) requires the applied couple

$$
\mathbf G_2=-4\pi\mu a^3\boldsymbol\omega_2
=-\frac{6\pi\mu a^4}{R^3}\mathbf U_0\times\mathbf R.
$$

The resulting [rotlet](../../../../../rotlet.md) adds at the first centre

$$
\delta\mathbf U_{\mathrm{rot}}
=\frac{\mathbf G_2\times(-\mathbf R)}{8\pi\mu R^3}
=-\frac{3a^4}{4R^4}\left[\mathbf U_0-(\mathbf U_0\cdot\widehat{\mathbf R})\widehat{\mathbf R}\right].
$$

This is the additional [rotational constraint correction to sphere mobility](../../../../../rotational-constraint-correction-to-sphere-mobility.md). Including the strain reflection, the total leading change relative to the isolated velocity is

$$
\boxed{\mathbf U_{\mathrm{locked}}-\mathbf U_0
=-\frac{3a^4}{4R^4}\left[\mathbf U_0+4(\mathbf U_0\cdot\widehat{\mathbf R})\widehat{\mathbf R}\right]
+O(U_0a^5/R^5).}
$$

For motion parallel to the line of centres the constraint adds nothing at this order; for transverse motion it supplies an extra resisting correction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 329](../../paper-329-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
