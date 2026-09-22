<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[General relativity](../../../../../general-relativity-split.md) models spacetime by a smooth four-dimensional [Lorentzian manifold](../../../../../lorentzian-manifold.md) whose [metric tensor](../../../../../metric-tensor.md) governs clock readings, causal cones and free-particle motion. The [Einstein equivalence principle](../../../../../einstein-equivalence-principle.md) motivates local [special relativity](../../../../../special-relativity-split.md) and universal [geodesic](../../../../../geodesic.md) [free fall](../../../../../free-fall.md) for test bodies; it does not by itself select a unique gravitational field equation. We assume a [Levi-Civita connection](../../../../../levi-civita-connection.md), a [metric tensor](../../../../../metric-tensor.md) as the gravitational field with no additional dynamical gravitational variables, and matter with a covariantly conserved [stress-energy tensor](../../../../../stress-energy-tensor.md). Units have $c=1$.

The existence of [local inertial frames](../../../../../local-inertial-frame.md) is a local statement. At any regular event choose an [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md) and [Riemann normal coordinates](../../../../../normal-coordinates.md), so that $g_{ab}=\eta_{ab}$ and $\Gamma^a{}_{bc}=0$ at the event, with [metric signature](../../../../../metric-signature.md) $(+---)$. [Metric compatibility](../../../../../metric-compatibility.md) then gives $\partial_cg_{ab}=0$ there. The [geodesic equation](../../../../../geodesic-equation.md) at that point is the special-relativistic inertial equation. Along a [timelike geodesic](../../../../../timelike-geodesic.md), a parallel-transported [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md) gives [Fermi normal coordinates](../../../../../fermi-coordinates.md), eliminating the connection along the central worldline. These constructions do not in general eliminate second derivatives of the [metric tensor](../../../../../metric-tensor.md) in a neighborhood. The [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) is built from the derivatives of the [connection coefficients](../../../../../connection-components.md) as well as their quadratic terms; nonzero [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) components can remain when all [connection coefficients](../../../../../connection-components.md) vanish at a chosen point. Conversely, [Polar coordinates](../../../../../polar-coordinates.md) in [Minkowski spacetime](../../../../../minkowski-spacetime.md) can have nonzero [connection coefficients](../../../../../connection-components.md) but zero [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md). [Connection coefficients](../../../../../connection-components.md) alone are therefore not an invariant measure of gravity.

For the tensorial content, consider a two-parameter family of [geodesics](../../../../../geodesic.md) parametrized by an [affine parameter](../../../../../affine-parameter.md), with tangent $U$ and connecting field $J$. Their coordinate construction gives $[U,J]=0$, and torsion-freeness gives $\nabla_UJ=\nabla_JU$. Since $\nabla_UU=0$, commuting derivatives in the convention of Question 1 yields [geodesic deviation](../../../../../geodesic-deviation.md):

$$
\boxed{\frac{D^2J^a}{d\tau^2}=-R^a{}_{bcd}U^bU^cJ^d.}
$$

The left side is covariant relative acceleration, rather than the second coordinate derivative of an arbitrary separation. In an [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md) in [free fall](../../../../../free-fall.md) with $U=(1,0,0,0)$, its spatial components are $D^2J^i/d\tau^2=-R^i{}_{00j}J^j$. This is a measurable [tidal force](../../../../../tidal-force.md), and a coordinate transformation cannot make a nonzero [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) disappear. It is the distinction between gravity at one event and the behavior of an extended freely falling laboratory.

In a static [Newtonian limit](../../../../../newtonian-limit.md), $g_{00}=1+2\Phi$ and $\Gamma^i{}_{00}=\partial_i\Phi$, so the test-body acceleration is $-\nabla\Phi$. The [curvature-sign convention in Killing derivative identities](../../../../../curvature-sign-convention-in-killing-derivative-identities.md) gives $R^i{}_{00j}\simeq\partial_i\partial_j\Phi$. Hence relative acceleration is the negative [Hessian](../../../../../hessian-matrix.md) of the [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md). For the [Newtonian potential of a point mass](../../../../../newtonian-potential-of-a-point-mass.md) $\Phi=-GM/r$, the [Hessian](../../../../../hessian-matrix.md) has radial [eigenvalue](../../../../../eigenvalue.md) $-2GM/r^3$ and two tangential [eigenvalues](../../../../../eigenvalue.md) $GM/r^3$: radial separations stretch and tangential ones compress. Outside the source the [Ricci tensor](../../../../../ricci-tensor.md) can vanish while the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) remains nonzero. Its vacuum tidal part is encoded by the [Weyl tensor](../../../../../weyl-tensor.md); vacuum does not mean flatness. [Gravitational waves](../../../../../gravitational-wave.md) likewise carry [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) disturbances without a local material source.

To obtain the field equations, make the additional dynamical assumptions explicit: locality and [diffeomorphism invariance of general relativity](../../../../../diffeomorphism-invariance-of-general-relativity.md); a symmetric [metric tensor](../../../../../metric-tensor.md) field equation using at most second derivatives of the [metric tensor](../../../../../metric-tensor.md); a geometrical left-hand side linear in the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) with constant coefficients; and compatibility with local matter conservation. These restrictions exclude higher-curvature or extra-field alternatives. Under them the available rank-two curvature contractions give the ansatz

$$
F_{ab}=aR_{ab}+bRg_{ab}+c_0g_{ab}.
$$

The [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) and [metric compatibility](../../../../../metric-compatibility.md) give

$$
\nabla^aF_{ab}=\left(\frac a2+b\right)\nabla_bR.
$$

For this to vanish identically for arbitrary [metric tensors](../../../../../metric-tensor.md), $b=-a/2$. Assuming $a\ne0$ and absorbing its normalization into the coupling gives

$$
G_{ab}+\Lambda g_{ab}=\kappa T_{ab},\qquad G_{ab}=R_{ab}-\frac12Rg_{ab}.
$$

The permitted constant term is the [cosmological constant](../../../../../cosmological-constant.md). Its value is not fixed by the [Equivalence principle](../../../../../equivalence-principle.md). Conservation of $T$ follows for generally covariant matter on its equations of motion: varying the matter [action](../../../../../action.md) under a compactly supported infinitesimal [diffeomorphism](../../../../../diffeomorphism.md), then integrating its term $T^{ab}\nabla_a\xi_b$ by parts, gives $\nabla_aT^{ab}=0$. The divergence-free [Einstein tensor](../../../../../einstein-tensor.md) is consistent with this identity.

The coupling sign must be fixed in the actual [curvature-sign convention in Killing derivative identities](../../../../../curvature-sign-convention-in-killing-derivative-identities.md), with $R_{ab}=R^c{}_{acb}$. For the static [weak-field approximation](../../../../../weak-field-approximation.md), $R_{00}\simeq-\Delta\Phi$. Set $\Lambda=0$ for the local asymptotically flat Newtonian comparison. In four dimensions the trace equation gives $R=-\kappa T$, so $R_{00}=\kappa(T_{00}-\tfrac12g_{00}T)\simeq\kappa\rho/2$ for slowly moving matter. Matching $\Delta\Phi=4\pi G\rho$ forces $\kappa=-8\pi G$. Thus, with this convention,

$$
\boxed{R_{ab}-\frac12Rg_{ab}+\Lambda g_{ab}=-8\pi GT_{ab}.}
$$

Under the opposite [curvature-sign convention in Killing derivative identities](../../../../../curvature-sign-convention-in-killing-derivative-identities.md) the coupling sign reverses, as in [Einstein-equation coupling under reversed curvature](../../../../../einstein-equation-coupling-under-reversed-curvature.md). This sign statement is compatible with the supplied linearized handout. **[Local inertial frames](../../../../../local-inertial-frame.md) remove the connection at an event; tidal [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) effects remain tensorial, and the field equations require dynamical assumptions beyond the [Equivalence principle](../../../../../equivalence-principle.md).**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
