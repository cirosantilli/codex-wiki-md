<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [anti-dynamo theorem](../../../../../anti-dynamo-theorem.md) identifies a restriction that prevents a conducting fluid from regenerating its [magnetic field](../../../../../magnetic-field.md) against resistive losses. The hypotheses matter: throughout the following arguments take positive uniform [magnetic diffusivity](../../../../../magnetic-diffusivity.md), smooth fields, no imposed magnetic source, and the stated isolated or energy-closed boundary conditions. An [anti-dynamo theorem](../../../../../anti-dynamo-theorem.md) does not rule out transient magnetic amplification, winding of an imposed field, or an externally supplied [magnetic flux](../../../../../magnetic-flux.md). The [resistive induction equation](../../../../../resistive-induction-equation.md) is the common starting point:

$$
\mathbf B_t=\nabla\times(\mathbf u\times\mathbf B)+\eta\nabla^2\mathbf B,\qquad\nabla\cdot\mathbf B=0.
$$

First consider [Backus' necessary condition for dynamo action](../../../../../backus-necessary-condition-for-dynamo-action.md). For a conductor contained in a sphere of radius $a$, include the potential field in the insulating exterior when defining the total [magnetic energy](../../../../../magnetic-energy.md):

$$
E_B=\frac1{2\mu_0}\int_{\mathbb R^3}|\mathbf B|^2\,dV.
$$

For an [incompressible flow](../../../../../incompressible-flow.md), with boundary conditions eliminating the mechanical surface term, such as a [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) for the fluid, [integration by parts](../../../../../integration-by-parts.md) gives

$$
\frac{dE_B}{dt}=\frac1{\mu_0}\int_D B_i e_{ij}B_j\,dV
-\frac\eta{\mu_0}\int_D|\nabla\times\mathbf B|^2\,dV,
$$

where $e_{ij}=(\partial_i u_j+\partial_j u_i)/2$ is the [rate-of-strain tensor](../../../../../strain-rate-tensor.md). Its antisymmetric part does no stretching, since $B_iB_j$ is symmetric. If $S$ bounds the largest [eigenvalue](../../../../../eigenvalue.md) of $e$ throughout the flow, the first term is at most $2SE_B$.

The [magnetic free-decay spectral bound](../../../../../magnetic-free-decay-spectral-bound.md) for the enclosing insulating sphere is

$$
\int_D|\nabla\times\mathbf B|^2\,dV\geq\frac{\pi^2}{a^2}\int_{\mathbb R^3}|\mathbf B|^2\,dV.
$$

The exterior energy is essential to this variational estimate. Its constant comes from the slowest freely decaying dipolar poloidal mode: the spherical radial matching condition reduces to $j_0(\kappa a)=0$, whose first positive root is $\kappa a=\pi$. Expanding an admissible field in the orthogonal free-decay modes, or using their variational characterization, gives the bound. A smaller conductor can only increase the minimum dissipation quotient for the enclosing-sphere comparison. Combining the two estimates yields

$$
\frac{dE_B}{dt}\leq2\left(S-\frac{\eta\pi^2}{a^2}\right)E_B.
$$

Thus

$$
\boxed{\frac{Sa^2}{\eta}\geq\pi^2\quad\text{is necessary for sustained dynamo action}.}
$$

Below this threshold the [Gronwall inequality](../../../../../gronwall-inequality.md) gives exponential energy decay. Above it the estimate merely permits growth; it does not prove that the geometry regenerates the field. A time-dependent version bounds the field-amplitude exponent by the time average of the maximum strain minus the diffusive rate.

The geometric obstruction in [Cowling anti-dynamo theorem](../../../../../cowling-anti-dynamo-theorem.md) is different: an isolated exactly axisymmetric [magnetic field](../../../../../magnetic-field.md) cannot be self-maintained. To see the missing regeneration mechanism, write its [poloidal magnetic field](../../../../../poloidal-magnetic-field.md) in terms of the [poloidal magnetic flux function](../../../../../poloidal-magnetic-flux-function.md) $\psi$:

$$
B_r=-\frac1r\psi_z,\qquad B_z=\frac1r\psi_r.
$$

The poloidal part of the [resistive induction equation](../../../../../resistive-induction-equation.md) becomes

$$
\psi_t+u_r\psi_r+u_z\psi_z=\eta\left(\psi_{rr}-\frac1r\psi_r+\psi_{zz}\right).
$$

There is no term containing $B_\phi$ that creates new poloidal flux. Fix the gauge by setting $\psi=0$ on the regular symmetry axis, and match to a decaying exterior field with no imposed flux. At a positive interior maximum away from the axis, the advective term vanishes and the diffusive term is nonpositive. The [parabolic comparison principle](../../../../../parabolic-comparison-principle.md) therefore prevents increase of the maximum; it likewise prevents decrease of a negative minimum. In the steady problem the [strong maximum principle](../../../../../strong-maximum-principle-for-elliptic-operators.md), regularity at the axis and decay outside exclude a nonzero maximum altogether. Matching to the insulating exterior does not create a maximum at the interface: the exterior flux is harmonic in the corresponding axisymmetric operator, and the two normal-derivative conditions exclude such an interface extremum. The same homogeneous scalar diffusion problem gives decay in time on a bounded conductor with no replenishing boundary data.

Once the poloidal field has decayed, let $b=B_\phi/r$ and let $\Omega_f=u_\phi/r$ denote the fluid's angular velocity. Its equation is

$$
b_t+\mathbf u_p\cdot\nabla b=\mathbf B_p\cdot\nabla\Omega_f
+\eta\left(b_{rr}+\frac3r b_r+b_{zz}\right).
$$

Differential rotation can make toroidal field from poloidal field, but it cannot close the reverse loop. When $\mathbf B_p=0$, this too is a homogeneous advection-diffusion equation, with a regular axis and zero toroidal field at an insulating exterior. Hence it cannot sustain the remaining field. **The exactly axisymmetric field, rather than merely an axisymmetric velocity, is excluded.** If an exactly axisymmetric field were maintained by a nonaxisymmetric velocity, averaging the linear induction equation in azimuth would replace that velocity by its azimuthal mean and give the same contradiction. An [axisymmetric flow](../../../../../axisymmetric-flow.md) can, however, excite a nonaxisymmetric field. Also an axisymmetric averaged field in [mean-field dynamo theory](../../../../../mean-field-dynamo.md) has an additional fluctuating electromotive force, so this unmodified scalar proof does not apply to it.

The [toroidal-velocity anti-dynamo theorem](../../../../../toroidal-velocity-anti-dynamo-theorem.md) restricts the flow instead. In a conducting sphere, suppose $\mathbf u\cdot\mathbf x=0$, so the [incompressible flow](../../../../../incompressible-flow.md) is tangent to every concentric sphere. No assumption of axisymmetry is made. Define $P=\mathbf x\cdot\mathbf B$. A direct Cartesian calculation is particularly useful:

$$
(\partial_t+\mathbf u\cdot\nabla)P
=\mathbf B\cdot\nabla(\mathbf u\cdot\mathbf x)+\eta\mathbf x\cdot\nabla^2\mathbf B
=\eta\nabla^2P.
$$

The last equality uses $\nabla\cdot\mathbf B=0$, so $\nabla^2(\mathbf x\cdot\mathbf B)=\mathbf x\cdot\nabla^2\mathbf B$. Thus the radial magnetic scalar is a passive diffusing scalar, not a regenerated field. Multiplying by $P$, integrating over the sphere and using tangential incompressible advection gives

$$
\frac12\frac d{dt}\int_D P^2\,dV
=-\eta\int_D|\nabla P|^2\,dV+\eta\int_{\partial D}P\partial_nP\,dS.
$$

In an insulating exterior, a [spherical harmonic](../../../../../spherical-harmonic.md) component of degree $l\geq1$ has $P\propto r^{-l-1}$, so its boundary contribution is negative: $\partial_nP=-(l+1)P/a$. The monopole component is absent because the [magnetic field](../../../../../magnetic-field.md) is solenoidal and regular. The resulting dissipative scalar problem makes $P$, and hence the poloidal field, decay.

When that radial field is absent, the remaining tangential solenoidal field can be written $\mathbf B=\nabla\times(T\mathbf x)$. Its induction equation reduces to a second passive scalar equation. Indeed

$$
\mathbf u\times\mathbf B=-\mathbf x(\mathbf u\cdot\nabla T),\qquad
\nabla^2(T\mathbf x)=\mathbf x\nabla^2T+2\nabla T,
$$

and the curl of the last gradient term is zero. Therefore $T_t+\mathbf u\cdot\nabla T=\eta\nabla^2T$, up to an irrelevant radial gauge function, which can be removed by taking the angular mean of $T$ to be zero. Its angular variations vanish at the insulating spherical boundary, so this scalar also decays by its quadratic energy identity. Equivalently, a putative growing magnetic normal mode must first have $P=0$, after which the scalar $T$ equation rules it out. **Purely toroidal spherical flow cannot close a dynamo regeneration loop, even if it is nonaxisymmetric.** This does not assert that purely poloidal flow is always incapable of a dynamo, or that any azimuthally directed cylindrical flow is governed by the same spherical theorem.

Other restrictions illuminate the same distinction between stretching and regeneration. The [planar anti-dynamo theorem](../../../../../planar-anti-dynamo-theorem.md) has a similar scalar proof in the usual two-dimensional geometry. For planar [velocity](../../../../../velocity.md) and [magnetic field](../../../../../magnetic-field.md) independent of the third coordinate, write the in-plane field as $\nabla\times(A\hat{\mathbf z})$. Its [vector potential](../../../../../vector-potential.md) obeys $A_t+\mathbf u\cdot\nabla A=\eta\Delta A$ after fixing the gauge, so $\frac12\frac d{dt}\int A^2=-\eta\int|\nabla A|^2$ under periodic or homogeneous energy-closed boundary conditions. A third field component independent of that coordinate is also a passive scalar. A spatially uniform imposed field may survive in a periodic box but is not regenerated dynamo field. Three-component motions depending on only two coordinates are not covered by this strictly planar formulation.

There are also necessary bounds in terms of velocity amplitude rather than strain. The magnetic work term is bounded by $\|\mathbf u\|_\infty\|\mathbf B\|_2\|\nabla\times\mathbf B\|_2$; combining this with the same free-decay inequality gives a velocity-based lower threshold on the [magnetic Reynolds number](../../../../../magnetic-reynolds-number.md). These bounds, like [Backus' necessary condition for dynamo action](../../../../../backus-necessary-condition-for-dynamo-action.md), are necessary rather than sufficient. Pure motion that only rearranges a scalar magnetic potential cannot evade diffusion merely by becoming faster. Conversely the stagnation-flow energy amplification in Question 2 does not contradict the bounded-body theorems: it uses an unbounded three-dimensional strain field and, for its growing finite-energy modes, a slowly decaying field at infinity. Similarly, the [torsional Alfvén waves](../../../../../torsional-alfven-wave.md) in Question 3 transfer energy between velocity and a toroidal perturbation about a prescribed background; they are not a construction of that background by dynamo action. **The anti-dynamo results identify failed regeneration mechanisms and the assumptions under which those failures are rigorous.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
