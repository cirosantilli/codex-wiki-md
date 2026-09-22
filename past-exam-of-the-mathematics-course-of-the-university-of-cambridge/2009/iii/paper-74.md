# Paper 74

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper74.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper74.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
  - [vi](#1/vi)
    - [Solution](#1/vi/solution)
  - [vii](#1/vii)
    - [Solution](#1/vii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 74](paper-74.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For a fixed fluid domain, consider an incompressible Newtonian [Stokes flow](../../../stokes-flow.md) with prescribed [velocities](../../../classical-mechanics.md#velocity) on its boundaries and prescribed far-field behaviour. Conservative body [forces](../../../classical-mechanics.md#force), such as gravity, may be absorbed into the [pressure](../../../thermodynamics.md#pressure). Among all sufficiently regular divergence-free trial [velocity fields](../../../fluid-mechanics.md#velocity-field) with exactly those boundary [velocities](../../../classical-mechanics.md#velocity) and far-field behaviour, the Stokes solution minimizes the [viscous dissipation](../../../stokes-flow.md#viscous-dissipation)

$$
\mathcal D[\mathbf u]=2\mu\int_{\mathcal D}e_{ij}(\mathbf u)e_{ij}(\mathbf u)\,dV,
\qquad e_{ij}=\tfrac12(\partial_i u_j+\partial_j u_i).
$$

To see this [Minimum-dissipation theorem for Stokes flow](../../../stokes-flow.md#minimum-dissipation-theorem-for-stokes-flow), write a trial field as $\mathbf v=\mathbf u+\mathbf w$, with $\nabla\cdot\mathbf w=0$ and homogeneous [velocity](../../../classical-mechanics.md#velocity) boundary data. The [Newtonian fluid stress tensor](../../../viscous-fluid-flow.md#newtonian-fluid-stress-tensor) satisfies $\nabla\cdot\boldsymbol\sigma=0$, so integration by parts gives

$$
2\mu\int e(\mathbf u):e(\mathbf w)\,dV
=\int\boldsymbol\sigma:\nabla\mathbf w\,dV=0.
$$

Therefore

$$
\boxed{\mathcal D[\mathbf v]-\mathcal D[\mathbf u]
=2\mu\int e(\mathbf w):e(\mathbf w)\,dV\geq0.}
$$

Equality requires the difference to be a [rigid motion](../../../geometry-and-topology.md#rigid-transformation), eliminated by the fixed wall and far-field data. The theorem varies the [velocity field](../../../fluid-mechanics.md#velocity-field) in one fixed geometry; it does not minimize over particle positions. If a nonconservative body [force](../../../classical-mechanics.md#force) is prescribed, the appropriate variational functional also includes its work, rather than being the dissipation alone.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Neglect tube-end effects and use the localized flow with no imposed throughflow, as implied by the [sphere](../../../geometry-and-topology.md#sphere) being the only cause of motion. Extend the fluid [velocity](../../../classical-mechanics.md#velocity) through the [sphere](../../../geometry-and-topology.md#sphere) by its rigid-body [velocity](../../../classical-mechanics.md#velocity). This extended field is continuous across the surface by the [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) and divergence-free both inside and outside. The divergence theorem therefore makes its total flux through a complete tube section independent of height. In sections far from the [sphere](../../../geometry-and-topology.md#sphere) the fluid is quiescent, so this total flux is zero.

At height $z$ cutting the [sphere](../../../geometry-and-topology.md#sphere), let $A_s(z)$ be the area of its circular slice and take $z$ upward. The translation contributes $V_zA_s$. The vertical component of $\boldsymbol\Omega\times(\mathbf x-\mathbf x_c)$ integrates to zero over that circle because its first moments about the centre vanish. Hence the [zero total flux for localized tube Stokes flow](../../../stokes-flow.md#zero-total-flux-for-localized-tube-stokes-flow) gives

$$
\boxed{Q_f(z)=-V_zA_s(z)>0,}
$$

where $V_z<0$ for a falling [sphere](../../../geometry-and-topology.md#sphere). Thus the net fluid flux is upwards in every section intersecting the [sphere](../../../geometry-and-topology.md#sphere)'s interior, even though some fluid locally moves downwards. At a tangential section $A_s=0$ and the flux vanishes. The zero-total-flux condition is important: an imposed throughflow or appreciable open-tube end effects would change this argument.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

The [Minimum-dissipation theorem for Stokes flow](../../../stokes-flow.md#minimum-dissipation-theorem-for-stokes-flow) compares fields with fixed geometry and boundary [velocities](../../../classical-mechanics.md#velocity). Moving the [sphere](../../../geometry-and-topology.md#sphere) changes the geometry, while sedimentation prescribes its effective weight rather than its [velocity](../../../classical-mechanics.md#velocity). It therefore supplies no rule for migrating toward a position of least dissipation. Indeed, at fixed [force](../../../classical-mechanics.md#force) $W$, the power is $WV$, and a lower drag resistance gives a larger settling speed and larger power, rather than a smaller power. This is a [fixed-force comparison of minimum viscous dissipation](../../../stokes-flow.md#fixed-force-comparison-of-minimum-viscous-dissipation) issue.

The proposed migration is itself false in ideal [Stokes flow](../../../stokes-flow.md). Reflect the uniform vertical tube in a horizontal plane through the [sphere](../../../geometry-and-topology.md#sphere) centre. The [sphere](../../../geometry-and-topology.md#sphere)'s lateral position is unchanged, but the applied axial [force](../../../classical-mechanics.md#force) reverses. Reflection leaves a transverse translational [velocity](../../../classical-mechanics.md#velocity) unchanged. By [Linearity of Stokes flow](../../../stokes-flow.md#linearity-of-stokes-flow), however, reversing the [force](../../../classical-mechanics.md#force) reverses that transverse [velocity](../../../classical-mechanics.md#velocity). It must therefore be zero. This proves [no lateral migration of a single sphere in a uniform tube in Stokes flow](../../../stokes-flow.md#no-lateral-migration-of-a-single-sphere-in-a-uniform-tube-in-stokes-flow):

$$
\boxed{\text{a single rigid sphere retains its distance from the tube centreline}.}
$$

Rotation and a wall-dependent vertical speed are allowed. Inertial lift, particle deformation or tube-end effects belong to different problems and do not follow from the dissipation theorem.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Let downward [velocity](../../../classical-mechanics.md#velocity) be positive in this part, and let $W>0$ be the dense [sphere](../../../geometry-and-topology.md#sphere)'s weight minus [buoyancy](../../../fluid-mechanics.md#buoyancy). For the original centreline configuration, write its six-component translation-and-rotation [velocity](../../../classical-mechanics.md#velocity) as $q$, and its diagonal positive [hydrodynamic resistance matrix](../../../stokes-flow.md#hydrodynamic-resistance-matrix) as $R_0$. Its single-sphere dissipation is

$$
D_0(q)=q^TR_0q=R_{zz}V_z^2+\sum_{\beta\ne z}R_{\beta\beta}q_\beta^2.
$$

With only axial [force](../../../classical-mechanics.md#force) and no [torque](../../../classical-mechanics.md#torque), the original [velocity](../../../classical-mechanics.md#velocity) is $V_0=W/R_{zz}$.

Now add the neutral [sphere](../../../geometry-and-topology.md#sphere). In its actual [Stokes flow](../../../stokes-flow.md), extend the [velocity](../../../classical-mechanics.md#velocity) rigidly through the new [sphere](../../../geometry-and-topology.md#sphere)'s interior. This extension is a valid incompressible trial field for the domain without that [sphere](../../../geometry-and-topology.md#sphere), with exactly the dense [sphere](../../../geometry-and-topology.md#sphere)'s actual six boundary [velocities](../../../classical-mechanics.md#velocity); its strain and dissipation inside the inserted ball are zero. The [Minimum-dissipation theorem for Stokes flow](../../../stokes-flow.md#minimum-dissipation-theorem-for-stokes-flow) and [extra dissipation due to a rigid inclusion](../../../stokes-flow.md#extra-dissipation-due-to-a-rigid-inclusion) therefore give

$$
D\geq D_0(q)\geq R_{zz}V_z^2.
$$

The neutral [sphere](../../../geometry-and-topology.md#sphere) has zero net external [force](../../../classical-mechanics.md#force) and [torque](../../../classical-mechanics.md#torque), and the dense [sphere](../../../geometry-and-topology.md#sphere) has only the axial [force](../../../classical-mechanics.md#force) $W$. The dissipation equals total external power, so $D=WV_z$. Positivity gives $V_z>0$, and the comparison yields $V_z\leq W/R_{zz}$ without assuming that either [sphere](../../../geometry-and-topology.md#sphere) translates only vertically or that either angular [velocity](../../../classical-mechanics.md#velocity) vanishes.

For a finite nonoverlapping placement, the first inequality is strict. Equality would make the extended field the old Stokes solution and thus make that solution rigid throughout the added ball. Analyticity and connectedness then [force](../../../classical-mechanics.md#force) its strain to vanish throughout the original fluid domain; the stationary tube wall and quiescent far field would [force](../../../classical-mechanics.md#force) the whole motion to vanish, contradicting $V_z>0$. Hence the [force-free inclusion reduces axial mobility of a centred settling sphere](../../../stokes-flow.md#force-free-inclusion-reduces-axial-mobility-of-a-centred-settling-sphere):

$$
\boxed{0<V_z<V_0.}
$$

The difference tends to zero as the added [sphere](../../../geometry-and-topology.md#sphere) recedes infinitely far away. The lateral and rotational contributions are nonnegative in the resistance comparison, which is precisely why they cannot invalidate the bound.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Let $\delta\ll a$ be the minimum gap as the [spheres](../../../geometry-and-topology.md#sphere) approach, and $w=-\dot\delta>0$ their normal relative approach speed. For smooth equal-radius [spheres](../../../geometry-and-topology.md#sphere) the gap has local form $\delta+O(s^2/a)$, so the thin-gap region has lateral scale $\ell\sim(a\delta)^{1/2}$. [Incompressibility](../../../fluid-mechanics.md#incompressible-flow) drives a radial escape speed of order $w\ell/\delta$. The [lubrication pressure](../../../viscous-fluid-flow.md#lubrication-pressure) therefore scales as

$$
p\sim\mu\frac{w\ell^2}{\delta^3}\sim\frac{\mu aw}{\delta^2},\qquad
F_n\sim p\ell^2\sim\frac{\mu a^2w}{\delta}.
$$

The available gravitational forcing remains finite. Thus [lubrication resistance](../../../viscous-fluid-flow.md#lubrication-resistance) gives $w=O(W\delta/(\mu a^2))$: the normal approach becomes proportionally slower as the gap closes. In particular, for a bounded coefficient $C$, $\dot\delta\geq-C\delta$, so $\delta(t)\geq\delta(t_1)e^{-C(t-t_1)}>0$ at every finite time. Equivalently the estimated time to reach zero contains $\int_0^{\delta_1}d\delta/\delta$, which diverges. This is how [lubrication prevents finite-time collision of smooth spheres](../../../viscous-fluid-flow.md#lubrication-prevents-finite-time-collision-of-smooth-spheres).

The small nonzero initial lateral offset breaks the exactly collinear configuration; the [spheres](../../../geometry-and-topology.md#sphere) can deflect sideways and pass with a positive gap rather than touch. The condition $R>2a$ leaves space for a side-by-side passage. Smooth surfaces, continuum hydrodynamics and the [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) are essential to the noncontact conclusion; the argument is not a model of surface roughness or molecular contact.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#1/vi)

Choose time $t_c$ when the passing [sphere](../../../geometry-and-topology.md#sphere) centres are at the same height, and let $S$ reflect positions in that horizontal plane. For each instantaneous configuration, [Stokes flow](../../../stokes-flow.md) determines particle [velocities](../../../classical-mechanics.md#velocity) uniquely and linearly from the fixed external [forces](../../../classical-mechanics.md#force). Time reversal reverses all [velocities](../../../classical-mechanics.md#velocity) and the dense [sphere](../../../geometry-and-topology.md#sphere)'s applied [force](../../../classical-mechanics.md#force); reflecting in the horizontal plane reverses that [force](../../../classical-mechanics.md#force) again. The neutral [sphere](../../../geometry-and-topology.md#sphere) remains force-free under both operations. Thus the reflected time-reversed motion obeys the same original forcing.

At $t_c$, reflection fixes both particle centres. Since the [spheres](../../../geometry-and-topology.md#sphere) have no orientational shape variables and there is no contact, uniqueness of the particle-trajectory initial-value problem makes the reflected backward motion coincide with the forward motion:

$$
\boxed{\mathbf r_j(t_c+\tau)=S\mathbf r_j(t_c-\tau),\qquad j=1,2.}
$$

This [reflection symmetry of a two-sphere passing trajectory](../../../stokes-flow.md#reflection-symmetry-of-a-two-sphere-passing-trajectory) fixes the transverse coordinates and reverses the relative axial separation. Consequently, at matching large separations above and below, **both [spheres](../../../geometry-and-topology.md#sphere) return to their original distances from the centreline**. Their intermediate lateral excursions are undone. This uses [kinematic reversibility of Stokes flow](../../../stokes-flow.md#kinematic-reversibility-of-stokes-flow), geometric reflection symmetry and the noncontact result, not a dissipation-minimizing trajectory. It assumes the [spheres](../../../geometry-and-topology.md#sphere) pass one another; a perfectly collinear approach would not supply the side-by-side symmetry event.

<h3 id="1/vii">vii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#1/vii)

When both [spheres](../../../geometry-and-topology.md#sphere) have the same effective downward weight, the second [sphere](../../../geometry-and-topology.md#sphere) adds a force-driven disturbance instead of being merely a force-free rigid inclusion. The power now contains both $WV_{1z}$ and $WV_{2z}$, so the one-forced-sphere bound from part (iv) no longer applies.

For $a\ll R$, place the [spheres](../../../geometry-and-topology.md#sphere) in a tandem configuration with $a\ll s\ll R$. Locally the flow around the second [sphere](../../../geometry-and-topology.md#sphere) is dominated by its downward [Stokeslet](../../../stokes-flow.md#stokeslet). Its axial incident [velocity](../../../classical-mechanics.md#velocity) at the first [sphere](../../../geometry-and-topology.md#sphere) is downward, so the first [sphere](../../../geometry-and-topology.md#sphere) falls faster to leading order. By contrast, the [zero total flux for localized tube Stokes flow](../../../stokes-flow.md#zero-total-flux-for-localized-tube-stokes-flow) requires compensating upward flow away from the downward-moving particle core in sections cutting the [sphere](../../../geometry-and-topology.md#sphere). There are therefore positions in the return flow where the disturbance acts upwards.

One can choose the second [sphere](../../../geometry-and-topology.md#sphere) in such an upward-flow region generated by the first. The [Lorentz reciprocal theorem](../../../stokes-flow.md#lorentz-reciprocal-theorem-for-stokes-flow) makes the axial cross coefficients of the [hydrodynamic mobility matrix](../../../stokes-flow.md#hydrodynamic-mobility-matrix) equal, so the downward [force](../../../classical-mechanics.md#force) on the second [sphere](../../../geometry-and-topology.md#sphere) then produces an upward contribution to the first [sphere](../../../geometry-and-topology.md#sphere)'s [velocity](../../../classical-mechanics.md#velocity). With small well-separated [spheres](../../../geometry-and-topology.md#sphere), this force-driven interaction dominates the higher-order self-resistance change from simply inserting the other [sphere](../../../geometry-and-topology.md#sphere). In mobility notation, with downward positive,

$$
V_{1z}\simeq V_0+W\mathcal M_{12}^{zz},
$$

and the cross coefficient can have either sign in the tube. Thus

$$
\boxed{V_{1z}>V_0\text{ in a downward entraining configuration},\qquad
V_{1z}<V_0\text{ in a return-flow configuration}.}
$$

The distinction is the sign of the incident flow, not whether adding a second geometrical obstacle lowers a fixed-velocity dissipation.

## 2

↑ **Parent:** [Paper 74](paper-74.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

One normalization of the [Papkovich–Neuber representation](../../../stokes-flow.md#papkovich-neuber-representation) uses a harmonic vector $\boldsymbol\Phi$ and harmonic scalar $\psi$:

$$
\boxed{\mathbf u=\boldsymbol\Phi-\frac12\nabla(\mathbf x\cdot\boldsymbol\Phi+\psi),\qquad
p=-\mu\nabla\cdot\boldsymbol\Phi,\qquad
\nabla^2\boldsymbol\Phi=0,\quad\nabla^2\psi=0.}
$$

These formulae give $\nabla\cdot\mathbf u=0$ because $\nabla^2(\mathbf x\cdot\boldsymbol\Phi)=2\nabla\cdot\boldsymbol\Phi$, and give $\mu\nabla^2\mathbf u=\nabla p$. Rescaling the potentials gives the other common normalizations of the representation.

A point [force](../../../classical-mechanics.md#force) requires a decaying, rotationally covariant field linear in $\mathbf F$, with no length scale. Thus choose the harmonic monopole $\boldsymbol\Phi=c\mathbf F/r$, $\psi=0$, for $r>0$. Differentiating gives

$$
\mathbf u=\frac c2\left(\frac{\mathbf F}{r}+\frac{(\mathbf F\cdot\mathbf x)\mathbf x}{r^3}\right),\qquad
p=\mu c\frac{\mathbf F\cdot\mathbf x}{r^3}.
$$

The [Newtonian fluid stress tensor](../../../viscous-fluid-flow.md#newtonian-fluid-stress-tensor) is $\sigma_{ij}=-p\delta_{ij}+\mu(\partial_i u_j+\partial_j u_i)$, which simplifies to $\sigma_{ij}=-3\mu c(\mathbf F\cdot\mathbf x)x_ix_j/r^5$. Its traction resultant on a [sphere](../../../geometry-and-topology.md#sphere), using an outward normal from the origin, is $-4\pi\mu c\mathbf F$. Momentum balance with the [force](../../../classical-mechanics.md#force) $\mathbf F\delta(\mathbf x)$ therefore fixes $c=1/(4\pi\mu)$. The resulting [Stokeslet](../../../stokes-flow.md#stokeslet) is

$$
\boxed{u_i=\frac1{8\pi\mu}\left(\frac{F_i}{r}+\frac{(\mathbf F\cdot\mathbf x)x_i}{r^3}\right),\qquad
p=\frac{\mathbf F\cdot\mathbf x}{4\pi r^3},\qquad
\sigma_{ij}=-\frac3{4\pi}\frac{(\mathbf F\cdot\mathbf x)x_ix_j}{r^5}.}
$$

An arbitrary constant [pressure](../../../thermodynamics.md#pressure) may be added. The stress has purely radial traction on concentric [spheres](../../../geometry-and-topology.md#sphere), and its integrated traction $-\mathbf F$ supplies the required distributional point-force normalization.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Take the upward direction as $\mathbf e_z$, with polar angle $\theta$ measured from it. The liquid is quiescent at infinity. On a translating clean inviscid bubble, the [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) is $(\mathbf u-U\mathbf e_z)\cdot\mathbf n=0$, and the [stress-free boundary condition](../../../viscous-fluid-flow.md#stress-free-boundary-condition) is zero tangential traction. The normal traction must balance uniform gas [pressure](../../../thermodynamics.md#pressure) and any constant-curvature surface-tension jump.

For a vertical [Stokeslet](../../../stokes-flow.md#stokeslet) of strength $F$, the radial [velocity](../../../classical-mechanics.md#velocity) is $u_r=F\cos\theta/(4\pi\mu r)$. Its traction on a concentric [sphere](../../../geometry-and-topology.md#sphere) is purely normal, so zero tangential traction is automatic. The kinematic condition at $r=a$ gives

$$
\boxed{F=4\pi\mu aU.}
$$

The singularity is only a device for generating the exterior solution; there is no liquid point [force](../../../classical-mechanics.md#force) inside the actual bubble. The integrated dynamic traction on the bubble is $-F\mathbf e_z$, giving the [clean-bubble Stokes drag](../../../stokes-flow.md#clean-bubble-stokes-drag). The upward [buoyancy](../../../fluid-mechanics.md#buoyancy) is $4\pi\rho ga^3/3$, hence [force](../../../classical-mechanics.md#force) balance gives

$$
\boxed{U=\frac{\rho ga^2}{3\mu}.}
$$

The normal stress also shows that [surface tension](../../../fluid-mechanics.md#surface-tension) is not required for this particular spherical solution. Let the ambient [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) at the bubble centre be $p_c$, so on its surface $p_h=p_c-\rho ga\cos\theta$. Adding the Stokeslet's dynamic normal traction gives

$$
\sigma_{nn}^{\rm total}=-p_c+
\left(\rho ga-\frac{3F}{4\pi a^2}\right)\cos\theta=-p_c,
$$

where the terminal [buoyancy](../../../fluid-mechanics.md#buoyancy) value of $F$ cancels the dipole. This is the [spherical clean bubble without surface tension](../../../stokes-flow.md#spherical-clean-bubble-without-surface-tension) balance: **an initially spherical bubble can remain spherical in this ideal steady Stokes solution even when [surface tension](../../../fluid-mechanics.md#surface-tension) is zero**. With uniform [surface tension](../../../fluid-mechanics.md#surface-tension) $\gamma$, choose gas [pressure](../../../thermodynamics.md#pressure) $p_b=p_c+2\gamma/a$; with $\gamma=0$, $p_b=p_c$. This proves compatibility of the spherical shape, not stability of arbitrary deformations or validity when inertia matters.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [force](../../../classical-mechanics.md#force) scale is $F\sim\rho ga^3$. At the distant [free surface](../../../fluid-mechanics.md#free-surface), the Stokeslet's [pressure](../../../thermodynamics.md#pressure) and viscous normal-stress scales are $F/d^2$. Gravity restores a displaced surface by a [pressure](../../../thermodynamics.md#pressure) change $\rho gh$, so

$$
\boxed{h\sim\frac F{\rho gd^2}=O\!\left(\frac{a^3}{d^2}\right).}
$$

Thus $h/d=O((a/d)^3)\ll1$, consistent with treating the boundary as approximately flat and impermeable at leading order. This uses the stipulated gravity-dominated restoring balance.

The liquid-air interface has negligible tangential traction. The [stress-free image of a normal Stokeslet](../../../stokes-flow.md#stress-free-image-of-a-normal-stokeslet) places an opposite point [force](../../../classical-mechanics.md#force) at the reflection point, a distance $2d$ above the bubble centre. Across the flat surface the combined normal [velocity](../../../classical-mechanics.md#velocity) is odd and the tangential [velocity](../../../classical-mechanics.md#velocity) is even, so the normal [velocity](../../../classical-mechanics.md#velocity) and tangential stress vanish there. A same-radius inviscid drop of density $2\rho$ has downward excess weight $4\pi\rho ga^3/3$, exactly opposite the bubble's upward [buoyancy](../../../fluid-mechanics.md#buoyancy). Its exterior Stokeslet therefore supplies this image, giving the asserted full-space comparison to leading order in $a/d$.

The image's incident axial [velocity](../../../classical-mechanics.md#velocity) at the bubble is

$$
u_{\rm image}=-\frac{F}{4\pi\mu(2d)}=-\frac{F}{8\pi\mu d}.
$$

To first reflection, the bubble translates with this locally uniform incident [velocity](../../../classical-mechanics.md#velocity) plus its isolated rise speed $F/(4\pi\mu a)$. Hence the [bubble rise near a distant stress-free free surface](../../../stokes-flow.md#bubble-rise-near-a-distant-stress-free-free-surface) is

$$
\boxed{U_b=\frac{F}{4\pi\mu a}-\frac{F}{8\pi\mu d}
=U\left(1-\frac a{2d}+o(a/d)\right).}
$$

Only the first relative correction is retained; the image's spatial variation and additional reflections affect higher terms.

The customary capillary-controlled small-deformation condition is a small [capillary number](../../../fluid-mechanics.md#capillary-number),

$$
\boxed{\mathrm{Ca}=\frac{\mu U}{\gamma}=\frac{\rho ga^2}{3\gamma}\ll1,}
$$

equivalently a small [Bond number](../../../fluid-mechanics.md#bond-number) $\mathrm{Bo}=\rho ga^2/\gamma$. This is a sufficient condition, not a necessary condition for the special isolated spherical solution in part (b). More precisely, the image's strain is $O(F/(\mu d^2))$, so its deformation-producing normal stress compared with $\gamma/a$ is $O(\mathrm{Bo}(a/d)^2)$. When exploiting the exact isolated solution, that smaller combination controls the leading boundary-induced distortion. If capillarity at the distant free surface is also retained, the gravity-dominated deflection scaling requires $\gamma/(\rho gd^2)\ll1$; $a\ll\sqrt{\gamma/(\rho g)}\ll d$ allows both the usual spherical-bubble criterion and gravity-dominated surface restoration.

## 3

↑ **Parent:** [Paper 74](paper-74.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let the undisturbed water surface be $z=0$, the oil's upper surface $z=\eta(x,t)$ and its lower surface $z=b(x,t)$, so $h=\eta-b$. Leading [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) in the nearly inviscid water is $p_w=-\rho_wgz$ relative to atmospheric [pressure](../../../thermodynamics.md#pressure); in the oil it is $p_H=\rho g(\eta-z)$. Equality at the interface gives $\rho gh=-\rho_wgb$, hence

$$
b=-\frac\rho{\rho_w}h,\qquad
\eta=\frac{\rho_w-\rho}{\rho_w}h.
$$

Thus the horizontal hydrostatic driving gradient is

$$
\boxed{p_{H,x}=\rho g\eta_x=\rho g'h_x,\qquad
 g'=\frac{\rho_w-\rho}{\rho_w}g.}
$$

This [reduced gravity](../../../reduced-gravity.md) accounts for most of the oil thickness being below the undisturbed water level.

Because the oil is much more viscous than the water and air, tangential tractions on both faces are negligible. In a thin layer, the leading horizontal [velocity](../../../classical-mechanics.md#velocity) is consequently independent of depth: the [floating extensional viscous gravity current](../../../reduced-gravity.md#floating-extensional-viscous-gravity-current) is a plug, rather than the parabolic profile of a no-slip gravity current. Integrating [incompressibility](../../../fluid-mechanics.md#incompressible-flow) $u_x+w_z=0$ between the moving material boundaries, and using their [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition), gives conservation of oil volume,

$$
\boxed{h_t+(hu)_x=0,\qquad h_t+uh_x+hu_x=0.}
$$

To derive the factor $4$ in the extensional balance, [incompressibility](../../../fluid-mechanics.md#incompressible-flow) gives $w_z=-u_x$. The [Newtonian fluid stress tensor](../../../viscous-fluid-flow.md#newtonian-fluid-stress-tensor) has $\sigma_{zz}=-p-2\mu u_x$. Normal-stress balance relative to the hydrostatic part therefore requires $p=p_H-2\mu u_x$. The horizontal stress then satisfies

$$
\sigma_{xx}=-p+2\mu u_x=-p_H+4\mu u_x.
$$

Thus the longitudinal tensile [force](../../../classical-mechanics.md#force) in an oil slice, relative to its [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure), is $4\mu hu_x$ per unit width. Balancing its difference across the slice with the horizontal driving [force](../../../classical-mechanics.md#force) $-hp_{H,x}\,dx$ yields

$$
\boxed{4\mu(hu_x)_x=hp_{H,x},\qquad
\frac{4\mu}{h}(hu_x)_x=p_{H,x}.}
$$

The coefficient is the planar extensional [Trouton ratio](../../../rheology.md#trouton-ratio), arising from both the direct horizontal strain and the [pressure](../../../thermodynamics.md#pressure) correction required by the transverse normal-stress condition.

Using the [pressure gradient](../../../fluid-mechanics.md#pressure-gradient) above, integration in $x$ gives

$$
4\mu hu_x=\frac12\rho g'h^2+C(t).
$$

The stated nose stress condition sets $C(t)=0$, not an arbitrary imposed inlet tension. Consequently

$$
u_x=kh,\qquad k=\frac{\rho g'}{8\mu}.
$$

For a material slice injected at time $t_0$, let $\tau=t-t_0$ be its age. The thickness equation along its [Lagrangian trajectory](../../../continuum-mechanics.md#lagrangian-trajectory) is $dh/dt=-hu_x=-kh^2$, with $h=h_0$ at injection. Define

$$
T=\frac1{kh_0}=\frac{8\mu}{\rho g'h_0}.
$$

Then $h=h_0/(1+\tau/T)$. The slice injected during $dt_0$ has volume $h_0u_0dt_0$ per unit width, so at fixed observation time $t$,

$$
-h\frac{\partial x}{\partial t_0}=h_0u_0,
\qquad
\frac{\partial x}{\partial\tau}=u_0\left(1+\frac\tau T\right).
$$

Since a newly injected slice has $x(t,t)=0$, integration and subsequent differentiation along a material slice give the [constant-flux floating extensional gravity current](../../../reduced-gravity.md#constant-flux-floating-extensional-gravity-current):

$$
\boxed{h(t;t_0)=\frac{h_0}{1+(t-t_0)/T},\qquad
u(t;t_0)=u_0\left(1+\frac{t-t_0}{T}\right),\qquad
x(t;t_0)=u_0\left[(t-t_0)+\frac{(t-t_0)^2}{2T}\right].}
$$

The oldest slice forms the nose. Measuring time from the start of injection, $t_0=0$ there, so

$$
\boxed{x_N(t)=u_0t+\frac{\rho g'h_0u_0}{16\mu}t^2,\qquad
h_N(t)=\frac{h_0}{1+t/T}.}
$$

Its speed $\dot x_N=u_0(1+t/T)$ is exactly the material [velocity](../../../classical-mechanics.md#velocity) at the nose, as required.

For a fixed position $x$ behind the nose, the age needed to reach it is determined by $x/u_0=\tau+\tau^2/(2T)$, independently of the observation time. Hence both thickness and [velocity](../../../classical-mechanics.md#velocity) become stationary there once the nose has passed. Eliminating $\tau$ gives

$$
\boxed{h(x)=h_0\left(1+\frac{\rho g'h_0x}{4\mu u_0}\right)^{-1/2},\qquad
u(x)=u_0\left(1+\frac{\rho g'h_0x}{4\mu u_0}\right)^{1/2}.}
$$

Their product is $h_0u_0$, so the steady profile carries precisely the inlet [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate); integrating it to $x_N(t)$ gives the total injected volume $h_0u_0t$.

The length

$$
\boxed{\ell=\frac{\mu u_0}{\rho g'h_0}}
$$

is the horizontal distance over which reduced-gravity driving causes an order-one change in inlet speed and thickness by viscous extension. The associated age is $T=8\ell/u_0$; the exact profile contains $x/(4\ell)$. It is an extensional adjustment length, not a shear-diffusion scale. The result applies while the stated thin-layer and negligible-inertia approximations remain valid.

## 4

↑ **Parent:** [Paper 74](paper-74.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Take positive $x$ in the snail's direction of travel, and let $y$ measure height above the rigid plane. The wave moves at laboratory [velocity](../../../classical-mechanics.md#velocity) $U-V$. In the wave frame the plane's horizontal [velocity](../../../classical-mechanics.md#velocity) is $V-U$ and the foot's is $V$. The foot is stationary as a shape, so its material [velocity](../../../classical-mechanics.md#velocity) is tangent to $y=h(x)$: to leading [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory) order its components are $(V,Vh_x)$. Apply the [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) to both surfaces.

The leading [Stokes flow](../../../stokes-flow.md) equations are $p_y=0$ and $\mu u_{yy}=p_x$. Their solution is the local [Couette-Poiseuille flow](../../../viscous-fluid-flow.md#couette-poiseuille-flow)

$$
\boxed{u(x,y)=V-U+\frac{Uy}{h(x)}+\frac{p_x}{2\mu}y(y-h).}
$$

The normal-velocity condition on each steady surface and [incompressibility](../../../fluid-mechanics.md#incompressible-flow) make the wave-frame flux independent of $x$. Integrating the [velocity](../../../classical-mechanics.md#velocity) gives

$$
q=h\left(V-\frac U2\right)-\frac{h^3p_x}{12\mu}.
$$

Put $C=V-U/2$. Periodicity of [pressure](../../../thermodynamics.md#pressure) gives $0=\int_0^Lp_xdx=12\mu(CI_2-qI_3)$, and hence

$$
\boxed{q=C\frac{I_2}{I_3},\qquad
p_x=12\mu\left(\frac C{h^2}-\frac q{h^3}\right),\qquad
I_j=\int_0^Lh^{-j}dx.}
$$

The shear traction exerted by the fluid on the plane, positive in the $x$ direction, is

$$
\boxed{\tau_0=\mu u_y(x,0)=\frac{\mu U}{h}-\frac h2p_x
=\frac{\mu(4U-6V)}h+\frac{6\mu q}{h^2}.}
$$

The snail is force-free horizontally: its gait consists of internal motion and it has no externally applied horizontal drive. Uniform locomotion therefore requires zero net horizontal fluid [force](../../../classical-mechanics.md#force) on the foot per wavelength. The stresses on opposite periodic fluid faces cancel, so horizontal momentum balance also makes the net [force](../../../classical-mechanics.md#force) on the plane zero. Thus

$$
0=\int_0^L\tau_0dx=\mu(4U-6V)I_1+6\mu qI_2.
$$

Substitution of $q$ proves the [lubrication model of a crawling snail](../../../viscous-fluid-flow.md#lubrication-model-of-a-crawling-snail):

$$
\boxed{U=\frac{6(1-\alpha)}{4-3\alpha}V,\qquad
\alpha=\frac{I_2^2}{I_1I_3}.}
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) applied to $h^{-1/2}$ and $h^{-3/2}$ gives $0<\alpha\leq1$, with equality exactly for a uniform gap. Thus the denominator is positive, and a nonuniform waveform gives forward motion; the flat gap gives $U=0$.

For the sinusoidal shape, the given integrals yield

$$
I_1=\frac{L}{h_0\sqrt{1-A^2}},\qquad
I_2=\frac{L}{h_0^2(1-A^2)^{3/2}},\qquad
I_3=\frac{L(1+A^2/2)}{h_0^3(1-A^2)^{5/2}}.
$$

Therefore $\alpha=1/(1+A^2/2)$ and

$$
\boxed{U=\frac{3A^2}{1+2A^2}V.}
$$

For small amplitude, $U\sim3A^2V$: the leading locomotion is quadratic, and there is no propulsion from a flat foot. As $A\to1^-$, $U\to V$, so the wave becomes nearly stationary in the laboratory frame while the snail advances relative to it. However, the minimum gap tends to zero; finite speed in this limit does not imply finite dissipation, and $A=1$ itself is excluded by the noncontact model.

For the general waveform, use the mechanical work identity for [viscous dissipation](../../../stokes-flow.md#viscous-dissipation). [Pressure](../../../thermodynamics.md#pressure) does no boundary work because the boundary motion is tangential in the wave frame. The plane's [velocity](../../../classical-mechanics.md#velocity) is constant, and its total [force](../../../classical-mechanics.md#force) is zero, so it contributes zero net work. The upper boundary supplies, at leading lubrication order,

$$
\Phi=\mu V\int_0^Lu_y(x,h)dx
=V\left(\mu UI_1+\frac12\int_0^Lhp_xdx\right).
$$

The zero plane-force relation is $\mu UI_1=\tfrac12\int hp_xdx$. Consequently

$$
\boxed{\Phi=2\mu UVI_1.}
$$

As a direct check, integrating the squared shear rate gives $\Phi=\int_0^L[\mu U^2/h+h^3p_x^2/(12\mu)]dx=\mu I_1[U^2+12C^2(1-\alpha)]$, which reduces to the same result using the force-free speed relation. Zero horizontal [force](../../../classical-mechanics.md#force) on the foot does not mean zero gait work: the tangential material [velocity](../../../classical-mechanics.md#velocity) along its sloping surface includes vertical motion.

For prescribed speed $U>0$ and sinusoidal shape, eliminate $V=U(1+2A^2)/(3A^2)$ to obtain

$$
\Phi(A)=\frac{2\mu LU^2}{3h_0}\frac{1+2A^2}{A^2\sqrt{1-A^2}}.
$$

Writing $y=A^2$, the logarithmic derivative of the amplitude-dependent factor is

$$
\frac2{1+2y}-\frac1y+\frac1{2(1-y)}=0
\quad\Longleftrightarrow\quad2y^2+3y-2=0.
$$

The only root in $0<y<1$ is $y=1/2$. The dissipation diverges at both endpoints, so this is the global minimum and gives the [optimal sinusoidal waveform for viscous snail locomotion](../../../viscous-fluid-flow.md#optimal-sinusoidal-waveform-for-viscous-snail-locomotion):

$$
\boxed{A_{\rm opt}=\frac1{\sqrt2},\qquad V_{\rm opt}=\frac43U,\qquad
\Phi_{\min}=\frac{8\sqrt2}{3}\frac{\mu LU^2}{h_0}.}
$$

The magically driven flat glider has simple [Couette flow](../../../viscous-fluid-flow.md#couette-flow) $u=Uy/h_0$ in the laboratory frame, and dissipation $\Phi_{\rm glide}=\mu LU^2/h_0$ per wavelength. Hence

$$
\boxed{\Phi_{\min}/\Phi_{\rm glide}=8\sqrt2/3.}
$$

The comparison is at the same $U$, mean thickness $h_0$ and wavelength $L$; the flat glider is externally propelled, whereas the snail must power its internal waveform.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
