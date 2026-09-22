# Paper 2

↑ **Parent:** [2022](../2022.md)

[Original paper, released PDF pages 248–252](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e/response/2127325/attach/3/FOI%202022%20639%20Sullivan%20materials.pdf?cookie_passthrough=1#page=248)

**Table of contents**

- [Section A](#section-a)
  - [A1](#section-a/a1)
    - [Solution](#section-a/a1/solution)
  - [A2](#section-a/a2)
    - [Solution](#section-a/a2/solution)
  - [A3](#section-a/a3)
    - [Solution](#section-a/a3/solution)
  - [A4](#section-a/a4)
    - [Solution](#section-a/a4/solution)
  - [A5](#section-a/a5)
    - [Solution](#section-a/a5/solution)
- [Section B](#section-b)
  - [B6](#section-b/b6)
    - [Solution](#section-b/b6/solution)
  - [B7](#section-b/b7)
    - [a](#section-b/b7/a)
      - [Solution](#section-b/b7/a/solution)
    - [b](#section-b/b7/b)
      - [Solution](#section-b/b7/b/solution)
    - [c](#section-b/b7/c)
      - [Solution](#section-b/b7/c/solution)
    - [d](#section-b/b7/d)
      - [Solution](#section-b/b7/d/solution)
- [Section C](#section-c)
  - [C8](#section-c/c8)
    - [a](#section-c/c8/a)
      - [Solution](#section-c/c8/a/solution)
    - [b](#section-c/c8/b)
      - [Solution](#section-c/c8/b/solution)
    - [c](#section-c/c8/c)
      - [Solution](#section-c/c8/c/solution)
    - [d](#section-c/c8/d)
      - [Solution](#section-c/c8/d/solution)
    - [e](#section-c/c8/e)
      - [Solution](#section-c/c8/e/solution)
    - [f](#section-c/c8/f)
      - [Solution](#section-c/c8/f/solution)
  - [C9](#section-c/c9)
    - [a](#section-c/c9/a)
      - [Solution](#section-c/c9/a/solution)
    - [b](#section-c/c9/b)
      - [Solution](#section-c/c9/b/solution)
    - [c](#section-c/c9/c)
      - [Solution](#section-c/c9/c/solution)
    - [d](#section-c/c9/d)
      - [Solution](#section-c/c9/d/solution)
    - [e](#section-c/c9/e)
      - [Solution](#section-c/c9/e/solution)

## Section A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-a/a1">A1</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a1/solution">Solution</h4>

↑ **Parent:** [A1](#section-a/a1)

Interpret the applied [pressure](../../pressure.md) as a uniform increase of external [hydrostatic pressure](../../fluid-mechanics.md#hydrostatic-pressure) on all six faces, and approximate the rock by an [isotropic](../../continuum-mechanics.md#isotropy) material obeying [linear elasticity](../../elasticity-physics.md#linear-elasticity). Taking tensile [stress](../../continuum-mechanics.md#stress) as positive, $\sigma_x=\sigma_y=\sigma_z=-p$. By [Hooke's law](../../elasticity-physics.md#hooke-s-law), the [strain](../../continuum-mechanics.md#strain) along any one axis is

$$
\epsilon_x=\frac{\sigma_x-\nu(\sigma_y+\sigma_z)}{E}=-\frac{(1-2\nu)p}{E}.
$$

To first order in the small [strain](../../continuum-mechanics.md#strain), the fractional [volume](../../geometry-and-topology.md#volume) change is the sum of the three axial [strains](../../continuum-mechanics.md#strain):

$$
\frac{\Delta V}{V}=\epsilon_x+\epsilon_y+\epsilon_z=-\frac{3(1-2\nu)p}{E}=-\frac pK,
\qquad K=\frac{E}{3(1-2\nu)}.
$$

Thus the [bulk modulus](../../elasticity-physics.md#bulk-modulus) is $K=40\,\mathrm{GPa}$. Using the specified [Young's modulus](../../elasticity-physics.md#young-s-modulus), [Poisson's ratio](../../elasticity-physics.md#poisson-s-ratio), $V=1\,\mathrm{m^3}$ and $p=101325\,\mathrm{Pa}$ gives

$$
\boxed{\Delta V=-2.53\times10^{-6}\,\mathrm{m^3}=-2.53\,\mathrm{cm^3}.}
$$

The sign indicates contraction. This is the change relative to the unloaded reference state; simply maintaining a specimen already equilibrated at this same [pressure](../../pressure.md) would produce no further change.

<h3 id="section-a/a2">A2</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a2/solution">Solution</h4>

↑ **Parent:** [A2](#section-a/a2)

Use the pipe-diameter convention for the [Reynolds number](../../dynamic-viscosity.md#reynolds-number), with mean [velocity](../../classical-mechanics.md#velocity) $\bar v$, [density](../../fluid-mechanics.md#density) $\rho$ and [dynamic viscosity](../../dynamic-viscosity.md) $\mu$:

$$
\mathrm{Re}=\frac{\rho\bar vD}{\mu},\qquad
D_{\rm crit}=\frac{\mathrm{Re}_{\rm crit}\mu}{\rho\bar v}.
$$

The [Reynolds number](../../dynamic-viscosity.md#reynolds-number) compares inertial and viscous effects in the [fluid flow](../../fluid-mechanics.md#fluid-flow). A conventional estimate for the onset of [turbulence](../../turbulence.md) in a pipe is $\mathrm{Re}_{\rm crit}\simeq2000$, giving

$$
D_{\rm crit}=\frac{2000(3.16\times10^{-4}\,\mathrm{Pa\,s})}{(789\,\mathrm{kg\,m^{-3}})(0.5\,\mathrm{m\,s^{-1}})}=1.60\times10^{-3}\,\mathrm m.
$$

Hence the usual onset estimate is $\boxed{D\gtrsim1.6\,\mathrm{mm}}$. Using the also common transition criterion $\mathrm{Re}_{\rm crit}=2300$ gives $1.84\,\mathrm{mm}$, whereas $\mathrm{Re}\gtrsim4000$, used for established [turbulence](../../turbulence.md), gives $D\gtrsim3.2\,\mathrm{mm}$. There is no universal sharp minimum: inlet disturbances and pipe conditions affect the transition from [laminar flow](../../fluid-mechanics.md#laminar-flow), so the threshold convention must accompany the answer.

<h3 id="section-a/a3">A3</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a3/solution">Solution</h4>

↑ **Parent:** [A3](#section-a/a3)

**(a)** Treat the lake as a [heat bath](../../thermal-equilibrium.md#heat-bath) at fixed [temperature](../../temperature.md) $T_0=288.15\,\mathrm K$ and the block's [heat capacity](../../heat.md#heat-capacity) as constant. Its initial [temperature](../../temperature.md) is $T_i=473.15\,\mathrm K$, and $C=mc=355\,\mathrm{J\,K^{-1}}$. Although the cooling is irreversible, [entropy](../../entropy.md) is a [state function](../../thermodynamics.md#state-function), so evaluate the block's change along an imagined [reversible thermodynamic process](../../second-law-of-thermodynamics.md#reversible-thermodynamic-process):

$$
\Delta S_{\rm block}=\int_{T_i}^{T_0}\frac{C\,dT}{T}=C\ln\frac{T_0}{T_i}=-176.1\,\mathrm{J\,K^{-1}}.
$$

The lake receives [heat](../../heat.md) $Q=C(T_i-T_0)=65675\,\mathrm J$, and therefore

$$
\Delta S_{\rm lake}=\frac{Q}{T_0}=227.9\,\mathrm{J\,K^{-1}}.
$$

Adding the two contributions gives

$$
\boxed{\Delta S_{\rm Universe}=C\left[\ln\frac{T_0}{T_i}+\frac{T_i-T_0}{T_0}\right]=51.9\,\mathrm{J\,K^{-1}}.}
$$

The positive result is consistent with the [Second law of thermodynamics](../../second-law-of-thermodynamics.md) for [heat transfer](../../heat.md#heat-transfer) across a finite [temperature](../../temperature.md) difference. The calculation uses $c=710\,\mathrm{J\,kg^{-1}\,K^{-1}}$ exactly as printed in both the original PDF and the transcription; it does not replace the supplied value by a tabulated value for lead.

**(b)** The block starts and eventually finishes at the lake's [temperature](../../temperature.md), so its net [entropy](../../entropy.md) change is approximately zero. Neglecting buoyancy, air resistance and the final immersion depth, the lost [gravitational potential energy](../../energy.md#gravitational-energy) $mgh$ becomes [internal energy](../../internal-energy.md) in the lake after the motion and waves have dissipated. The lake remains at $T_0$, giving

$$
\boxed{\Delta S_{\rm Universe}\simeq\frac{mgh}{T_0}=\frac{(0.5\,\mathrm{kg})(9.81\,\mathrm{m\,s^{-2}})(200\,\mathrm m)}{288.15\,\mathrm K}=3.40\,\mathrm{J\,K^{-1}}.}
$$

Temporary heating of the block or temporary storage in [kinetic energy](../../energy.md#kinetic-energy) does not change this final [energy](../../energy.md) and [entropy](../../entropy.md) balance once [thermal equilibrium](../../thermal-equilibrium.md) is restored.

<h3 id="section-a/a4">A4</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a4/solution">Solution</h4>

↑ **Parent:** [A4](#section-a/a4)

For a fixed amount of a [simple compressible system](../../thermodynamics.md#simple-compressible-system), write the [internal energy](../../internal-energy.md) as $U(S,V)$. Its exact [differential](../../smooth-manifold.md#differential-of-a-smooth-map) is

$$
dU=T\,dS-p\,dV,\qquad T=\left(\frac{\partial U}{\partial S}\right)_V,\qquad -p=\left(\frac{\partial U}{\partial V}\right)_S.
$$

Assuming the [thermodynamic potential](../../thermodynamic-potential.md) has continuous second [partial derivatives](../../multivariable-calculus.md#partial-derivative), equality of its [mixed partial derivatives](../../multivariable-calculus.md#mixed-partial-derivative) yields the first [Maxwell relation](../../thermodynamics.md#maxwell-relations):

$$
\boxed{\left(\frac{\partial T}{\partial V}\right)_S=\frac{\partial^2U}{\partial V\partial S}=-\left(\frac{\partial p}{\partial S}\right)_V.}
$$

For the second [Maxwell relation](../../thermodynamics.md#maxwell-relations), use the [Legendre transform](../../convex-optimization.md#convex-conjugate) $H=U+pV$, the [enthalpy](../../enthalpy.md). Its natural variables are $S,p$ since

$$
dH=dU+p\,dV+V\,dp=T\,dS+V\,dp.
$$

Thus $T=(\partial H/\partial S)_p$ and $V=(\partial H/\partial p)_S$. Equality of the [mixed partial derivatives](../../multivariable-calculus.md#mixed-partial-derivative) now gives

$$
\boxed{\left(\frac{\partial T}{\partial p}\right)_S=\frac{\partial^2H}{\partial p\partial S}=\left(\frac{\partial V}{\partial S}\right)_p.}
$$

<h3 id="section-a/a5">A5</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a5/solution">Solution</h4>

↑ **Parent:** [A5](#section-a/a5)

Let $N_u,N_l$ be the upper- and lower-level populations and $g_u,g_l$ their [degeneracy factors](../../statistical-physics.md#degeneracy-factor). At [thermal equilibrium](../../thermal-equilibrium.md), the [Boltzmann distribution](../../thermodynamics.md#boltzmann-distribution) gives

$$
\frac{N_u}{N_l}=\frac{g_u}{g_l}\exp\left(-\frac{\Delta E}{k_BT}\right),\qquad
\frac{\Delta E}{k_B}=\frac{27\times10^{-6}\,\mathrm{eV}}{8.617333262\times10^{-5}\,\mathrm{eV\,K^{-1}}}=0.313322\,\mathrm K.
$$

No [degeneracy factors](../../statistical-physics.md#degeneracy-factor) are supplied, so the numerical answers use equal [degeneracy factors](../../statistical-physics.md#degeneracy-factor). Stating the ratio as upper population divided by lower population removes an otherwise arbitrary inversion.

**(a)** At $T=500\,\mathrm K$,

$$
\boxed{\frac{N_u}{N_l}=e^{-0.000626644}=0.999374.}
$$

The two populations are nearly equal because the level separation is much smaller than the thermal [energy](../../energy.md) $k_BT$.

**(b)** At $T=2\,\mathrm{mK}=0.002\,\mathrm K$,

$$
\boxed{\frac{N_u}{N_l}=e^{-156.661}=9.18\times10^{-69}.}
$$

Almost every atom occupies the lower level. If the levels have unequal [degeneracy factors](../../statistical-physics.md#degeneracy-factor), each boxed ratio must be multiplied by $g_u/g_l$; their individual values cannot be inferred from the paper.

## Section B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-b/b6">B6</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b6/solution">Solution</h4>

↑ **Parent:** [B6](#section-b/b6)

[Newton's second law](../../force.md#newton-s-second-law) takes its familiar form $m\mathbf a=\mathbf F$ in an [inertial frame](../../mathematical-physics.md#inertial-frame). Axes fixed to a turning apparatus or to the [Earth](../../planetary-science.md#earth) form a [rotating reference frame](../../mathematical-physics.md#rotating-reference-frame). Extra [inertial forces](../../mathematical-physics.md#fictitious-force) account for the [acceleration](../../classical-mechanics.md#acceleration) of these coordinates. Their values depend on the chosen [reference frame](../../mathematical-physics.md#reference-frame); physical interactions such as [gravity](../../physics.md#gravity), [tension](../../force.md#tension) and contact [forces](../../force.md) must still be included separately.

Let the rotating origin have inertial [acceleration](../../classical-mechanics.md#acceleration) $\mathbf A$, and let its axes have [angular velocity](../../rigid-body-dynamics.md#angular-velocity) $\boldsymbol\Omega(t)$. For any [vector](../../vector-space.md#vector) $\mathbf q$, the [rotating-frame derivative formula](../../mathematical-physics.md#rotating-frame-derivative-formula) is

$$
\left(\frac{d\mathbf q}{dt}\right)_{\rm I}=\left(\frac{d\mathbf q}{dt}\right)_{\rm R}+\boldsymbol\Omega\times\mathbf q.
$$

Each rotating [basis vector](../../vector-space.md#basis-vector) changes by $\boldsymbol\Omega\times\mathbf e_i$, which proves this rule by expanding $\mathbf q$ in that basis. Apply it twice to the position relative to the moving origin. With $\mathbf v'$ and $\mathbf a'$ measured in the rotating axes,

$$
\mathbf a_{\rm I}=\mathbf A+\mathbf a'+2\boldsymbol\Omega\times\mathbf v'+\dot{\boldsymbol\Omega}\times\mathbf r+\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf r).
$$

Consequently the equation in the [rotating reference frame](../../mathematical-physics.md#rotating-reference-frame) is

$$
m\mathbf a'=\mathbf F-m\mathbf A-2m\boldsymbol\Omega\times\mathbf v'-m\dot{\boldsymbol\Omega}\times\mathbf r-m\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf r).
$$

The additional terms are the translational [inertial force](../../mathematical-physics.md#fictitious-force), [Coriolis force](../../mathematical-physics.md#coriolis-force), [Euler force](../../mathematical-physics.md#euler-force) and [centrifugal force](../../mathematical-physics.md#centrifugal-force), respectively. The last two simplify when the [angular velocity](../../rigid-body-dynamics.md#angular-velocity) is constant: the [Euler force](../../mathematical-physics.md#euler-force) vanishes, while the other rotation terms remain.

The [centrifugal force](../../mathematical-physics.md#centrifugal-force) points away from the rotation axis. If $\mathbf r_\perp$ is the perpendicular displacement from that axis, then

$$
\boxed{\mathbf F_{\rm cf}=m\Omega^2\mathbf r_\perp.}
$$

For uniform rotation it has [potential energy](../../energy.md#potential-energy)

$$
\Phi_{\rm cf}=-\frac12m|\boldsymbol\Omega\times\mathbf r|^2,\qquad \mathbf F_{\rm cf}=-\nabla\Phi_{\rm cf}.
$$

A mass at rest relative to a turntable can therefore be described as having an inward [tension](../../force.md#tension) or [friction](../../newtonian-mechanics.md#friction) balancing its outward [centrifugal force](../../mathematical-physics.md#centrifugal-force). In an [inertial frame](../../mathematical-physics.md#inertial-frame), the inward physical [force](../../force.md) instead produces the required [centripetal acceleration](../../classical-mechanics.md#centripetal-acceleration). These are two descriptions of the same motion; one must not insert the rotating-frame outward term into the inertial equation as an additional physical interaction.

A rotating liquid gives a useful quantitative example. For a liquid in [hydrostatic equilibrium](../../statistical-physics.md#hydrostatic-equilibrium) relative to a vessel rotating uniformly about the vertical axis,

$$
\frac{\partial p}{\partial s}=\rho\Omega^2s,\qquad \frac{\partial p}{\partial z}=-\rho g.
$$

Along the [free surface](../../fluid-mechanics.md#free-surface) the [pressure](../../pressure.md) is constant, so $\Omega^2s\,ds-g\,dz=0$ and

$$
z(s)=z(0)+\frac{\Omega^2s^2}{2g}.
$$

The surface is a [elliptic paraboloid](../../euclidean-geometry.md#elliptic-paraboloid). This is the balance of [gravity](../../physics.md#gravity) and the [centrifugal force](../../mathematical-physics.md#centrifugal-force) in the rotating description. On the [Earth](../../planetary-science.md#earth), the same outward [acceleration](../../classical-mechanics.md#acceleration) reduces effective [gravity](../../physics.md#gravity), most strongly at the equator, and contributes to the planet's equatorial bulge.

The [Coriolis force](../../mathematical-physics.md#coriolis-force) depends on relative motion:

$$
\boxed{\mathbf F_{\rm cor}=-2m\boldsymbol\Omega\times\mathbf v'.}
$$

It is perpendicular to both $\boldsymbol\Omega$ and $\mathbf v'$, vanishes for motion along the rotation axis, and reverses when the relative [velocity](../../classical-mechanics.md#velocity) reverses. The [dot product](../../inner-product.md#dot-product) gives

$$
\mathbf F_{\rm cor}\cdot\mathbf v'=0.
$$

Thus the [Coriolis force](../../mathematical-physics.md#coriolis-force) does no [work](../../energy.md#work) in the [rotating reference frame](../../mathematical-physics.md#rotating-reference-frame): it changes the direction of motion rather than directly changing the rotating-frame [kinetic energy](../../energy.md#kinetic-energy). For example, on a horizontal turntable rotating anticlockwise as viewed from above, an outward-moving slider has a clockwise [Coriolis acceleration](../../mathematical-physics.md#coriolis-acceleration), whereas an inward-moving slider has an anticlockwise one. The deflection can be observed by comparing a laboratory camera with a camera rotating with the table.

For slow horizontal motion on the [Earth](../../planetary-science.md#earth) at latitude $\lambda$, keep the vertical component $\Omega_E\sin\lambda$ of its [angular velocity](../../rigid-body-dynamics.md#angular-velocity). In east-north coordinates $(u,v)$ the horizontal [Coriolis acceleration](../../mathematical-physics.md#coriolis-acceleration) is

$$
(a_E,a_N)=(fv,-fu),\qquad f=2\Omega_E\sin\lambda.
$$

It deflects motion to the right in the northern hemisphere and to the left in the southern hemisphere. In large-scale atmospheric and oceanic motion it can balance a horizontal [pressure gradient](../../fluid-mechanics.md#pressure-gradient), giving [geostrophic balance](../../mathematical-physics.md#geostrophic-balance). With $\hat{\mathbf z}$ upward, the steady horizontal equation without [friction](../../newtonian-mechanics.md#friction) is

$$
f\hat{\mathbf z}\times\mathbf v=-\frac1\rho\nabla_h p.
$$

The resulting [velocity](../../classical-mechanics.md#velocity) runs along lines of equal [pressure](../../pressure.md). This approximation requires rotation to dominate local inertial changes; it is inappropriate close to the equator where $f$ tends to zero.

The [Foucault pendulum](../../simple-pendulum.md#foucault-pendulum) gives another terrestrial example. In the [small-angle approximation](../../geometry-and-topology.md#small-angle-approximation), its horizontal coordinates satisfy

$$
\ddot x+\omega_0^2x=f\dot y,\qquad \ddot y+\omega_0^2y=-f\dot x,\qquad \omega_0^2=\frac g\ell.
$$

To first order in the small ratio $\Omega_E/\omega_0$, the oscillation plane precesses relative to the ground at angular rate $-\Omega_E\sin\lambda$: clockwise in the northern hemisphere, zero at the equator, and one revolution per sidereal day at a pole. The [Coriolis force](../../mathematical-physics.md#coriolis-force) explains this changing orientation without requiring [energy](../../energy.md) input. Together these examples show why [inertial forces](../../mathematical-physics.md#fictitious-force) are useful whenever the apparatus or environment supplies naturally rotating coordinates.

<h3 id="section-b/b7">B7</h3>

↑ **Parent:** [Section B](#section-b)

The examination asks for three notes. All four options are worked below so that each topic has a complete study answer.

<h4 id="section-b/b7/a">a</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/a/solution">Solution</h5>

↑ **Parent:** [A](#section-b/b7/a)

The [method of images](../../mathematics.md#method-of-images) solves certain [electrostatics](../../electrostatics.md) problems by replacing a conductor by fictitious [electric charges](../../electric-charge.md) outside the region where the solution is required. The replacement must satisfy the actual boundary values of the [electric potential](../../electric-field.md#electric-potential) as well as the prescribed sources. The [uniqueness of Poisson equation](../../analysis.md#uniqueness-of-poisson-equation) then establishes that the constructed [electric potential](../../electric-field.md#electric-potential) equals the physical one in that region. The image locations are mathematical devices; they are not real charges inside the metal.

For a [point charge](../../electric-field.md#point-charge) $q$ at $(0,0,a)$ above an infinite grounded conducting plane $z=0$, put an image charge $-q$ at $(0,0,-a)$. In a [cylindrical coordinate system](../../multivariable-calculus.md#cylindrical-coordinate-system) with coordinates $(s,z)$ the potential in the physical region is

$$
\phi(s,z)=\frac{q}{4\pi\epsilon_0}\left[\frac1{\sqrt{s^2+(z-a)^2}}-\frac1{\sqrt{s^2+(z+a)^2}}\right],\qquad z>0.
$$

This vanishes at $z=0$, has the required singularity at the real charge, and tends to zero at infinity. With [electric field](../../electric-field.md) $\mathbf E=-\nabla\phi$, the induced [surface charge density](../../electrostatics.md#surface-charge-density) follows from the normal field immediately above the conductor:

$$
\sigma(s)=\epsilon_0E_z(s,0^+)=-\frac{qa}{2\pi(s^2+a^2)^{3/2}},\qquad
\int_0^\infty\sigma(s)\,2\pi s\,ds=-q.
$$

The [force](../../force.md) on $q$ is the field of the image evaluated at the real charge:

$$
\boxed{\mathbf F=-\frac{q^2}{16\pi\epsilon_0a^2}\hat{\mathbf z}.}
$$

The [electrostatic energy](../../electrostatics.md#electrostatic-energy) relative to infinite separation is $U=\tfrac12q\phi_{\rm image}=-q^2/(16\pi\epsilon_0a)$. The factor $1/2$ accounts for the fact that the induced charge changes as the real charge is assembled; treating the image as an independently fixed physical charge would give the wrong [energy](../../energy.md).

A second standard geometry is a grounded conducting sphere of radius $b$ with a charge $q$ a distance $d>b$ from its centre. Its exterior field is generated by an image $q'=-qb/d$ at distance $b^2/d$ from the centre on the line towards the real charge. On the sphere the distances to the real and image charges are in the ratio $d/b$, making their potentials cancel. For an isolated neutral sphere, an additional central image $+qb/d$ makes the total induced charge zero and leaves the surface an [equipotential](../../electric-field.md#equipotential). The construction is powerful for suitable symmetric boundaries, but arbitrary boundaries do not in general admit a finite image system.

<h4 id="section-b/b7/b">b</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/b/solution">Solution</h5>

↑ **Parent:** [B](#section-b/b7/b)

An [electrical insulator](../../permittivity.md#electrical-insulator) has no freely conducting bulk charge in the ideal static description, but an applied [electric field](../../electric-field.md) can displace bound positive and negative charge relative to one another. The resulting [electric dipole moments](../../electrostatics.md#electric-dipole-moment) per unit [volume](../../geometry-and-topology.md#volume) define the [polarization density](../../electromagnetism.md#polarization-density) $\mathbf P$. Distortion of electronic charge clouds, relative displacement of [ions](../../chemistry.md#ion), and partial alignment of permanent molecular [electric dipoles](../../electrostatics.md#electric-dipole) can all contribute. Thermal agitation opposes the last mechanism.

For a weak field in a linear [isotropic](../../continuum-mechanics.md#isotropy) [dielectric](../../permittivity.md#dielectric), the constitutive law is

$$
\mathbf P=\epsilon_0\chi_e\mathbf E,\qquad
\mathbf D=\epsilon_0\mathbf E+\mathbf P=\epsilon\mathbf E,\qquad
\epsilon=\epsilon_0(1+\chi_e)=\epsilon_0\epsilon_r.
$$

Here $\chi_e$ is the [electric susceptibility](../../permittivity.md#electric-susceptibility), $\epsilon$ is the [permittivity](../../permittivity.md), and $\mathbf D$ is the [electric displacement field](../../electromagnetism.md#electric-displacement-field). In an [anisotropic](../../continuum-mechanics.md#anisotropy) material, $\chi_e$ is a [tensor](../../multilinear-algebra.md#tensor) and $\mathbf P$ need not be parallel to $\mathbf E$. These response laws describe the macroscopic field, not necessarily the microscopic field acting on one [molecule](../../molecule.md).

Spatial variation and surface termination of the [polarization density](../../electromagnetism.md#polarization-density) give [bound charge and bound current](../../electromagnetism.md#bound-charge-and-bound-current) through the bound charge densities

$$
\rho_b=-\nabla\cdot\mathbf P,\qquad \sigma_b=\mathbf P\cdot\hat{\mathbf n},
$$

where $\hat{\mathbf n}$ is outward from the material. Thus uniform [polarization density](../../electromagnetism.md#polarization-density) has no bulk bound charge, but generally has opposite bound charges on opposing surfaces. [Gauss's law](../../maxwell-equations.md#gauss-s-law) can be rewritten as

$$
\nabla\cdot\mathbf D=\rho_{\rm free}.
$$

With no [free surface](../../fluid-mechanics.md#free-surface) charge, the normal component of $\mathbf D$ is continuous across an interface; the tangential [electric field](../../electric-field.md) is continuous in [electrostatics](../../electrostatics.md).

For example, fill a [parallel-plate capacitor](../../electromagnetism.md#parallel-plate-capacitor) of plate area $A$ and gap $d$ with a uniform [dielectric](../../permittivity.md#dielectric), neglecting fringing. At fixed free plate charge $Q$, $D=Q/A$, so

$$
E=\frac{Q}{\epsilon A},\qquad V=Ed,\qquad
\boxed{C=\frac{\epsilon A}{d}=\epsilon_rC_0.}
$$

The induced bound surface charges oppose the original field, reducing the [electric field](../../electric-field.md) and potential difference at fixed $Q$. At fixed applied potential difference, the field remains $V/d$ and the battery instead supplies more free charge. The [electric displacement field](../../electromagnetism.md#electric-displacement-field) separates these free-charge and bound-charge roles.

<h4 id="section-b/b7/c">c</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/c/solution">Solution</h5>

↑ **Parent:** [C](#section-b/b7/c)

Because the [magnetic field](../../magnetic-field.md) obeys $\nabla\cdot\mathbf B=0$, it can be represented locally as the [curl](../../multivariable-calculus.md#curl) of a [magnetic vector potential](../../electromagnetism.md#magnetic-vector-potential):

$$
\boxed{\mathbf B=\nabla\times\mathbf A.}
$$

This automatically enforces the absence of magnetic monopoles. It is also a global representation throughout ordinary all-space problems without monopole singularities. It is not unique: the [gauge transformation](../../electromagnetism.md#gauge-transformation)

$$
\mathbf A\longmapsto\mathbf A+\nabla\chi
$$

leaves $\mathbf B$ unchanged because the [curl](../../multivariable-calculus.md#curl) of a [gradient](../../multivariable-calculus.md#gradient) vanishes. In a time-dependent problem,

$$
\mathbf E=-\nabla\phi-\frac{\partial\mathbf A}{\partial t},\qquad
\phi\longmapsto\phi-\frac{\partial\chi}{\partial t}
$$

makes the same transformation leave both physical fields unchanged and automatically satisfies [Faraday's law](../../maxwell-equations.md#faraday-s-law-of-induction).

In vacuum [magnetostatics](../../electromagnetism.md#magnetostatics), choose the [Coulomb gauge](../../electromagnetism.md#coulomb-gauge) $\nabla\cdot\mathbf A=0$. Substitution into [Ampère's law](../../maxwell-equations.md#ampere-s-circuital-law) and the identity $\nabla\times(\nabla\times\mathbf A)=\nabla(\nabla\cdot\mathbf A)-\nabla^2\mathbf A$ gives

$$
\nabla^2\mathbf A=-\mu_0\mathbf J,\qquad
\mathbf A(\mathbf r)=\frac{\mu_0}{4\pi}\int\frac{\mathbf J(\mathbf r')}{|\mathbf r-\mathbf r'|}\,d^3r'
$$

for a localized steady [electric current density](../../electric-charge.md#current-density) and a potential vanishing at infinity. Taking the [curl](../../multivariable-calculus.md#curl) recovers the [Biot-Savart law](../../electromagnetism.md#biot-savart-law). The [magnetic vector potential](../../electromagnetism.md#magnetic-vector-potential) converts a constrained [vector](../../vector-space.md#vector) field problem into componentwise [Poisson equations](../../partial-differential-equation.md#poisson-s-equation) once a gauge is chosen.

For a uniform [magnetic field](../../magnetic-field.md), $\mathbf A=\tfrac12\mathbf B\times\mathbf r$ is a convenient choice. For a localized [magnetic dipole moment](../../electromagnetism.md#magnetic-dipole-moment) $\mathbf m$, the leading far-field potential is

$$
\mathbf A(\mathbf r)=\frac{\mu_0}{4\pi}\frac{\mathbf m\times\mathbf r}{r^3}.
$$

Another useful relation is [Stokes theorem](../../multivariable-calculus.md#stokes-theorem), which relates a closed-path [integral](../../integral.md) to the [magnetic flux](../../magnetic-field.md#magnetic-flux) through a spanning surface:

$$
\oint_{\partial S}\mathbf A\cdot d\boldsymbol\ell=\int_S\mathbf B\cdot d\mathbf S.
$$

The units of $\mathbf A$ are $\mathrm{T\,m}$, equivalently $\mathrm{Wb\,m^{-1}}$.

<h4 id="section-b/b7/d">d</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/d/solution">Solution</h5>

↑ **Parent:** [D](#section-b/b7/d)

An incident [electromagnetic wave](../../electromagnetic-wave.md) generally produces reflected and transmitted waves because the two media have different electromagnetic response. Consider a flat interface between homogeneous, linear, lossless media with [permittivities](../../permittivity.md) $\epsilon_j$ and [magnetic permeabilities](../../maxwell-equations.md#permeability-electromagnetism) $\mu_j$. Their wave speeds and [wave impedances](../../electromagnetic-wave.md#wave-impedance) are

$$
v_j=\frac1{\sqrt{\mu_j\epsilon_j}},\qquad Z_j=\sqrt{\frac{\mu_j}{\epsilon_j}}.
$$

For each [plane electromagnetic wave](../../electromagnetic-wave.md#plane-electromagnetic-wave), $\mathbf H=\hat{\mathbf k}\times\mathbf E/Z_j$. With no [free surface](../../fluid-mechanics.md#free-surface) charge or current, the [interface conditions for electromagnetic fields](../../electromagnetic-wave.md#interface-conditions-for-electromagnetic-fields) require continuous tangential $\mathbf E,\mathbf H$ and normal $\mathbf D,\mathbf B$. Equality of the [phase](../../wave.md#phase-waves) at every point on the boundary gives equal [angular frequencies](../../lagrangian-mechanics.md#angular-frequency) and tangential [wavevectors](../../elasticity-physics.md#wavevector). Hence the reflection [angle](../../geometry-and-topology.md#angle) equals the incidence [angle](../../geometry-and-topology.md#angle) and [Snell's law](../../partial-differential-equation.md#snell-s-law) is

$$
n_1\sin\theta_i=n_2\sin\theta_t,
$$

where $n_j=c/v_j$ and each [angle](../../geometry-and-topology.md#angle) is measured from the normal.

At normal incidence use the same tangential axis for all electric [amplitudes](../../wave.md#wave-amplitude). The two independent boundary equations are

$$
E_i+E_r=E_t,\qquad \frac{E_i-E_r}{Z_1}=\frac{E_t}{Z_2}.
$$

Solving gives the [amplitude](../../wave.md#wave-amplitude) [Fresnel equations](../../electromagnetic-wave.md#fresnel-equations)

$$
\boxed{r=\frac{E_r}{E_i}=\frac{Z_2-Z_1}{Z_2+Z_1},\qquad t=\frac{E_t}{E_i}=\frac{2Z_2}{Z_1+Z_2}.}
$$

For nonmagnetic media, these become $r=(n_1-n_2)/(n_1+n_2)$ and $t=2n_1/(n_1+n_2)$. Reflection into a medium of larger [refractive index](../../electromagnetic-wave.md#refractive-index) therefore reverses the electric [amplitude](../../wave.md#wave-amplitude)'s sign at normal incidence.

The normal [Poynting vector](../../electromagnetic-wave.md#poynting-vector) determines the reflected and transmitted fractions of incident [power](../../energy.md#power). At normal incidence,

$$
\mathcal R=|r|^2,\qquad \mathcal T=\frac{Z_1}{Z_2}|t|^2,\qquad
\boxed{\mathcal R+\mathcal T=1.}
$$

It is the [power](../../energy.md#power) fractions, rather than the squared electric [amplitudes](../../wave.md#wave-amplitude) alone, that add to unity.

At oblique incidence separate [transverse electric polarization](../../electromagnetic-wave.md#transverse-electric-polarization) ($s$, [electric field](../../electric-field.md) perpendicular to the incidence plane) from [transverse magnetic polarization](../../electromagnetic-wave.md#transverse-magnetic-polarization) ($p$, [electric field](../../electric-field.md) in that plane). For nonmagnetic media, writing $c_i=\cos\theta_i$ and $c_t=\cos\theta_t$, the [Fresnel equations](../../electromagnetic-wave.md#fresnel-equations) are

$$
r_s=\frac{n_1c_i-n_2c_t}{n_1c_i+n_2c_t},\qquad
t_s=\frac{2n_1c_i}{n_1c_i+n_2c_t},
$$



$$
r_p=\frac{n_2c_i-n_1c_t}{n_2c_i+n_1c_t},\qquad
t_p=\frac{2n_1c_i}{n_2c_i+n_1c_t}.
$$

Here choose a common $s$ direction and, for each ray, the $p$ direction as $\hat{\mathbf s}\times\hat{\mathbf k}$. This makes the reflected $p$ basis reverse its tangential direction at normal incidence, explaining why the displayed $r_p$ then has the opposite sign to $r_s$. Physical [reflectance](../../radiometry.md#reflectance) is independent of this sign convention. For either polarization with propagating transmission,

$$
\mathcal R=|r|^2,\qquad \mathcal T=\frac{n_2\cos\theta_t}{n_1\cos\theta_i}|t|^2.
$$

For $p$ polarization, zero reflection occurs at the [Brewster angle](../../electromagnetic-wave.md#brewster-s-angle) $\tan\theta_B=n_2/n_1$. If $n_1>n_2$, incidence above the [critical angle for total internal reflection](../../electromagnetic-wave.md#critical-angle-for-total-internal-reflection) $\sin\theta_c=n_2/n_1$ produces an [evanescent field in total internal reflection](../../electromagnetic-wave.md#evanescent-field-in-total-internal-reflection) and $\mathcal R=1$ for an isolated lossless interface. A lossy second medium requires complex response coefficients and an absorption term in the [energy](../../energy.md) balance.

## Section C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-c/c8">C8</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c8/a">a</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/a/solution">Solution</h5>

↑ **Parent:** [A](#section-c/c8/a)

Use an [ideal gas](../../ideal-gas.md) to illustrate the [Carnot cycle](../../second-law-of-thermodynamics.md#carnot-cycle), with hot and cold [heat baths](../../thermal-equilibrium.md#heat-bath) at $T_h=T_2$ and $T_c=T_1$. The four processes are all [reversible thermodynamic processes](../../second-law-of-thermodynamics.md#reversible-thermodynamic-process). Lettered states below belong only to this illustration; the engine later in the question uses numbered states.

<a id="section-c/c8/a/image-an-ideal-gas-carnot-cycle-two-isotherms-joined-by-two-reversible-adiabats"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2-c8-carnot-pv.png)

**[Figure 1](#section-c/c8/a/image-an-ideal-gas-carnot-cycle-two-isotherms-joined-by-two-reversible-adiabats). An ideal-gas Carnot cycle: two isotherms joined by two reversible adiabats**.

Starting at $A$, perform the following four stages:

- $A\to B$: [isothermal expansion](../../second-law-of-thermodynamics.md#isothermal-expansion) at $T_h$. The gas absorbs [heat](../../heat.md) $Q_h$ from the hot [heat bath](../../thermal-equilibrium.md#heat-bath) and does [work](../../energy.md#work). Its [internal energy](../../internal-energy.md) is unchanged, so $Q_h=W_{AB}=nRT_h\ln(V_B/V_A)$.
- $B\to C$: [reversible ideal-gas adiabat](../../first-law-of-thermodynamics.md#reversible-ideal-gas-adiabat) during expansion. Insulation prevents [heat transfer](../../heat.md#heat-transfer); [work](../../energy.md#work) done by the gas reduces its [internal energy](../../internal-energy.md) and lowers its [temperature](../../temperature.md) from $T_h$ to $T_c$.
- $C\to D$: [isothermal compression](../../second-law-of-thermodynamics.md#isothermal-compression) at $T_c$. [Work](../../energy.md#work) done on the gas is rejected as [heat](../../heat.md) $Q_c$ to the cold [heat bath](../../thermal-equilibrium.md#heat-bath), with $Q_c=nRT_c\ln(V_C/V_D)>0$.
- $D\to A$: insulated [adiabatic compression](../../first-law-of-thermodynamics.md#adiabatic-compression), performed reversibly, raises the [temperature](../../temperature.md) back to $T_h$ and closes the cycle.

The clockwise enclosed area in the [pressure](../../pressure.md)-[volume](../../geometry-and-topology.md#volume) diagram is the positive net [work](../../energy.md#work) per cycle, $W=\oint p\,dV=Q_h-Q_c$.

<h4 id="section-c/c8/b">b</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/b/solution">Solution</h5>

↑ **Parent:** [B](#section-c/c8/b)

Because the working substance returns to its original [thermodynamic state](../../thermodynamics.md#thermodynamic-state), its net [entropy](../../entropy.md) change is zero. There is no [entropy](../../entropy.md) change on either [reversible ideal-gas adiabat](../../first-law-of-thermodynamics.md#reversible-ideal-gas-adiabat); on each [isothermal process](../../second-law-of-thermodynamics.md#isothermal-process) the [entropy](../../entropy.md) transfer is the exchanged [heat](../../heat.md) divided by the bath's absolute [temperature](../../temperature.md). Hence

$$
\frac{Q_h}{T_h}-\frac{Q_c}{T_c}=0,\qquad \frac{Q_c}{Q_h}=\frac{T_c}{T_h}.
$$

The [first law of thermodynamics](../../first-law-of-thermodynamics.md) over a complete cycle gives $W=Q_h-Q_c$. The [thermal efficiency](../../thermodynamics.md#thermal-efficiency) is therefore

$$
\boxed{\eta_{\rm Carnot}=\frac{W}{Q_h}=1-\frac{Q_c}{Q_h}=1-\frac{T_c}{T_h}=1-\frac{T_1}{T_2}.}
$$

The use of kelvins is essential. This result does not depend on the working substance. For the [ideal gas](../../ideal-gas.md) illustration, the two [reversible ideal-gas adiabats](../../first-law-of-thermodynamics.md#reversible-ideal-gas-adiabat) imply $V_C/V_B=V_D/V_A=(T_h/T_c)^{1/(\gamma-1)}$, so $\ln(V_B/V_A)=\ln(V_C/V_D)$; the explicit [heat](../../heat.md) expressions in (a) give the same ratio.

<h4 id="section-c/c8/c">c</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/c/solution">Solution</h5>

↑ **Parent:** [C](#section-c/c8/c)

The complete cycle must be a [reversible thermodynamic process](../../second-law-of-thermodynamics.md#reversible-thermodynamic-process): no [friction](../../newtonian-mechanics.md#friction), viscous dissipation, unrestrained expansion, or other source of [entropy](../../entropy.md). Each moving boundary must be arbitrarily close to [mechanical equilibrium](../../thermodynamics.md#mechanical-equilibrium). [Heat transfer](../../heat.md#heat-transfer) to or from a bath must occur across an infinitesimal [temperature](../../temperature.md) difference, and the insulated stages must be genuinely [adiabatic processes](../../first-law-of-thermodynamics.md#adiabatic-process). There must also be no direct [heat](../../heat.md) leak between the [heat baths](../../thermal-equilibrium.md#heat-bath).

For an engine exchanging [heat](../../heat.md) only with these two [heat baths](../../thermal-equilibrium.md#heat-bath), the [Second law of thermodynamics](../../second-law-of-thermodynamics.md) gives

$$
S_{\rm gen}=\frac{Q_c}{T_c}-\frac{Q_h}{T_h}\geq0,
$$

and thus

$$
\eta=1-\frac{T_c}{T_h}-\frac{T_cS_{\rm gen}}{Q_h}\leq\eta_{\rm Carnot}.
$$

Practical engines generate [entropy](../../entropy.md) through finite [temperature](../../temperature.md) differences, [friction](../../newtonian-mechanics.md#friction) and other dissipative effects. They therefore fall below the [Carnot cycle](../../second-law-of-thermodynamics.md#carnot-cycle) limit. Approaching reversible [heat](../../heat.md) exchange generally requires vanishingly slow operation for a finite heat-transfer apparatus, limiting useful [power](../../energy.md#power).

<h4 id="section-c/c8/d">d</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/d/solution">Solution</h5>

↑ **Parent:** [D](#section-c/c8/d)

For the numbered engine, denote the low and high [pressures](../../pressure.md) by $p_1=p_4=p_l$ and $p_2=p_3=p_h$. Let $R_g$ denote the [molar gas constant](../../ideal-gas.md#molar-gas-constant). The [ideal gas law](../../ideal-gas.md#ideal-gas-law) makes the constant-pressure branches straight rays in a [temperature](../../temperature.md)-[volume](../../geometry-and-topology.md#volume) diagram:

$$
T=\frac{p_h}{nR_g}V\quad(2\to3),\qquad
T=\frac{p_l}{nR_g}V\quad(4\to1).
$$

The high-pressure ray is steeper. For a constant [heat capacity ratio](../../ideal-gas.md#heat-capacity-ratio) $\gamma$, each [reversible ideal-gas adiabat](../../first-law-of-thermodynamics.md#reversible-ideal-gas-adiabat) obeys

$$
TV^{\gamma-1}=\text{constant}.
$$

Consequently $1\to2$ curves upward and left during compression; $2\to3$ goes upward and right along the steeper ray; $3\to4$ curves downward and right during expansion; and $4\to1$ goes downward and left along the shallower ray.

<a id="section-c/c8/d/image-temperature-volume-solution-sketch-for-the-two-pressure-gas-engine-cycle"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2-c8-brayton-tv.png)

**[Figure 2](#section-c/c8/d/image-temperature-volume-solution-sketch-for-the-two-pressure-gas-engine-cycle). Temperature-volume solution sketch for the two-pressure gas-engine cycle**.

The plot is an original calculation for $\gamma=7/5$, $p_h/p_l=10$ and $V_3/V_2=2$; its state directions follow the original paper. The dashed extensions identify the two constant-pressure rays, not additional stages of the cycle.

<h4 id="section-c/c8/e">e</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/e/solution">Solution</h5>

↑ **Parent:** [E](#section-c/c8/e)

This is the [Brayton cycle](../../thermodynamics.md#brayton-cycle). Assume fixed gas amount, constant [heat capacities](../../heat.md#heat-capacity), and internally reversible [adiabatic processes](../../first-law-of-thermodynamics.md#adiabatic-process), as intended by the ideal engine model. Put $r_p=p_h/p_l=p_2/p_1>1$ and

$$
a=\frac{\gamma-1}{\gamma},\qquad k=r_p^a.
$$

Combining $pV^\gamma=\text{constant}$ with the [ideal gas law](../../ideal-gas.md#ideal-gas-law) gives $T\propto p^{(\gamma-1)/\gamma}$ along either [reversible ideal-gas adiabat](../../first-law-of-thermodynamics.md#reversible-ideal-gas-adiabat). Therefore

$$
\frac{T_2}{T_1}=k,\qquad \frac{T_3}{T_4}=k,
\qquad T_3-T_2=k(T_4-T_1).
$$

During a constant-pressure process the [heat](../../heat.md) supplied equals the [enthalpy](../../enthalpy.md) increase. If $C_p$ is the molar [heat capacity at constant pressure](../../enthalpy.md#heat-capacity-at-constant-pressure), the positive [heat](../../heat.md) input and output are

$$
Q_{\rm in}=nC_p(T_3-T_2),\qquad
Q_{\rm out}=nC_p(T_4-T_1).
$$

The insulated branches exchange no [heat](../../heat.md), so the [first law of thermodynamics](../../first-law-of-thermodynamics.md) gives $W=Q_{\rm in}-Q_{\rm out}$. Hence

$$
\boxed{\eta=1-\frac{Q_{\rm out}}{Q_{\rm in}}=1-\frac1k=1-\left(\frac{p_2}{p_1}\right)^{(1-\gamma)/\gamma}.}
$$

An [adiabatic process](../../first-law-of-thermodynamics.md#adiabatic-process) alone need not be an [isentropic process](../../first-law-of-thermodynamics.md#isentropic-process); the relations used here also require internal reversibility. Dissipative compression or expansion would require extra information and would not, in general, obey this efficiency formula.

<h4 id="section-c/c8/f">f</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/f/solution">Solution</h5>

↑ **Parent:** [F](#section-c/c8/f)

For a diatomic [ideal gas](../../ideal-gas.md) in the usual regime with three translational and two rotational quadratic [degrees of freedom](../../classical-mechanics.md#degree-of-freedom), but frozen vibrational excitation, the [equipartition theorem](../../canonical-ensemble.md#equipartition-theorem) gives

$$
C_V=\frac52R_g,\qquad C_p=\frac72R_g,\qquad \gamma=\frac75.
$$

The [Brayton cycle](../../thermodynamics.md#brayton-cycle) efficiency is therefore

$$
\boxed{\eta=1-10^{-2/7}=0.4821\simeq48.2\%.}
$$

The constant-pressure expansion has $T_3/T_2=V_3/V_2=2$, while the compression has $T_2/T_1=10^{2/7}=1.93070$. The same relations give $T_4/T_1=2$. Thus, in units of the minimum [temperature](../../temperature.md),

$$
(T_1,T_2,T_3,T_4)=T_1(1,1.93070,3.86140,2).
$$

The maximum and minimum [temperatures](../../temperature.md) are $T_3$ and $T_1$. A [Carnot cycle](../../second-law-of-thermodynamics.md#carnot-cycle) between those extremes has

$$
\boxed{\eta_{\rm Carnot}=1-\frac{T_1}{T_3}=1-\frac1{2\,10^{2/7}}=0.7410\simeq74.1\%.}
$$

The difference is about $25.9$ percentage points. In the [Brayton cycle](../../thermodynamics.md#brayton-cycle), [heat](../../heat.md) is supplied and rejected over ranges of [temperature](../../temperature.md); the whole input is not supplied at $T_3$, nor is the whole rejection made at $T_1$. This explains the lower efficiency even for mechanically ideal stages. Absolute state [temperatures](../../temperature.md) are not supplied, so $\gamma=7/5$ is an explicit standard diatomic-gas approximation rather than a conclusion about all possible rotational and vibrational excitation regimes.

<h3 id="section-c/c9">C9</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c9/a">a</h4>

↑ **Parent:** [C9](#section-c/c9)

<h5 id="section-c/c9/a/solution">Solution</h5>

↑ **Parent:** [A](#section-c/c9/a)

A cubic reflecting cavity supports [standing waves](../../mathematical-physics.md#standing-wave) with positive integer mode indices and [wavevector](../../elasticity-physics.md#wavevector) components $k_i=\pi n_i/L$. A cell in mode space has [volume](../../geometry-and-topology.md#volume) $(\pi/L)^3$. In the continuum approximation, a spherical shell of radius $k$ and thickness $dk$ has one-eighth of its [volume](../../geometry-and-topology.md#volume) in the positive octant. There are two independent transverse [photon polarizations](../../quantum-mechanics.md#photon-polarization) for a generic [wavevector](../../elasticity-physics.md#wavevector). Hence

$$
dN=2\times\frac18\times4\pi k^2dk\left(\frac L\pi\right)^3=\frac{L^3k^2}{\pi^2}\,dk.
$$

The [photon](../../quantum-mechanics.md#photon) [energy](../../energy.md) is $\epsilon=\hbar\omega=\hbar ck$, so $dk=d\epsilon/(\hbar c)$. Therefore

$$
\boxed{dN=\frac{L^3\epsilon^2}{\pi^2\hbar^3c^3}\,d\epsilon.}
$$

This is the leading bulk [density of states](../../quantum-ideal-gas-statistics.md#density-of-states), valid when the cavity is large compared with the relevant [wavelengths](../../wave-equation.md#wavelength) and many modes lie in the counting interval. A finite cavity has a discrete mode spectrum, with boundary corrections beyond this approximation. Modes with vanishing indices require separate boundary counting but do not change the leading $L^3$ term. Here $\hbar$ is the [reduced Planck constant](../../quantum-mechanics.md#reduced-planck-constant), as printed in the original PDF; replacing it by $h$ would introduce an erroneous factor of $(2\pi)^3$.

<h4 id="section-c/c9/b">b</h4>

↑ **Parent:** [C9](#section-c/c9)

<h5 id="section-c/c9/b/solution">Solution</h5>

↑ **Parent:** [B](#section-c/c9/b)

Each independent cavity mode is a [quantum harmonic oscillator](../../quantum-harmonic-oscillator.md) of [angular frequency](../../lagrangian-mechanics.md#angular-frequency) $\omega$. Its occupation numbers $n=0,1,\ldots$ represent the numbers of [photons](../../quantum-mechanics.md#photon) in that mode. At [thermal equilibrium](../../thermal-equilibrium.md), [photons](../../quantum-mechanics.md#photon) can be absorbed and emitted by the walls, so their number is not conserved and the [photon chemical potential](../../chemical-potential.md#photon-chemical-potential) is zero. The [Boltzmann distribution](../../thermodynamics.md#boltzmann-distribution) of the oscillator excitations then gives

$$
\langle n\rangle=\frac1{e^{\hbar\omega/(k_BT)}-1},\qquad
\bar U=\hbar\omega\langle n\rangle.
$$

The expression supplied in the paper is the thermal excitation [energy](../../energy.md). The oscillator's temperature-independent [zero-point energy](../../quantum-harmonic-oscillator.md#zero-point-energy) is excluded from the emitted [thermal radiation](../../electromagnetic-radiation.md#thermal-radiation).

Putting $\epsilon=\hbar\omega$ and $d\epsilon=\hbar\,d\omega$ into the mode count from (a) gives the number of modes per unit cavity [volume](../../geometry-and-topology.md#volume):

$$
\frac{dN}{L^3}=\frac{\omega^2}{\pi^2c^3}\,d\omega.
$$

Multiplying by the mean thermal [energy](../../energy.md) in each mode yields [Planck's law](../../statistical-physics.md#planck-s-law) in the angular-frequency convention:

$$
\boxed{u(T,\omega)\,d\omega=\frac{\omega^2\,d\omega}{\pi^2c^3}\frac{\hbar\omega}{e^{\hbar\omega/(k_BT)}-1}.}
$$

The two [photon polarizations](../../quantum-mechanics.md#photon-polarization) are already included in the [density of states](../../quantum-ideal-gas-statistics.md#density-of-states); no further factor of two is needed. $u(T,\omega)d\omega$ has units $\mathrm{J\,m^{-3}}$, whereas $u(T,\omega)$ has units $\mathrm{J\,s\,m^{-3}}$.

<h4 id="section-c/c9/c">c</h4>

↑ **Parent:** [C9](#section-c/c9)

<h5 id="section-c/c9/c/solution">Solution</h5>

↑ **Parent:** [C](#section-c/c9/c)

The equilibrium [photon gas](../../statistical-physics.md#photon-gas) is [isotropic](../../continuum-mechanics.md#isotropy), so the [energy density](../../statistical-physics.md#energy-density) per unit [solid angle](../../euclidean-geometry.md#solid-angle) in a narrow angular-frequency interval is $u(T,\omega)d\omega/(4\pi)$. For rays making [angle](../../geometry-and-topology.md#angle) $\theta$ with an outward surface normal, a surface element $dA$ is crossed in time $dt$ by rays initially in a [volume](../../geometry-and-topology.md#volume) $c\,dt\,dA\cos\theta$. Only the outward hemisphere contributes. Thus

$$
e(T,\omega)=\frac{cu(T,\omega)}{4\pi}\int_0^{2\pi}d\phi\int_0^{\pi/2}\cos\theta\sin\theta\,d\theta
=\boxed{\frac{cu(T,\omega)}4}.
$$

The hemispherical restriction supplies a factor $1/2$ and the directional projection supplies another $1/2$. A small aperture in a cavity therefore emits this spectral [power](../../energy.md#power) per unit area. A [blackbody](../../astrophysics.md#blackbody) at the same [temperature](../../temperature.md) emits the same amount: otherwise radiation exchange between it and the aperture would violate [thermal equilibrium](../../thermal-equilibrium.md).

Integrating [Planck's law](../../statistical-physics.md#planck-s-law) over all positive [angular frequencies](../../lagrangian-mechanics.md#angular-frequency) gives the total emitted [heat flux density](../../heat.md#heat-flux-density)

$$
M(T)=\int_0^\infty e(T,\omega)\,d\omega
=\frac{\hbar}{4\pi^2c^2}\int_0^\infty\frac{\omega^3\,d\omega}{e^{\hbar\omega/(k_BT)}-1}.
$$

Set $x=\hbar\omega/(k_BT)$. Then

$$
M(T)=\frac{k_B^4T^4}{4\pi^2\hbar^3c^2}\int_0^\infty\frac{x^3\,dx}{e^x-1}.
$$

The remaining [integral](../../integral.md) is independent of [temperature](../../temperature.md), proving $M\propto T^4$. Its value follows by expanding $(e^x-1)^{-1}=\sum_{m=1}^\infty e^{-mx}$ and integrating termwise:

$$
\int_0^\infty\frac{x^3\,dx}{e^x-1}=\sum_{m=1}^\infty\frac6{m^4}=\frac{\pi^4}{15}.
$$

Consequently the [Stefan–Boltzmann law](../../heat.md#stefan-boltzmann-law) is

$$
\boxed{M(T)=\sigma T^4,\qquad \sigma=\frac{\pi^2k_B^4}{60\hbar^3c^2}=5.67037\times10^{-8}\,\mathrm{W\,m^{-2}\,K^{-4}}.}
$$

This is emitted [power](../../energy.md#power) alone. A body in a radiation environment also absorbs incoming radiation, which must be included when calculating net [radiative cooling](../../heat.md#radiative-cooling).

<h4 id="section-c/c9/d">d</h4>

↑ **Parent:** [C9](#section-c/c9)

<h5 id="section-c/c9/d/solution">Solution</h5>

↑ **Parent:** [D](#section-c/c9/d)

Let the spacecraft radius be $a$, and assume that [heat](../../heat.md) redistribution keeps its whole surface at a common [temperature](../../temperature.md) $T$. Neglect background radiation, and let $R\gg r,a$. The Sun's [luminosity](../../astrophysics.md#luminosity), from the [Stefan–Boltzmann law](../../heat.md#stefan-boltzmann-law), is

$$
L_S=4\pi r^2\sigma T_S^4.
$$

At distance $R$, the incident [irradiance](../../radiometry.md#irradiance) is $F_S=L_S/(4\pi R^2)=\sigma T_S^4(r/R)^2$. The spacecraft intercepts radiation over its projected disc, area $\pi a^2$, but emits from its whole spherical area $4\pi a^2$. The [radiative equilibrium](../../heat.md#radiative-equilibrium) condition is therefore

$$
\pi a^2\sigma T_S^4\frac{r^2}{R^2}=4\pi a^2\sigma T^4.
$$

Cancelling the common factors gives

$$
\boxed{T=T_S\sqrt{\frac r{2R}}\ \propto\ T_S\sqrt{\frac rR}.}
$$

The radius of the spacecraft cancels. The factor $1/\sqrt2$ follows from the ratio of absorbing projected area to emitting surface area. Uniform surface [temperature](../../temperature.md) is the intended additional idealization behind a single equilibrium surface [temperature](../../temperature.md). A poorly conducting spacecraft would have position-dependent [temperatures](../../temperature.md); for example, a locally reradiating patch facing the Sun would instead have $T_{\rm subsolar}=T_S\sqrt{r/R}$, and a different maximum-temperature constraint.

<h4 id="section-c/c9/e">e</h4>

↑ **Parent:** [C9](#section-c/c9)

<h5 id="section-c/c9/e/solution">Solution</h5>

↑ **Parent:** [E](#section-c/c9/e)

[Kirchhoff's law of thermal radiation](../../astrophysics.md#kirchhoff-s-law-of-thermal-radiation) equates spectral absorptivity and [spectral emissivity](../../heat.md#spectral-emissivity) at the same [wavelength](../../wave-equation.md#wavelength) and direction. A surface that is a poor absorber in the thermal [infrared](../../optics.md#infrared) is also a poor emitter there; a coating cannot be assigned its solar absorption independently of its thermal emission spectrum.

**(i) All-wavelength black paint.** It absorbs the sunlight and also radiates maximally at the spacecraft's own [temperature](../../temperature.md). With the isothermal-sphere assumptions of (d), the limiting black-surface distance is

$$
\boxed{\frac{R_{\min,\rm black}}r=\frac12\left(\frac{T_S}{T_{\max}}\right)^2=\frac12\left(\frac{6000}{600}\right)^2=50.}
$$

The spacecraft can operate at $R\geq50r$ in this model. A surface already assumed to be a [blackbody](../../astrophysics.md#blackbody) is not improved by another black coating; relative to option (ii), however, this paint permits closer operation.

**(ii) Black at short [wavelengths](../../wave-equation.md#wavelength) and grey in the [infrared](../../optics.md#infrared).** By [Wien's displacement law](../../astrophysics.md#wien-s-displacement-law), changing the [black-body radiation](../../statistical-physics.md#black-body-radiation) [temperature](../../temperature.md) from $6000\,\mathrm K$ to $600\,\mathrm K$ shifts the [wavelength](../../wave-equation.md#wavelength) peak from about $0.5\,\mu\mathrm m$ to about $5\,\mu\mathrm m$. Most solar [power](../../energy.md#power) is therefore in the highly absorbing short-wavelength band, whereas most spacecraft emission lies beyond $2\,\mu\mathrm m$, where the [spectral emissivity](../../heat.md#spectral-emissivity) is reduced. The coating retains most of the heating but suppresses much of the cooling. Under the intended two-band [grey body](../../heat.md#grey-body) approximation, **option (ii) makes the spacecraft hotter at the same distance and requires a larger minimum distance than black paint.**

To express the comparison without inventing a grey absorptivity, let $\bar\alpha_S$ be [radiometric absorptance](../../radiometry.md#radiometric-absorptance) averaged over the solar spectrum and $\bar\epsilon_T$ be emissivity averaged over the spacecraft's own thermal spectrum. The [radiative equilibrium](../../heat.md#radiative-equilibrium) equation becomes

$$
\bar\alpha_S\sigma T_S^4\frac{r^2}{R^2}=4\bar\epsilon_T\sigma T^4,
\qquad
T=T_S\sqrt{\frac r{2R}}\left(\frac{\bar\alpha_S}{\bar\epsilon_T}\right)^{1/4}.
$$

At the failure threshold,

$$
\boxed{\frac{R_{\min}}r=50\sqrt{\frac{\bar\alpha_S}{\bar\epsilon_{600}}}.}
$$

For an ideal two-band coating take a constant [radiometric absorptance](../../radiometry.md#radiometric-absorptance) $g<1$ beyond $\lambda_c=2\,\mu\mathrm m$, and unity below it. If $f(T)$ is the fraction of the [power](../../energy.md#power) emitted by a [blackbody](../../astrophysics.md#blackbody) below $\lambda_c$, [Planck's law](../../statistical-physics.md#planck-s-law) gives

$$
f(T)=\frac{15}{\pi^4}\int_{hc/(\lambda_ck_BT)}^\infty\frac{x^3}{e^x-1}\,dx,
\qquad
\bar\alpha_S=g+(1-g)f(T_S),\quad
\bar\epsilon_{600}=g+(1-g)f(600\,\mathrm K).
$$

Since $f(T_S)>f(600\,\mathrm K)$, this model has $\bar\alpha_S>\bar\epsilon_{600}$ and hence $R_{\min}>50r$. The paper supplies neither a numerical value of $g$ nor a detailed spectrum, so no unique numerical distance for the grey paint follows. If its long-wavelength absorption is not approximately grey, the spectrum must be integrated explicitly rather than inferred from a peak alone. A coating designed to improve close approach would instead reflect much of the solar radiation while retaining strong thermal [infrared](../../optics.md#infrared) emission.

## ↑ Ancestors (11)

1. [2022](../2022.md)
2. [Past exam of the physics B course of the University of Cambridge](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge.md)
3. [Physics B course of the University of Cambridge](../../university-of-cambridge.md#physics-b-course-of-the-university-of-cambridge)
4. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
