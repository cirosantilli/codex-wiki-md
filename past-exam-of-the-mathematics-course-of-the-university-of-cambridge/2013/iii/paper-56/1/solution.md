<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $M=M_1+M_2$, and let $\mu=M_1M_2/M$ be the [reduced mass](../../../../../reduced-mass.md). The stellar distances from the [center of mass](../../../../../center-of-mass.md) are $a_1=aM_2/M$ and $a_2=aM_1/M$. For a [circular Kepler orbit](../../../../../circular-kepler-orbit.md), $\Omega^2=GM/a^3$, so summing the two orbital contributions gives the **[circular-binary orbital angular momentum](../../../../../circular-binary-orbital-angular-momentum.md)**

$$
J_{\mathrm{orb}}=(M_1a_1^2+M_2a_2^2)\Omega
=\mu a^2\Omega
=\boxed{\frac{M_1M_2}{M}\sqrt{GMa}.}
$$

The separation $a$ is inside the square root. This also has the required dimensions of [angular momentum](../../../../../angular-momentum.md).

For the [homologous rotating collapse](../../../../../homologous-rotating-collapse.md), label a fluid element by $s=r/R$ and its polar angle $\theta$. Its enclosed mass $m(s)$ is constant during [stellar homology](../../../../../stellar-homology.md), as are the dimensionless density profile and the inertia coefficient $\alpha$. [Conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) and [solid-body rotation](../../../../../solid-body-rotation.md) give

$$
\Omega=\frac{J}{\alpha MR^2}.
$$

The magnitude of the [centrifugal acceleration](../../../../../centrifugal-acceleration.md) is $\Omega^2r\sin\theta$, while the [Newtonian gravitational field](../../../../../newtonian-gravitational-field.md) has magnitude $Gm(s)/r^2$. Therefore

$$
\boxed{\frac{F_{\mathrm{cent}}}{F_{\mathrm{grav}}}=\frac{\Omega^2r^3\sin\theta}{Gm(s)}
=\frac{J^2s^3\sin\theta}{\alpha^2GM^2m(s)}\frac1R\ \propto R^{-1}.}
$$

Using only the radial component of centrifugal force replaces $\sin\theta$ by $\sin^2\theta$ and leaves the scaling unchanged. The centrifugal force vanishes on the rotation axis; the central point is understood through the limiting field rather than a ratio of two zero forces.

At the equator of the cloud, [critical rotation of a spherical cloud](../../../../../critical-rotation-of-a-spherical-cloud.md) means $\Omega_c^2R_c=GM/R_c^2$, where $R_c=R_{\mathrm{crit}}$. Consequently

$$
J=\alpha M\sqrt{GMR_c},\qquad R_c=\frac{J^2}{\alpha^2GM^3}.
$$

Immediately after the first fission, each daughter has mass $M/2$ and radius $a/2$ because the spheres touch. Their orbital [moment of inertia](../../../../../moment-of-inertia.md) is $Ma^2/4$, while their combined spin [moment of inertia](../../../../../moment-of-inertia.md) is $\alpha Ma^2/4$. With a common spin and orbital frequency $\Omega_f=\sqrt{GM/a^3}$, the [synchronous fission model for binary formation](../../../../../synchronous-fission-model-for-binary-formation.md) gives

$$
J=\frac{1+\alpha}{4}M\sqrt{GMa}.
$$

The common frequency can change during fission; corotation requires equal instantaneous frequencies, not an unchanged frequency from before the rearrangement. Equating the two values of $J$ yields

$$
\boxed{\frac a{R_c}=\frac{16\alpha^2}{(1+\alpha)^2}.}
$$

For a nonzero positive inertia coefficient, the **necessary and sufficient condition in this algebraic model for $a<R_c$** is

$$
\boxed{0<\alpha<\frac13.}
$$

For example, a [moment of inertia of a uniform solid sphere](../../../../../moment-of-inertia-of-a-uniform-solid-sphere.md) has $\alpha=2/5$ and gives $a/R_c=64/49>1$; it fails the required compact-fission condition. A sufficiently centrally concentrated cloud can have smaller $\alpha$.

For the next collapse, neglect exchange of spin with the unchanged outer orbit, so each daughter's spin [angular momentum](../../../../../angular-momentum.md) is separately conserved. Immediately after the first fission that spin is

$$
S_d=\alpha\frac M2\left(\frac a2\right)^2\Omega_f
=\frac{\alpha M}{8}\sqrt{GMa}.
$$

For a daughter of mass $m=M/2$ to reach [critical rotation of a spherical cloud](../../../../../critical-rotation-of-a-spherical-cloud.md) at radius $R_{c,d}$, the same relation gives $S_d=\alpha m\sqrt{GmR_{c,d}}$. Hence

$$
\boxed{R_{c,d}=\frac a8.}
$$

Equivalently, its centrifugal-to-gravity ratio starts at $1/4$ when its radius is $a/2$ and reaches one after contraction by a factor four. Applying the same fission rule to this daughter produces an inner pair with separation

$$
\boxed{\frac{a'}a=\frac{16\alpha^2}{(1+\alpha)^2}\frac18
=\frac{2\alpha^2}{(1+\alpha)^2}.}
$$

Corotation at this second fission is local to each newly formed inner pair; it is not a single common frequency for the entire four-star hierarchy.

This spin assumption matters. If [tidal locking](../../../../../tidal-locking.md) instead kept each shrinking daughter synchronized to the fixed outer [orbital period](../../../../../orbital-period.md) throughout the intervening collapse, its [angular velocity](../../../../../angular-velocity.md) would remain fixed. Its centrifugal-to-gravity ratio would then scale as $R_d^3$ and decrease, so it would never reach the proposed second fission. This is a counterexample to extending the corotation assumption through the whole contraction. The printed ratio describes the separately spin-conserving interpretation of the [repeated fission hierarchy](../../../../../repeated-fission-hierarchy.md).

**The model can generate a compact hierarchy algebraically, but is not a general physical account of multiple-star formation.** In the allowed range $\alpha<1/3$, one has $a'/a<1/8$, suggesting well-separated inner and outer scales. However, rapidly rotating gas deforms, touching daughters are tidally distorted, and pressure, gas flows, dissipation and spin-orbit torques cannot generally be ignored. The assumed identical profiles, equal mass splits, instantaneous corotation and later torque-free contractions are restrictive. [Star formation](../../../../../star-formation.md) can involve [gravitational fragmentation](../../../../../gravitational-fragmentation.md) and redistribution of [angular momentum](../../../../../angular-momentum.md); the toy budget neither proves that fission occurs nor predicts the population of real multiple systems.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
