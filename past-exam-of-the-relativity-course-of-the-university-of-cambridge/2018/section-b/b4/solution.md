<h1 id="section-b/b4/solution">Solution</h1>

↑ **Parent:** [B4](../b4.md)

**Local equivalence and tides.** In [Newtonian mechanics](../../../../newtonian-mechanics-split.md), [inertial mass](../../../../inertial-mass.md) $m_{\rm i}$ measures the response to a [force](../../../../force-split.md), whereas passive [gravitational mass](../../../../gravitational-mass.md) $m_{\rm g}$ couples to an imposed [Newtonian gravitational field](../../../../newtonian-gravitational-field.md). A freely falling body obeys

$$
m_{\rm i}\mathbf a=m_{\rm g}\mathbf g,\qquad
\mathbf a=\frac{m_{\rm g}}{m_{\rm i}}\mathbf g.
$$

The observed composition independence of [free fall](../../../../free-fall.md) says that this ratio is universal. With a common choice of units it is one. This is the Newtonian content of the [weak equivalence principle](../../../../weak-equivalence-principle.md) for [test particles](../../../../test-particle.md); it does not by itself specify all nongravitational physics.

The [Einstein equivalence principle](../../../../einstein-equivalence-principle.md) further says that local nongravitational experiments in a sufficiently small freely falling laboratory have the form predicted by [special relativity](../../../../special-relativity-split.md), independently of the laboratory's location and motion. In such a [local inertial frame](../../../../local-inertial-frame.md), the [metric tensor](../../../../metric-tensor.md) is locally the [Minkowski metric](../../../../minkowski-metric.md) and the [Christoffel symbols](../../../../christoffel-symbol.md) vanish at the selected event. The [strong equivalence principle](../../../../strong-equivalence-principle.md) extends the universality claim to local gravitational experiments and bodies with significant gravitational self-energy. None of these statements removes measurable [tidal forces](../../../../tidal-force.md) across a finite apparatus.

In an ideal small freely falling lift, a released ball initially floats relative to the cabin, because both undergo the same [free fall](../../../../free-fall.md). Two separated balls, however, need not retain their separation: they sample different parts of the [gravitational field](../../../../gravitational-field.md). For a point source, linearizing $\mathbf g=-GM\mathbf r/r^3$ across a small separation $\boldsymbol\xi$ gives the [tidal tensor](../../../../tidal-tensor.md) prediction

$$
\boxed{\frac{d^2\boldsymbol\xi}{dt^2}
=\frac{GM}{r^3}\big[3\widehat{\mathbf r}(\widehat{\mathbf r}\cdot\boldsymbol\xi)-\boldsymbol\xi\big].}
$$

A radial separation stretches with coefficient $2GM/r^3$, whereas a transverse separation is compressed with coefficient $-GM/r^3$. Initially parallel [velocities](../../../../velocity.md) therefore develop relative motion even though the individual bodies experience zero [proper acceleration](../../../../proper-acceleration.md).

The relativistic statement is [geodesic deviation](../../../../geodesic-deviation.md). With the [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) convention

$$
R^\mu{}_{\nu\rho\sigma}
=\partial_\rho\Gamma^\mu{}_{\sigma\nu}-\partial_\sigma\Gamma^\mu{}_{\rho\nu}
+\Gamma^\mu{}_{\rho\alpha}\Gamma^\alpha{}_{\sigma\nu}
-\Gamma^\mu{}_{\sigma\alpha}\Gamma^\alpha{}_{\rho\nu},
$$

a connecting vector between neighboring freely falling [worldlines](../../../../world-line.md) satisfies

$$
\boxed{\frac{D^2\xi^\mu}{d\tau^2}
=-R^\mu{}_{\nu\rho\sigma}U^\nu\xi^\rho U^\sigma.}
$$

Here $D/d\tau$ is the [covariant derivative](../../../../covariant-derivative.md) along the reference [geodesic](../../../../geodesic.md), and $U^\mu$ its [four-velocity](../../../../four-velocity.md). [Curvature](../../../../curvature.md) can be nonzero where the [Christoffel symbols](../../../../christoffel-symbol.md) have been made zero. In the weak, static, slow-motion limit this equation reduces to $\ddot\xi^i=-\partial_i\partial_j\Phi\,\xi^j$, recovering the [tidal tensor](../../../../tidal-tensor.md) above. A finite falling lift can detect [gravity](../../../../gravity.md) through these relative [accelerations](../../../../acceleration.md); local equivalence does not imply a globally uniform field.

**Weak-field connection and potential.** Take $x^0=ct$ and the $+---$ [metric signature](../../../../metric-signature.md). There is an index error in the printed formula for the [Christoffel symbols](../../../../christoffel-symbol.md): its first differentiated metric component must be $g_{\nu0}$, not $g_{\mu0}$. The correctly contracted expression is

$$
\Gamma^\mu{}_{00}=\frac12g^{\mu\nu}
\left(2\partial_0g_{\nu0}-\partial_\nu g_{00}\right).
$$

The offending term vanishes under the stipulated time independence, so this correction does not change the intended calculation. Write $g_{\mu\nu}=\eta_{\mu\nu}+h_{\mu\nu}$ and treat both $h$ and its [derivatives](../../../../derivative.md) as first order. To that order $g^{00}=1-h_{00}$, $g^{0i}=O(h)$, and $g^{ij}=-\delta^{ij}+O(h)$. A stationary [metric tensor](../../../../metric-tensor.md) gives

$$
\Gamma^\mu{}_{00}=-\frac12g^{\mu j}\partial_jh_{00}.
$$

For the temporal component the inverse-metric coefficient is already first order, so

$$
\boxed{\Gamma^0{}_{00}=O(h\,\partial h)\approx0.}
$$

For a spatial component the zeroth-order inverse metric contributes:

$$
\boxed{\Gamma^i{}_{00}\approx\frac12\delta^{ij}\partial_jh_{00}
=\frac12\frac{\partial h_{00}}{\partial x^i}.}
$$

The time component of the approximate [geodesic equation](../../../../geodesic-equation.md) says that $dt/d\tau$ is constant to the retained order. In its spatial component, convert the [proper time](../../../../proper-time.md) derivatives to coordinate-time derivatives and cancel $(dt/d\tau)^2$:

$$
\frac{d^2x^i}{dt^2}\approx-c^2\Gamma^i{}_{00}
\approx-\frac{c^2}{2}\partial_i h_{00}.
$$

Comparison with the Newtonian equation $d^2\mathbf x/dt^2=-\boldsymbol\nabla\Phi$ identifies $h_{00}=2\Phi/c^2+C$. For an isolated source, choose the [gravitational potential](../../../../newtonian-potential-of-a-point-mass.md) to tend to zero at infinity and normalize the time coordinate there, giving $C=0$. Thus

$$
\boxed{g_{00}\approx1+\frac{2\Phi}{c^2}.}
$$

The quantity $\Phi$ is the Newtonian [gravitational potential](../../../../newtonian-potential-of-a-point-mass.md), or [gravitational potential energy](../../../../gravitational-energy.md) per unit [mass](../../../../mass.md), in $\mathrm{J\,kg^{-1}}=\mathrm{m^2\,s^{-2}}$. For a point source, $\Phi=-GM/r$. A static clock has $d\tau=\sqrt{g_{00}}\,dt\approx(1+\Phi/c^2)dt$, connecting the [Newtonian limit](../../../../newtonian-limit.md) with [gravitational time dilation](../../../../gravitational-time-dilation.md).

**Frequency of the orbiting source.** Treat the gas blob as a [test particle](../../../../test-particle.md) on a [timelike circular Schwarzschild geodesic](../../../../timelike-circular-schwarzschild-geodesic.md), with pressure and other nongravitational forces negligible. Treat our very distant location as infinity, so the observer's own [gravitational potential](../../../../newtonian-potential-of-a-point-mass.md) is negligible. These are the assumptions that make a unique answer in terms of $R_S/r$ possible.

Put $f=1-R_S/r$ and use a local static observer at the emission point as an intermediate measuring frame. The remote observer lies on the symmetry axis of the orbit. A ray arriving on that axis has zero conserved axial [angular momentum](../../../../angular-momentum.md), so its local direction is perpendicular to the emitter's azimuthal [velocity](../../../../velocity.md). Bending within a meridional plane does not alter this orthogonality. The transverse [relativistic Doppler effect](../../../../relativistic-doppler-effect.md) therefore gives

$$
\nu_{\rm stat}=\frac{\nu_{\rm em}}{\gamma_v},\qquad
\gamma_v=\frac1{\sqrt{1-v^2/c^2}},
$$

where $v$ is the orbital [speed](../../../../speed.md) measured by that local static observer. The [gravitational redshift between static Schwarzschild observers](../../../../gravitational-redshift-between-static-schwarzschild-observers.md) then gives

$$
\frac{\nu_{\rm ob}}{\nu_{\rm em}}=\frac{\sqrt{1-R_S/r}}{\gamma_v}.
$$

A gravitational [circular orbit](../../../../circular-orbit.md) has $v^2=GM/r+O((GM/r)^2/c^2)$ in the weak-field limit, so $v^2/c^2=R_S/(2r)+O((R_S/r)^2)$. Expanding both factors,

$$
\frac{\nu_{\rm ob}}{\nu_{\rm em}}
=\left(1-\frac{R_S}{2r}\right)
\left(1-\frac{R_S}{4r}\right)+O\!\left(\frac{R_S^2}{r^2}\right)
=1-\frac{3R_S}{4r}+O\!\left(\frac{R_S^2}{r^2}\right).
$$

Solving for the emitted [frequency](../../../../frequency.md) gives

$$
\boxed{\nu_{\rm em}=\nu_{\rm ob}\left[1+\frac{3R_S}{4r}+O\!\left(\frac{R_S^2}{r^2}\right)\right].}
$$

The gravitational part is $R_S/(2r)$ and the transverse kinematic [time dilation](../../../../time-dilation.md) contributes another $R_S/(4r)$; the absence of line-of-sight motion does not remove this second effect.

As an exact check, the local speed on a [timelike circular Schwarzschild geodesic](../../../../timelike-circular-schwarzschild-geodesic.md) satisfies $v^2/c^2=\mu/(r-2\mu)$, where $\mu=GM/c^2=R_S/2$. Therefore the [face-on frequency shift of a circular Schwarzschild source](../../../../face-on-frequency-shift-of-a-circular-schwarzschild-source.md) is

$$
\frac{\nu_{\rm ob}}{\nu_{\rm em}}=\sqrt{1-\frac{3\mu}{r}}
=\sqrt{1-\frac{3R_S}{2r}},
$$

whose expansion agrees with the boxed answer. If the gas is supported or accelerated by pressure or magnetic stresses rather than following a [geodesic](../../../../geodesic.md), its [orbital speed](../../../../orbital-speed.md) is not fixed by the mass and radius alone; the appropriate first-order result is instead $\nu_{\rm em}\approx\nu_{\rm ob}[1+GM/(rc^2)+v^2/(2c^2)]$, with $v$ supplied independently.

## ↑ Ancestors (13)

1. [B4](../b4.md)
2. [Section B](../../section-b.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
