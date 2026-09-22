<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [strong equivalence principle](../../../../../strong-equivalence-principle.md) asserts universality of free fall even for bodies with gravitational self-binding, together with independence of local experimental outcomes, including gravitational experiments, from the location and velocity of a freely falling laboratory. “Local” means that external tidal variation across the apparatus can be neglected. It does not mean that all curvature, or a laboratory's own gravitational field, can be removed. The weak principle concerns freely falling test bodies without appreciable self-gravity; laboratory composition tests alone therefore do not establish the strong version.

Lunar laser ranging supplies evidence specifically sensitive to the strong version. The Earth and Moon have different fractions of gravitational self-energy. If those fractions affected gravitational and inertial mass differently, their accelerations toward the Sun would differ and the lunar orbit would acquire a periodically varying polarization, the [Nordtvedt effect](../../../../../nordtvedt-effect.md). Combining lunar ranging with laboratory bounds on composition-dependent differential acceleration separates this self-energy effect. A determination available before this examination found the self-energy contribution to the Earth–Moon difference in $m_G/m_I$ to be $(-2.0\pm2.0)\times10^{-13}$, consistent with zero; see [the 2004 experimental analysis](https://arxiv.org/abs/gr-qc/0411113). Universality-of-free-fall experiments, [gravitational redshift](../../../../../gravitational-redshift.md) measurements and tests of local [Lorentz invariance](../../../../../lorentz-invariance.md) support the weaker constituent principles, but should not be confused with a direct self-gravity test.

In [general relativity](../../../../../general-relativity-split.md), all matter couples to one [metric tensor](../../../../../metric-tensor.md), and freely falling test particles follow its [geodesics](../../../../../geodesic.md). At any event, [Riemann normal coordinates](../../../../../normal-coordinates.md) give $g_{ab}=\eta_{ab}$ and $\Gamma^a{}_{bc}=0$. Nongravitational local equations reduce to their special-relativistic forms in that frame. Gravitational binding is governed by the same metric field equations rather than a separate composition-dependent force, and the local gravitational coupling is universal. These features implement the [strong equivalence principle](../../../../../strong-equivalence-principle.md). Curvature still governs [geodesic deviation](../../../../../geodesic-deviation.md), so this construction removes uniform acceleration, not tidal gravity.

To geometrize [Newtonian mechanics](../../../../../newtonian-mechanics.md), use a four-dimensional manifold with coordinates $(t,x^1,x^2,x^3)$, absolute time $\tau_a=(dt)_a$ and a degenerate spatial inverse metric $h^{ij}=\delta^{ij}$, $h^{0a}=0$. For a [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) $\Phi(t,x)$ define the torsion-free [Newton–Cartan gravitational connection](../../../../../newton-cartan-gravitational-connection.md) by

$$
\Gamma^i{}_{00}=\partial_i\Phi,\qquad\text{all other coefficients zero}.
$$

It satisfies $\nabla_a\tau_b=0$ and $\nabla_a h^{bc}=0$. An affine [geodesic](../../../../../geodesic.md) has $d^2t/d\lambda^2=0$; choosing $\lambda=t$ makes its spatial equations

$$
\boxed{\frac{d^2x^i}{dt^2}+\partial_i\Phi=0.}
$$

This is Newton's free-fall law. The geometry is [Newton–Cartan theory](../../../../../newton-cartan-theory.md), with an [affine connection](../../../../../affine-connection.md) and degenerate metric data, rather than a nondegenerate four-dimensional Lorentzian metric. The spatial slices themselves remain Euclidean.

Use the curvature convention

$$
[\nabla_c,\nabla_d]V^a=R^a{}_{bcd}V^b,\qquad
R^a{}_{bcd}=\partial_c\Gamma^a{}_{db}-\partial_d\Gamma^a{}_{cb}
+\Gamma^a{}_{ce}\Gamma^e{}_{db}-\Gamma^a{}_{de}\Gamma^e{}_{cb}.
$$

In these coordinates the quadratic connection terms vanish, and the only nonzero curvature components, apart from antisymmetry in $c,d$, are

$$
\boxed{R^i{}_{0j0}=\partial_j\partial_i\Phi,\qquad R^i{}_{00j}=-\partial_j\partial_i\Phi.}
$$

In particular $R_{00}=\nabla^2\Phi$ and all other components of the [Ricci tensor](../../../../../ricci-tensor.md) vanish. This [Newtonian tidal curvature](../../../../../newtonian-tidal-curvature.md) gives relative acceleration $\delta\ddot x^i=-\partial_i\partial_j\Phi\,\delta x^j$. Spatially constant gravitational acceleration can be removed by an accelerating frame because its Hessian vanishes. The [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) becomes $R_{ab}=4\pi G\rho\,\tau_a\tau_b$. Fluid mechanics is compatible with the same connection: the covariant continuity equation is the usual mass-conservation equation, and the spatial Euler equation is $u^b\nabla_bu^i=-\rho^{-1}\partial_i p$, which includes the gravitational force through the connection.

Now replace this absolute-time geometry by the Lorentzian metric of [general relativity](../../../../../general-relativity-split.md), with signature $(-,+,+,+)$. A [perfect fluid](../../../../../perfect-fluid.md) has

$$
T_{ab}=(\varepsilon+p)U_aU_b+p g_{ab},\qquad U^aU_a=-1,
$$

where $\varepsilon$ is rest-frame energy density. In units $c=1$, $\varepsilon\simeq\rho$ for a nonrelativistic fluid. The Newtonian equation suggests a covariant curvature equation sourced by $T_{ab}$. However $R_{ab}=\kappa T_{ab}$ alone conflicts with generic [stress-energy conservation](../../../../../stress-energy-conservation.md), because the [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) gives $\nabla^aR_{ab}=\tfrac12\nabla_bR$. Among expressions linear in Ricci curvature, conservation therefore selects

$$
G_{ab}=R_{ab}-\tfrac12Rg_{ab},\qquad \nabla^aG_{ab}=0.
$$

A constant multiple of the metric is also divergence-free, giving the possible [cosmological constant](../../../../../cosmological-constant.md) term. This is a heuristic selection using locality, universal metric coupling and second-order metric equations; Newtonian matching by itself does not prove uniqueness among every possible gravity theory.

To fix the coefficient, first set the cosmological constant to zero. The trace-reversed equation would read $R_{ab}=\kappa(T_{ab}-\tfrac12Tg_{ab})$. In the fluid rest frame, $T=-\varepsilon+3p$, so $R_{00}=\tfrac\kappa2(\varepsilon+3p)$. In the weak static [Newtonian limit](../../../../../newtonian-limit.md), $g_{00}=-(1+2\Phi)$ and $R_{00}\simeq\nabla^2\Phi$. For negligible pressure the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) then requires $\kappa/2=4\pi G$. Restoring $c$ uses $x^0=ct$, $R_{00}\simeq\nabla^2\Phi/c^2$ and $T_{00}\simeq\rho c^2$, giving $\kappa=8\pi G/c^4$. Thus

$$
\boxed{R_{ab}-\frac12Rg_{ab}+\Lambda g_{ab}=\frac{8\pi G}{c^4}T_{ab}.}
$$

Pressure contributes to relativistic active gravity, while the low-pressure weak-field limit recovers Newton's Poisson equation. The comparison fixes the Newtonian normalization but does not fix $\Lambda$, which is an independent parameter.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
