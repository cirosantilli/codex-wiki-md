<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [perfect fluid in general relativity](../../../../perfect-fluid-in-general-relativity.md), let $\rho$ be rest-frame total [energy](../../../../energy-split.md) density divided by $c^2$, $P$ its isotropic [pressure](../../../../pressure-split.md), and $U^\mu$ its [four-velocity](../../../../four-velocity.md), normalized by $U^\mu U_\mu=-c^2$. Then

$$
T^{\mu\nu}=\left(\rho+\frac{P}{c^2}\right)U^\mu U^\nu+Pg^{\mu\nu}.
$$

The [contracted Bianchi identity](../../../../contracted-bianchi-identity.md) and the [Einstein field equations](../../../../einstein-field-equations-split.md) give [stress-energy conservation](../../../../stress-energy-conservation.md), $\nabla_\mu T^{\mu\nu}=0$, for a constant [cosmological constant](../../../../cosmological-constant.md). Contract with $U_\nu$ and use the normalization to obtain

$$
U^\mu\partial_\mu\rho+\left(\rho+\frac{P}{c^2}\right)\nabla_\mu U^\mu=0.
$$

In [comoving coordinates](../../../../comoving-coordinate.md) $U^\mu=(1,0,0,0)$ and the [covariant divergence](../../../../covariant-divergence.md) is $\nabla_\mu U^\mu=3\dot R/R=3H$, where a dot is a [cosmic time](../../../../cosmic-time.md) [derivative](../../../../derivative.md) and $H$ the [Hubble parameter](../../../../hubble-parameter.md). Therefore

$$
\boxed{\dot\rho+3H\left(\rho+\frac{P}{c^2}\right)=0.}
$$

For a fixed region in [comoving coordinates](../../../../comoving-coordinate.md), let $V(t)=V_*R^3(t)$ be its physical [volume](../../../../volume.md), where $V_*$ is a fixed coordinate-volume integral, and let $E=\rho c^2V$. Since $\dot V=3HV$,

$$
\frac{dE}{dt}+P\frac{dV}{dt}
=c^2V\left[\dot\rho+3H\left(\rho+\frac{P}{c^2}\right)\right]=0.
$$

Thus the [cosmological perfect-fluid continuity equation](../../../../cosmological-perfect-fluid-continuity-equation.md) is exactly equivalent to the adiabatic [first law of thermodynamics](../../../../first-law-of-thermodynamics-split.md), $\boxed{dE=-P\,dV}$, for every nonzero such region. Conversely, expanding that [first law of thermodynamics](../../../../first-law-of-thermodynamics-split.md) and dividing by $c^2V$ recovers the same equation. No [heat](../../../../heat-split.md) or [particle](../../../../particle-physics.md) flux crosses the comoving boundary; interacting components separately need source terms, although the total still obeys this conservation equation.

There is a sign inconsistency in the supplied formula sheet worth isolating. Its [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) and [Ricci tensor](../../../../ricci-tensor.md) conventions, together with its stated $-+++$ [metric signature](../../../../metric-signature.md), give $G_{tt}=-3H^2$ for $R(t)=e^{Ht}$ with constant $H$. Its vacuum [Einstein field equations](../../../../einstein-field-equations-split.md) with $+\Lambda g_{\mu\nu}$ then require $H^2=-\Lambda c^2/3$, whereas its printed vacuum [Friedmann equation](../../../../friedmann-equations.md) gives $H^2=+\Lambda c^2/3$. For example, $H>0$, $\rho=P=0$ and $\Lambda=3H^2/c^2$ satisfy the latter but leave the former's $tt$ component equal to $-6H^2$. Changing the geometric [cosmological constant](../../../../cosmological-constant.md) term to $-\Lambda g_{\mu\nu}$ repairs this mismatch. The conservation derivation is unaffected; below take the geometric [cosmological constant](../../../../cosmological-constant.md) to be zero and include any [vacuum energy](../../../../vacuum-energy.md) as a fluid, so no ambiguous sign enters.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
