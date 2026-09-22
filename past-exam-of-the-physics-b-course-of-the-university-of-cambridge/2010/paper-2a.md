# Paper 2A

↑ **Parent:** [2010](../2010.md)

Original paper: [Public original PDF, physical pages 265–272](https://www.whatdotheyknow.com/request/physics_past_papers_23/response/3514893/attach/4/FOI%202026%20628%20Smith%20materials.pdf?cookie_passthrough=1#page=265).

**Table of contents**

- [Section A](#section-a)
  - [1](#section-a/1)
    - [Solution](#section-a/1/solution)
  - [2](#section-a/2)
    - [Solution](#section-a/2/solution)
  - [3](#section-a/3)
    - [Solution](#section-a/3/solution)
  - [4](#section-a/4)
    - [Solution](#section-a/4/solution)
  - [5](#section-a/5)
    - [Solution](#section-a/5/solution)
- [Section B](#section-b)
  - [B6](#section-b/b6)
    - [Solution](#section-b/b6/solution)
  - [B7](#section-b/b7)
    - [Solution](#section-b/b7/solution)
  - [B8](#section-b/b8)
    - [Solution](#section-b/b8/solution)
  - [B9](#section-b/b9)
    - [Solution](#section-b/b9/solution)
- [Section C](#section-c)
  - [C10](#section-c/c10)
    - [Solution](#section-c/c10/solution)
  - [C11](#section-c/c11)
    - [Solution](#section-c/c11/solution)
  - [C12](#section-c/c12)
    - [Solution](#section-c/c12/solution)
  - [C13](#section-c/c13)
    - [Solution](#section-c/c13/solution)
- [Section D](#section-d)
  - [D14](#section-d/d14)
    - [Solution](#section-d/d14/solution)
  - [D15](#section-d/d15)
    - [Solution](#section-d/d15/solution)
  - [D16](#section-d/d16)
    - [Solution](#section-d/d16/solution)
  - [D17](#section-d/d17)
    - [a](#section-d/d17/a)
      - [Solution](#section-d/d17/a/solution)
    - [b](#section-d/d17/b)
      - [Solution](#section-d/d17/b/solution)
    - [c](#section-d/d17/c)
      - [Solution](#section-d/d17/c/solution)
    - [d](#section-d/d17/d)
      - [Solution](#section-d/d17/d/solution)

## Section A

↑ **Parent:** [Paper 2A](paper-2a.md)

<h3 id="section-a/1">1</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/1/solution">Solution</h4>

↑ **Parent:** [1](#section-a/1)

For a reversible [isothermal expansion](../../second-law-of-thermodynamics.md#isothermal-expansion) of one mole of an [ideal gas](../../ideal-gas.md), [internal energy](../../internal-energy.md) depends only on [temperature](../../temperature.md), so $\Delta U=0$. The [first law of thermodynamics](../../first-law-of-thermodynamics.md) gives

$$
Q=W=\int_{V_i}^{2V_i}\frac{RT_0}{V}\,dV=\boxed{RT_0\ln2.}
$$

This uses quasistatic expansion against the gas pressure. Specifying only the initial and final volumes and constant [temperature](../../temperature.md) would not fix heat for an arbitrary irreversible process: an insulated ideal-gas free expansion has $Q=W=0$.

<h3 id="section-a/2">2</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/2/solution">Solution</h4>

↑ **Parent:** [2](#section-a/2)

Take the wires along $z$, with the first at $x=0$ carrying $+I\hat{\mathbf z}$, and observe at $x=-a$. The [Biot-Savart law](../../electromagnetism.md#biot-savart-law) gives a first-wire field in $-\hat{\mathbf y}$; wire $n$ is $na$ away. Therefore

$$
\mathbf B=-\frac{\mu_0I}{2\pi a}\hat{\mathbf y}\sum_{n=1}^N(-1)^{n-1}n^2.
$$

Pairing adjacent terms, with $N=2m$,

$$
\sum_{j=1}^m[(2j-1)^2-(2j)^2]
=\sum_{j=1}^m(1-4j)=-\frac{N(N+1)}2.
$$

Thus $\boxed{\mathbf B=\mu_0IN(N+1)\hat{\mathbf y}/(4\pi a)}$. Its direction is opposite to the field of the first wire at the observation point. Reversing every [electric current](../../electric-charge.md#electric-current) reverses this answer.

<h3 id="section-a/3">3</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/3/solution">Solution</h4>

↑ **Parent:** [3](#section-a/3)

An empty perfectly conducting rectangular [electromagnetic waveguide](../../electromagnetic-wave.md#electromagnetic-waveguide) has

$$
\omega^2=c^2\left[k_z^2+\pi^2\left(\frac{m^2}{a^2}+\frac{n^2}{b^2}\right)\right].
$$

The lowest [transverse electric mode](../../electromagnetic-wave.md#transverse-electric-mode) has indices $(1,0)$ or $(0,1)$. A simply connected hollow metallic guide has no [transverse electromagnetic mode](../../electromagnetic-wave.md#transverse-electromagnetic-mode). With $a=b=10^{-2}\,\mathrm m$, the two lowest modes are degenerate and their [cutoff frequency](../../electrical-engineering.md#cutoff-frequency) is

$$
\boxed{f_c=\frac{c}{2a}\simeq15.0\,\mathrm{GHz}.}
$$

Propagation with nonzero axial energy transport requires $f>f_c$; the equality is the lower limiting frequency, with zero axial [group velocity](../../dispersion-relation.md#group-velocity). A filling medium would replace $c$ by $1/\sqrt{\mu\epsilon}$.

<h3 id="section-a/4">4</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/4/solution">Solution</h4>

↑ **Parent:** [4](#section-a/4)

Suppose two distinct reversible [adiabatic processes](../../first-law-of-thermodynamics.md#adiabatic-process) intersect at an equilibrium state $C$. Choose an [isothermal process](../../second-law-of-thermodynamics.md#isothermal-process) that meets the two branches at distinct states $A$ and $B$, forming a nonzero-area three-sided [thermodynamic cycle](../../thermodynamics.md#thermodynamic-cycle). There is no heat exchange on $AC$ or $BC$, so the only net heat comes from the one heat reservoir on $AB$. Since $\Delta U=0$ around a cycle, $W_{\rm cycle}=Q_{AB}$.

Choose the direction in which this nonzero cycle delivers positive work. It would then convert heat from a single reservoir entirely into work, violating the [Kelvin-Planck statement of the second law](../../second-law-of-thermodynamics.md#kelvin-planck-statement-of-the-second-law). **Distinct reversible adiabats cannot intersect.** Equivalently, their constant [entropy](../../entropy.md) labels cannot differ at one equilibrium state. The argument concerns an ordinary equilibrium family of reversible adiabats, not arbitrary irreversible insulated paths. The usual local uniqueness of an equilibrium adiabat excludes coincident segments described as distinct curves.

<h3 id="section-a/5">5</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/5/solution">Solution</h4>

↑ **Parent:** [5](#section-a/5)

The [trihydrogen cation](../../chemistry.md#trihydrogen-cation) is a nonlinear three-nucleus molecule. Removing three translations and three rigid rotations leaves $3(3)-6=3$ vibrational degrees of freedom. One [normal mode](../../wave-equation.md#normal-mode) is the symmetric in-plane breathing motion: every nucleus moves radially toward or away from the centre. The remaining two [normal modes](../../wave-equation.md#normal-mode) form a degenerate in-plane distortion pair, stretching one direction while compressing another.

For an explicit sketch, let $\mathbf r_j$ be the equilibrium vertices relative to their centre. Displacements proportional to

$$
\mathbf u_j^{(1)}=\mathbf r_j,\qquad
\mathbf u_j^{(2)}=\begin{pmatrix}1&0\\0&-1\end{pmatrix}\mathbf r_j,\qquad
\mathbf u_j^{(3)}=\begin{pmatrix}0&1\\1&0\end{pmatrix}\mathbf r_j
$$

give the breathing mode and a basis of the degenerate pair. Linear combinations within the latter pair are equally valid. Their actual frequencies require molecular force constants, which are not supplied. An apparent out-of-plane motion of three point nuclei is a translation or infinitesimal rigid rotation, rather than an additional independent vibration.

<a id="section-a/5/image-breathing-and-degenerate-distortion-modes-of-an-equilateral-molecule"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a-triangular-modes.png)

**[Figure 1](#section-a/5/image-breathing-and-degenerate-distortion-modes-of-an-equilateral-molecule). Breathing and degenerate distortion modes of an equilateral molecule**. Original displacement vectors in a simple symmetric bond-spring illustration. The degeneracy is fixed by symmetry; no measured molecular frequencies are asserted.

## Section B

↑ **Parent:** [Paper 2A](paper-2a.md)

<h3 id="section-b/b6">B6</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b6/solution">Solution</h4>

↑ **Parent:** [B6](#section-b/b6)

Let the unit normal point from layer 1 to layer 2. The electrostatic [electric field](../../electric-field.md) boundary condition is $\mathbf n\times(\mathbf E_2-\mathbf E_1)=0$, while [Gauss's law](../../maxwell-equations.md#gauss-s-law) for the [electric displacement field](../../electromagnetism.md#electric-displacement-field) gives $\mathbf n\cdot(\mathbf D_2-\mathbf D_1)=\sigma_f$. Here $\epsilon_i$ denotes absolute [permittivity](../../permittivity.md); replace it by $\epsilon_0\epsilon_{ri}$ if dielectric constants are relative.

In the steady conducting state, [charge conservation](../../electric-charge.md#charge-conservation) makes the normal [current density](../../electric-charge.md#current-density) the same in both layers:

$$
J=\sigma_1E_1=\sigma_2E_2,\qquad V=E_1d_1+E_2d_2.
$$

Writing $\mathcal D=\sigma_2d_1+\sigma_1d_2$, the [steady fields in two leaky dielectric layers](../../permittivity.md#steady-fields-in-two-leaky-dielectric-layers) are

$$
\boxed{E_1=\frac{\sigma_2V}{\mathcal D},\qquad E_2=\frac{\sigma_1V}{\mathcal D},\qquad J=\frac{\sigma_1\sigma_2V}{\mathcal D}.}
$$

The signed interfacial free [surface charge density](../../electrostatics.md#surface-charge-density) is the jump of $D_n$:

$$
\boxed{\sigma_f=\frac{(\epsilon_2\sigma_1-\epsilon_1\sigma_2)V}{\mathcal D}.}
$$

The total free-plus-bound sheet charge instead follows from the vacuum form of [Gauss's law](../../maxwell-equations.md#gauss-s-law),

$$
\boxed{\sigma_{\rm total}=\epsilon_0(E_2-E_1)
=\frac{\epsilon_0(\sigma_1-\sigma_2)V}{\mathcal D}.}
$$

The bound contribution is $\sigma_{\rm total}-\sigma_f$. These are signed quantities for the chosen normal and voltage direction; their magnitudes are obtained by absolute values. They describe the long-time DC state, not the initial capacitive transient. Positive conductivities suffice for the derivation; if both vanish, conductivity alone does not determine the field division, which also depends on the initial free interfacial charge.

<h3 id="section-b/b7">B7</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b7/solution">Solution</h4>

↑ **Parent:** [B7](#section-b/b7)

[Faraday's law](../../maxwell-equations.md#faraday-s-law-of-induction) for a moving circuit is $\mathcal E=\oint(\mathbf E+\mathbf v\times\mathbf B)\cdot d\boldsymbol\ell=-d\Phi_B/dt$. The [magnetic flux](../../magnetic-field.md#magnetic-flux) $\Phi_B$ is through a surface bounded by the instantaneous loop, with consistent orientation. For the stationary external field here, the motion supplies the [motional electromotive force](../../electric-charge.md#motional-electromotive-force).

Let $x$ be downward penetration of the bottom segment, $v=\dot x$, and $K=B_0a$. While $0<x<b$, flux grows at rate $Kv$. Define positive current as the direction whose [magnetic force](../../relativistic-electromagnetism.md#magnetic-force) is upward. With negligible [self-inductance](../../electromagnetism.md#self-inductance), $I=Kv/R$ and

$$
m\dot v=mg-KI=mg-\frac{K^2}R v,\qquad \tau=\frac{mR}{K^2}.
$$

The [resistive magnetic entry of a falling loop](../../electromagnetism.md#resistive-magnetic-entry-of-a-falling-loop) gives

$$
\boxed{v=g\tau(1-e^{-t/\tau}),\qquad I=\frac{Kg\tau}R(1-e^{-t/\tau}),\qquad
x=g\tau[t-\tau(1-e^{-t/\tau})].}
$$

The initial acceleration is $g$ and the speed approaches $g\tau$ if the loop remains partly immersed long enough. Joule heating $I^2R$ removes gravitational energy. At the first $x=b$, both horizontal segments are inside the uniform field: the net flux becomes constant, the net magnetic force vanishes, and this zero-inductance model has $I=0$ thereafter. The subsequent speed increases with acceleration $g$.

For negligible [electrical resistance](../../electric-charge.md#electrical-resistance), conservation of total linked flux instead gives $LI=Kx$ in the braking-current convention. Therefore

$$
m\ddot x=mg-\frac{K^2}Lx,\qquad \omega=\frac K{\sqrt{mL}},
$$

and the [lossless limit of magnetic loop braking](../../maxwell-equations.md#lossless-limit-of-magnetic-loop-braking) yields

$$
\boxed{x=\frac g{\omega^2}(1-\cos\omega t),\qquad
v=\frac g\omega\sin\omega t,\qquad
I=\frac{mg}K(1-\cos\omega t).}
$$

Here energy is stored reversibly in $LI^2/2$, not dissipated. If $b>2g/\omega^2$, the loop reverses before complete entry and executes the ideal oscillatory motion while straddling the boundary. If $b<2g/\omega^2$, it reaches complete entry on its first descent; thereafter the current is constant, the forces on its two horizontal segments cancel, and it falls with acceleration $g$. The exact grazing case needs care at the ideal discontinuous field boundary. An entry-only sinusoid must not be extrapolated through full immersion.

<a id="section-b/b7/image-resistive-relaxation-and-reversible-inductive-motion-during-loop-entry"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a-loop-entry.png)

**[Figure 2](#section-b/b7/image-resistive-relaxation-and-reversible-inductive-motion-during-loop-entry). Resistive relaxation and reversible inductive motion during loop entry**. Original dimensionless entry solutions. Curves assume that the loop is long enough for the indicated stage; a fully immersed loop has different subsequent dynamics.

<h3 id="section-b/b8">B8</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b8/solution">Solution</h4>

↑ **Parent:** [B8](#section-b/b8)

The fundamental mode of an ideal [coaxial cable](../../electrical-engineering.md#coaxial-cable) is a [transverse electromagnetic mode](../../electromagnetic-wave.md#transverse-electromagnetic-mode): the [electric field](../../electric-field.md) is radial between the conductors, the [magnetic field](../../magnetic-field.md) is azimuthal, and energy flows along the cable through the dielectric. There is no cutoff for this mode; higher modes, conductor losses and dielectric dispersion can matter outside the ideal transmission-line regime.

Ignoring edge fields in the parallel-strip geometry, $E_x=V/a$ and $H_y=I/b$. Per unit length the charge is $\epsilon bV/a$ and the linked magnetic flux is $\mu aI/b$. Thus the [parallel-plate transmission line](../../electrical-engineering.md#parallel-plate-transmission-line) has

$$
\boxed{C=\epsilon\frac ba,\qquad L=\mu\frac ab,\qquad LC=\mu\epsilon.}
$$

For a segment $dz$, [charge conservation](../../electric-charge.md#charge-conservation), equivalently the appropriate integral of the [Ampère-Maxwell equation](../../maxwell-equations.md#ampere-s-circuital-law), gives $I(z)-I(z+dz)=C\,dz\,\partial_tV$. Applying [Faraday's law](../../maxwell-equations.md#faraday-s-law-of-induction) around a longitudinal rectangle between the plates gives $V(z)-V(z+dz)=L\,dz\,\partial_tI$. These are the lossless [telegrapher's equations](../../electrical-engineering.md#telegrapher-s-equations),

$$
\partial_zI=-C\partial_tV,\qquad\partial_zV=-L\partial_tI.
$$

Differentiate the second with respect to $z$ and use the first, and conversely for $I$:

$$
\boxed{\partial_z^2V=LC\partial_t^2V,\qquad\partial_z^2I=LC\partial_t^2I.}
$$

The signal speed is $1/\sqrt{LC}=1/\sqrt{\mu\epsilon}$, equal to $c$ for a vacuum-filled line. It is the speed of the coupled electromagnetic disturbance, rather than the [electron drift velocity](../../electric-charge.md#electron-drift-velocity). Electrons locally adjust their motion as the field arrives; one electron need not travel the cable's length to transmit a signal. The [Poynting vector](../../electromagnetic-wave.md#poynting-vector) in the dielectric integrates to power $VI$.

<h3 id="section-b/b9">B9</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b9/solution">Solution</h4>

↑ **Parent:** [B9](#section-b/b9)

The [method of images](../../mathematics.md#method-of-images) replaces conductors by fictitious charges chosen to reproduce their boundary potentials in the physical domain. The [uniqueness theorem for the electrostatic potential](../../electrostatics.md#uniqueness-theorem-for-the-electrostatic-potential) then identifies the resulting physical exterior field; the fictitious interior field is not the field inside the conductor.

For a source at $d\hat{\mathbf z}$, let $r'=a^2/d$ and $q'=-qa/d$. At a point on $r=a$, the distances $R$ and $R'$ to source and image obey $R'=(a/d)R$. Hence $q/R+q'/R'=0$ everywhere on the sphere. This proves the [image charge for a grounded conducting sphere](../../electric-field.md#image-charge-for-a-grounded-conducting-sphere) construction.

With real charges at $\pm d\hat{\mathbf z}$, superpose two images of charge $-qa/d$ at $\pm a^2\hat{\mathbf z}/d$. For the right-hand charge, take positive force away from the centre. Its [electrostatic force](../../electric-field.md#electrostatic-force) is

$$
F_0=\frac{q^2}{4\pi\epsilon_0}\left[\frac1{4d^2}-\frac ad\left(\frac1{(d-a^2/d)^2}+\frac1{(d+a^2/d)^2}\right)\right].
$$

Putting $x=d/a$, the [equal-charge balance around a grounded sphere](../../electric-field.md#equal-charge-balance-around-a-grounded-sphere) requires

$$
\boxed{\frac1{4x^2}=x\left[\frac1{(x^2-1)^2}+\frac1{(x^2+1)^2}\right].}
$$

For large $x$, the right side is approximately $2/x^3$, so $x\simeq8$. This is an approximate equilibrium, not an exact cancellation at $x=8$.

To hold the sphere at [electric potential](../../electric-field.md#electric-potential) $V$, add a central image $Q_0=4\pi\epsilon_0aV$. The grounded pair already contributes zero potential on its surface. Therefore

$$
\boxed{F=F_0+\frac{qaV}{d^2}.}
$$

At $d=8a$ this is $F_0(8a)+qV/(64a)$, or approximately $qV/(64a)$ if the small grounded residual is neglected as in the preceding approximation. The charge on the sphere is $Q_0-2qa/d$; fixing its potential is different from independently fixing its net charge.

## Section C

↑ **Parent:** [Paper 2A](paper-2a.md)

<h3 id="section-c/c10">C10</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c10/solution">Solution</h4>

↑ **Parent:** [C10](#section-c/c10)

For steady inviscid [incompressible flow](../../fluid-mechanics.md#incompressible-flow) subject to a conservative body force, [Bernoulli's theorem](../../euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) states that $p/\rho+u^2/2+gz$ is constant along a streamline. The same constant applies across streamlines only with an additional condition, such as an irrotational connected flow with the same upstream head.

Neglect gravity and let the film's free-surface pressure be atmospheric. Its radial speed is then $v$ in the ideal model. [Conservation of mass](../../continuum-mechanics.md#mass-conservation) equates the incoming flux $\pi r_1^2v$ to $2\pi rt(r)v$, so

$$
\boxed{t(r)=\frac{r_1^2}{2r},\qquad t(r_1)=\frac{r_1}{2}.}
$$

The latter value already warns that the thin-film approximation is poor near impact; the radial expression is most useful beyond that region. The incoming vertical [momentum flux](../../mathematical-physics.md#momentum-flux) gives downward force $F_m=\rho\pi r_1^2v^2$ when the outgoing flow is horizontal.

In the stipulated stagnant-rear-layer idealization, the excess rear pressure is the stagnation value $\rho v^2/2$. Its upward force is $\rho v^2\pi r_2^2/2$. Thus, with downward positive and ignoring the water's weight,

$$
F=\rho\pi v^2(r_1^2-r_2^2/2),\qquad\boxed{F=0\text{ at }r_2=\sqrt2r_1.}
$$

For a large plate, the radial-film volume is approximately

$$
\int_{r_1}^{r_2}2\pi rt(r)\,dr=\pi r_1^2(r_2-r_1)\simeq\pi r_1^2r_2.
$$

Its weight therefore changes the model to

$$
F\simeq\rho\pi\left[r_1^2v^2+gr_1^2r_2-\frac12v^2r_2^2\right].
$$

Cancellation occurs near

$$
r_{2,*}=\frac{gr_1^2}{v^2}+\sqrt{\frac{g^2r_1^4}{v^4}+2r_1^2}
\simeq\boxed{\frac{2gr_1^2}{v^2}}\quad(v^2\ll gr_1).
$$

**The printed claim of negligible force for every radius above this scale does not follow from this model.** Near the cancellation radius the force is small; for substantially larger radii the quadratic upward-pressure term dominates. The original PDF, not just its transcription, uses that inequality and wording. Moreover, the rear layer's mass and detailed gravity-dependent pressure field are unspecified. The calculation establishes a cancellation scale under the elementary stated pressure approximation, rather than a general large-radius zero-force theorem. A full free-surface flow model would be needed to extend it consistently.

<h3 id="section-c/c11">C11</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c11/solution">Solution</h4>

↑ **Parent:** [C11](#section-c/c11)

For a [Lagrangian](../../calculus-of-variations.md#lagrangian) $\mathcal L=T-U$, the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) is $d(\partial\mathcal L/\partial\dot q)/dt=\partial\mathcal L/\partial q$ for each unconstrained generalized coordinate. For example, $\mathcal L=m\dot x^2/2-kx^2/2$ gives $m\ddot x+kx=0$ for a spring oscillator.

For a uniform solid sphere, slicing into disks normal to the rotation axis gives

$$
I=\frac\rho2\int_{-R}^R\pi(R^2-z^2)^2\,dz
=\frac{8\pi\rho R^5}{15}=\frac25mR^2.
$$

Use total dumb-bell mass $M$ and $\ell=L-r$. Since both centres lie on its spin axis, its [moment of inertia](../../rigid-body-dynamics.md#moment-of-inertia) about that axis is $2MR^2/5$. If $\theta$ measures displacement from the bottom of the track, [rolling without slipping](../../rigid-body-dynamics.md#rolling-without-slipping) imposes spin speed $|\dot\phi|=\ell|\dot\theta|/r$. The [rolling inside a fixed circular cylinder](../../rigid-body-dynamics.md#rolling-inside-a-fixed-circular-cylinder) therefore has

$$
\mathcal L=\frac12M\ell^2\left(1+\frac{2R^2}{5r^2}\right)\dot\theta^2-Mg\ell(1-\cos\theta).
$$

The equation of motion and its small-amplitude limit are

$$
\ddot\theta+\frac{g\sin\theta}{\ell(1+2R^2/(5r^2))}=0,\qquad
\boxed{\omega=\sqrt{\frac g{L-r}}\left(1+\frac{2R^2}{5r^2}\right)^{-1/2}.}
$$

With $g=9.81\,\mathrm{m\,s^{-2}}$ and the given lengths, $\boxed{T=2\pi/\omega\simeq80.5\,\mathrm s}$. If the centre rises by height $h$, [conservation of energy](../../mathematical-physics.md#conservation-of-energy) at the bottom gives

$$
Mgh=\frac12M\left(1+\frac{2R^2}{5r^2}\right)v_{\max}^2,
\qquad\boxed{v_{\max}\simeq0.0349\,\mathrm{m\,s^{-1}}\quad(h=0.010\,\mathrm m).}
$$

The speed expression uses exact height-energy conversion within the ideal rolling constraint; only the period formula uses the small-angle approximation.

<h3 id="section-c/c12">C12</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c12/solution">Solution</h4>

↑ **Parent:** [C12](#section-c/c12)

Let $J_p=\int r^2dA=\pi a^4/2$ be the polar second moment of area. A twist gradient $\partial_x\theta$ gives shear strain $r\partial_x\theta$ and shear stress $Gr\partial_x\theta$. Integrating its moment over a cross section yields

$$
\boxed{C=GJ_p\frac\phi l=\frac{\pi a^4G}{2l}\phi.}
$$

The difference in torque on an element $dx$ is $GJ_p\partial_x^2\theta\,dx$, while its angular inertia is $\rho J_pdx$. Hence the [torsional wave equation in a circular shaft](../../wave-equation.md#torsional-wave-equation-in-a-circular-shaft) is

$$
\boxed{\partial_t^2\theta=\frac G\rho\partial_x^2\theta,\qquad c_T=\sqrt{G/\rho}.}
$$

For uniform rotation at $\Omega$, transmitted power is $P=C\Omega$, so the given values give $C=100\,\mathrm{N\,m}$. The [elastic strain energy](../../elasticity-physics.md#elastic-energy) and [rotational kinetic energy](../../energy.md#rotational-kinetic-energy) are

$$
\phi=\frac{Cl}{GJ_p}=\boxed{9.95\times10^{-3}\,\mathrm{rad}},\qquad
U=\frac{C^2l}{2GJ_p}=\boxed{0.497\,\mathrm J},\qquad
K=\frac12\rho J_pl\Omega^2=\boxed{181\,\mathrm J}.
$$

The torsional transit time is $l/c_T=6.32\times10^{-4}\,\mathrm s$. If the requested maximum rates mean stored-energy-over-transit-time estimates, they are

$$
\boxed{\frac{c_TU}{l}\simeq786\,\mathrm W,\qquad\frac{c_TK}{l}\simeq286\,\mathrm{kW}.}
$$

These estimates require a physical qualification. They are not separate upper bounds on transmitted mechanical power. The exact local [energy flux of a torsional wave](../../wave-equation.md#energy-flux-of-a-torsional-wave) is the stress-work rate

$$
\mathcal P=-GJ_p(\partial_x\theta)(\partial_t\theta).
$$

For the steadily rotating twisted shaft its magnitude is $C\Omega=30\,\mathrm{kW}$, even though this exceeds $c_TU/l$. Writing local energy densities $u_s=GJ_p\theta_x^2/2$ and $u_k=\rho J_p\theta_t^2/2$ gives $|\mathcal P|=2c_T\sqrt{u_su_k}\le c_T(u_s+u_k)$. A single travelling torsional wave has equal strain and kinetic energies; the steady shaft can instead be represented by oppositely travelling components whose powers largely cancel. Its stored strain pattern is not a fuel consumed once per transit. This distinguishes an energy-content estimate from the actual stress-mediated transport.

<h3 id="section-c/c13">C13</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c13/solution">Solution</h4>

↑ **Parent:** [C13](#section-c/c13)

In plane polar coordinates the radial component of [Newton's second law](../../force.md#newton-s-second-law) is $m(\ddot r-r\dot\theta^2)=-U'(r)$. A [central force](../../mathematical-physics.md#central-force) has zero torque, so [angular momentum](../../momentum.md#angular-momentum) $J=mr^2\dot\theta$ is constant. Therefore

$$
\boxed{m\ddot r=-U'(r)+\frac{J^2}{mr^3}=-U_{\rm eff}'(r),\qquad
U_{\rm eff}=Br^n+\frac{J^2}{2mr^2}.}
$$

For a nonzero-angular-momentum circular orbit at $r_0$, $nBr_0^{n+2}=J^2/m$. The curvature there is

$$
U_{\rm eff}''(r_0)=n(n+2)Br_0^{n-2}.
$$

Thus a stable circular orbit, and nearby bound orbits, require $\boxed{nB>0,\ n>-2}$, with $n=0$ excluded. For $n>0$, $B>0$ confines the particle at large radius; for $-2<n<0$, $B<0$ permits bound energies between the effective-potential minimum and zero. At $n=-2$ there is no isolated stable minimum.

The angular frequency is $\Omega^2=nBr_0^{n-2}/m$, and radial perturbations have frequency $\kappa=\sqrt{n+2}\,\Omega$. A rational ratio $\kappa/\Omega$ closes the _linearized_ near-circular trajectory. It does not prove finite-amplitude closure. [Bertrand's theorem](../../mathematical-physics.md#bertrand-s-theorem) supplies the stronger conclusion: **every bound orbit is closed only for $n=-1$ and $n=2$** among these smooth attractive power-law potentials. Particular circular or resonant orbits must not be confused with that all-orbit statement.

For $n=2+\epsilon$, the slowly rotating elliptical orientation has angular speed

$$
\Omega_{\rm prec}=\Omega-\frac\kappa2
=\Omega\left(1-\frac{\sqrt{4+\epsilon}}2\right)
=\boxed{-\frac\epsilon8\Omega+O(\epsilon^2\Omega).}
$$

This is retrograde for $\epsilon>0$ in the near-circular approximation. Consecutive radial maxima are separated by approximately $\pi$ in azimuth; the ellipse's axis is defined modulo $\pi$, which accounts for the factor of two relative to a Kepler-style apsidal convention.

## Section D

↑ **Parent:** [Paper 2A](paper-2a.md)

<h3 id="section-d/d14">D14</h3>

↑ **Parent:** [Section D](#section-d)

Source for this section: [Physical PDF pages 271–272, printed pages 7–8 of Physics B (2A), 2 June 2010](https://www.whatdotheyknow.com/request/physics_past_papers_23/response/3514893/attach/4/FOI%202026%20628%20Smith%20materials.pdf?cookie_passthrough=1#page=271).

<h4 id="section-d/d14/solution">Solution</h4>

↑ **Parent:** [D14](#section-d/d14)

A [normal mode](../../wave-equation.md#normal-mode) has all [displacement](../../classical-mechanics.md#displacement) coordinates proportional to a common time dependence, with fixed relative amplitudes. For a nonzero [frequency](../../wave.md#frequency) the time dependence is sinusoidal. A zero-frequency mode is a free [displacement](../../classical-mechanics.md#displacement) or uniform drift rather than an [oscillation](../../wave.md#oscillation).

Use the printed mass ordering $M,m,M$. [Displacements](../../classical-mechanics.md#displacement) are measured from the unstretched [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) positions, giving

$$
M\ddot x_1=k(x_2-x_1),\qquad
m\ddot x_2=k(x_1-2x_2+x_3),\qquad
M\ddot x_3=k(x_2-x_3).
$$

Equivalently,

$$
\boxed{\mathsf M\ddot{\mathbf x}+\mathsf K\mathbf x=0,\quad
\mathsf M=\operatorname{diag}(M,m,M),\quad
\mathsf K=k\begin{pmatrix}1&-1&0\\-1&2&-1\\0&-1&1\end{pmatrix}.}
$$

This is the [generalized eigenvalue problem](../../linear-operator-theory.md#generalized-eigenvalue-problem) for [normal modes of three masses connected by two equal springs](../../lagrangian-mechanics.md#normal-modes-of-three-masses-connected-by-two-equal-springs). Substitute $\mathbf x=\mathbf u e^{i\omega t}$ to obtain $\mathsf K\mathbf u=\omega^2\mathsf M\mathbf u$. [Reflection symmetry](../../physics.md#reflection-symmetry) gives an antisymmetric [vector](../../vector-space.md#vector) $(1,0,-1)$ and [symmetric](../../set-theory.md#symmetric-relation) [vectors](../../vector-space.md#vector) $(1,b,1)$. The former has $\omega^2=k/M$. For a [symmetric](../../set-theory.md#symmetric-relation) [vector](../../vector-space.md#vector), the end and centre equations give $M\omega^2=k(1-b)$ and $m\omega^2b=2k(b-1)$. Their solutions are $b=1$, $\omega=0$, or $b=-2M/m$, $\omega^2=k/M+2k/m$. Hence

$$
\boxed{\begin{array}{c|c|l}
\mathbf u&\omega^2&\text{relative motion}\\\hline
(1,1,1)&0&\text{rigid translation, neither spring stretched}\\
(1,0,-1)&k/M&\text{end masses opposite, centre fixed}\\
(1,-2M/m,1)&k/M+2k/m&\text{ends together, centre opposite}.
\end{array}}
$$

These are all three [eigenmodes](../../wave-equation.md#normal-mode). The last two keep the [centre of mass](../../classical-mechanics.md#center-of-mass) fixed and are [orthogonal](../../inner-product.md#orthogonal-vectors) in the mass-weighted [inner product](../../inner-product.md). The general zero-mode contribution is $(A+Bt)(1,1,1)$, accounting for both a centre-of-mass shift and a conserved total [momentum](../../momentum.md). There are no fixed end springs in this system.

<a id="section-d/d14/image-free-chain-mode-shapes"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a-three-mass-modes.png)

**[Figure 3](#section-d/d14/image-free-chain-mode-shapes). Free-chain mode shapes**.

The original amplitude profiles illustrate $M=2m$; the [symmetric](../../set-theory.md#symmetric-relation) internal shape is rescaled for display. The formula above gives every positive mass ratio.

Two further physical examples are **standing-wave modes of a string fixed at both ends**, with spatial shapes $\sin(n\pi x/L)$ and [frequencies](../../wave.md#frequency) $n\pi c/L$, and **electrical [normal modes](../../wave-equation.md#normal-mode) of two coupled [LC circuits](../../electrical-circuit.md#lc-circuit)**, in which the [capacitor](../../electromagnetism.md#capacitor) charges oscillate at fixed relative amplitudes. Independent [normal mode coordinates](../../classical-mechanics.md#normal-coordinate) simplify both systems in the same way as the spring-chain [eigenvectors](../../linear-operator-theory.md#eigenvector).

<h3 id="section-d/d15">D15</h3>

↑ **Parent:** [Section D](#section-d)

<h4 id="section-d/d15/solution">Solution</h4>

↑ **Parent:** [D15](#section-d/d15)

A [Fourier series](../../fourier-series.md) separates a periodic physical [signal](../../electrical-engineering.md#signal) into harmonics. For example, a periodic [voltage](../../random-walk.md#voltage) applied to a linear circuit can be treated one [frequency](../../wave.md#frequency) at a time; the harmonic responses then superpose to give the output waveform.

Write $w=\Delta T$ for the pulse width and $\delta=w/T$ for its [duty cycle](../../electrical-circuit.md#duty-cycle), with $0<w<T$. The waveform is a train of positive [rectangular pulses](../../electrical-engineering.md#rectangular-function) centred on $t=jT$, each with area one. It is even about $t=0$, so every [sine](../../geometry-and-topology.md#sine) coefficient vanishes. [Cosine](../../geometry-and-topology.md#cosine) [orthogonality](../../inner-product.md#orthogonal-vectors) gives

$$
a_0=\frac2T\int_{-T/2}^{T/2}f(t)\,dt=\frac2T,
$$

and, for $n\geq1$,

$$
a_n=\frac2{Tw}\int_{-w/2}^{w/2}\cos\frac{2\pi nt}{T}\,dt
=\frac{2}{\pi nw}\sin\frac{\pi nw}{T}.
$$

This is the [Fourier series of a periodic rectangular pulse](../../fourier-series.md#fourier-series-of-a-periodic-rectangular-pulse):

$$
\boxed{a_n=\frac2T\operatorname{sinc}(\pi n\delta)\quad(n\geq0),\qquad
\operatorname{sinc}z=\frac{\sin z}{z},\quad\operatorname{sinc}0=1.}
$$

The actual constant term in the series is $a_0/2=1/T$, not $a_0$. As usual for a [jump discontinuity](../../calculus.md#jump-discontinuity), the series converges to the average of the one-sided values at each pulse edge, namely $1/(2w)$, irrespective of the value assigned at that isolated endpoint. Elsewhere it converges to the rectangular waveform.

Counting the constant as the first term, the first three terms are

$$
\frac1T,\qquad \frac2T\operatorname{sinc}(\pi\delta)\cos\frac{2\pi t}{T},\qquad
\frac2T\operatorname{sinc}(2\pi\delta)\cos\frac{4\pi t}{T},
$$

so their sum is

$$
\boxed{S_2(t)=\frac1T+\frac2T\left[\operatorname{sinc}(\pi\delta)\cos\frac{2\pi t}{T}+\operatorname{sinc}(2\pi\delta)\cos\frac{4\pi t}{T}\right].}
$$

If “first three” instead means the first three nonconstant harmonics, add $a_3\cos(6\pi t/T)$; the original plot shows that alternative partial sum as well. The three-term approximation rounds the narrow peaks and ripples between them; many harmonics are needed to represent a sharp pulse.

<a id="section-d/d15/image-rectangular-pulse-harmonics"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a-pulse-fourier.png)

**[Figure 4](#section-d/d15/image-rectangular-pulse-harmonics). Rectangular pulse harmonics**.

The original sketches use the illustrative [duty cycle](../../electrical-circuit.md#duty-cycle) $\delta=0.15$ and cover $-T\leq t\leq T$. The coefficient panel also displays the first spectral zero.

For $n\delta\ll1$, expand the [sinc function](../../fourier-transform.md#sinc-function):

$$
\boxed{a_n=\frac2T\left[1-\frac{\pi^2n^2\delta^2}{6}+O(n^4\delta^4)\right]\simeq\frac2T.}
$$

Thus the low-index coefficients, including $a_0$, have nearly equal values, although their _constant-series contribution_ still has the factor $1/2$. The first sinc zero occurs at $n\delta=1$, or $n=T/w$. If this is not an integer, the closest integer coefficient is near zero rather than exactly zero: writing $n\delta=1+\varepsilon$ gives $a_n\simeq-(2/T)\varepsilon$. This [pulse-width scale of Fourier coefficients](../../fourier-series.md#pulse-width-scale-of-fourier-coefficients) means that a narrower pulse requires significant harmonics extending to proportionally larger indices, the reciprocal time-width/frequency-width relation.

<h3 id="section-d/d16">D16</h3>

↑ **Parent:** [Section D](#section-d)

<h4 id="section-d/d16/solution">Solution</h4>

↑ **Parent:** [D16](#section-d/d16)

[Linearity](../../vector-space.md#linearity) means that the [differential operator](../../analysis.md#differential-operator) $L=\partial_x^2-c^{-2}\partial_t^2$ obeys $L(ay_1+by_2)=aLy_1+bLy_2$. Therefore any [linear combination](../../vector-space.md#linear-combination) of homogeneous solutions is again a solution; associated initial or boundary data must be combined by the same rule.

With [characteristic coordinates](../../partial-differential-equation.md#characteristic-coordinate) $\xi=x-ct$ and $\eta=x+ct$, the equation becomes $4y_{\xi\eta}=0$. Integrating in these coordinates gives

$$
\boxed{y=F(x-ct)+G(x+ct).}
$$

The two profiles propagate without changing shape at speeds $+c$ and $-c$. Equivalently write $y=P(t-x/c)+Q(t+x/c)$. At $x=0$, the data imply $P+Q=f$ and $-P'+Q'=0$. Hence $P-Q$ is constant; its two contributions cancel in $y$, giving

$$
\boxed{y(x,t)=\tfrac12[f(t-x/c)+f(t+x/c)],\qquad
y_x(x,t)=\frac{-f'(t-x/c)+f'(t+x/c)}{2c}.}
$$

The slope formula holds classically wherever the two [derivatives](../../calculus.md#derivative) exist, and as a [weak derivative](../../distribution-theory.md#weak-derivative) otherwise. Since the string [tension](../../force.md#tension) is $\rho c^2$, $\rho$ here must be mass per unit length. These are [two-sided string data with zero slope](../../wave-equation.md#two-sided-string-data-with-zero-slope). The stipulated boundary data specify **incoming as well as outgoing waves**; this is not a pulse generated on an everywhere initially resting infinite string. For example, at a positive observation point its incoming [signal](../../electrical-engineering.md#signal) can begin before the motion at $x=0$ begins.

For explicit profiles put $u=t/a$, $s=x/(ca)$ and

$$
h(v)=\begin{cases}\sin(\pi v),&|v|\leq1,\\0,&|v|>1.\end{cases}
$$

Then $y_s(u)=[h(u-s)+h(u+s)]/2$ and $ca\,y_x=[-h'(u-s)+h'(u+s)]/2$. At ordinary points, $h'(v)=\pi\cos(\pi v)$ for $|v|<1$ and zero for $|v|>1$. Because $h$ itself vanishes at both support edges, this first [weak derivative](../../distribution-theory.md#weak-derivative) has **no delta-function term**, although it has jumps.

At $x=ca/2$, the [displacement](../../classical-mechanics.md#displacement) is

$$
\boxed{y_{1/2}(u)=\begin{cases}
\tfrac12\cos(\pi u),&-3/2<u<-1/2,\\
-\tfrac12\cos(\pi u),&1/2<u<3/2,\\
0,&\text{otherwise}.
\end{cases}}
$$

For non-front times its slope is

$$
\boxed{ca\,y_x=\begin{cases}
-\tfrac\pi2\sin(\pi u),&-3/2<u<-1/2,\\
-\pi\sin(\pi u),&-1/2<u<1/2,\\
-\tfrac\pi2\sin(\pi u),&1/2<u<3/2,\\
0,&|u|>3/2.
\end{cases}}
$$

This is [displacement cancellation without slope cancellation in crossing pulses](../../wave-equation.md#displacement-cancellation-without-slope-cancellation-in-crossing-pulses): **[displacement](../../classical-mechanics.md#displacement) cancels throughout the overlap $-1/2<u<1/2$, but slope generally does not.** Cancellation at one spatial position for an interval of time does not imply cancellation of the [spatial derivative](../../multivariable-calculus.md#spatial-derivative) there. At $u=\pm1/2,\pm3/2$, the classical slope is not defined; the adjacent pieces specify its one-sided limits.

At $x=ca$ the two windows meet without an open overlap. Their [displacements](../../classical-mechanics.md#displacement) combine into

$$
\boxed{y_1(u)=\begin{cases}-\tfrac12\sin(\pi u),&-2\leq u\leq2,\\0,&|u|>2,\end{cases}}
$$

with slope

$$
\boxed{ca\,y_x=\begin{cases}
-\tfrac\pi2\cos(\pi u),&-2<u<0,\\
\tfrac\pi2\cos(\pi u),&0<u<2,\\
0,&|u|>2\ \text{or }u=0.
\end{cases}}
$$

At $u=\pm2$ the classical slope is undefined. At the exceptional meeting time $u=0$, oddness of $f$ gives $y(x,0)=0$ for every $x$, so the [spatial derivative](../../multivariable-calculus.md#spatial-derivative) is **exactly zero** there. Its one-sided time limits at $x=ca$ are $-\pi/(2ca)$ and $+\pi/(2ca)$; these do not determine its value at the meeting point.

<a id="section-d/d16/image-displacement-and-slope-pulses"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a-string-boundary-pulse.png)

**[Figure 5](#section-d/d16/image-displacement-and-slope-pulses). Displacement and slope pulses**.

The original graphs distinguish continuous [displacements](../../classical-mechanics.md#displacement), open-ended one-sided slope traces, and the zero slope at the isolated meeting point. The sharp temporal window is not differentiable at its endpoints, so the overall solution is piecewise classical and globally weak. In particular the literal boundary slope at $(x,t)=(0,\pm a)$ is not a classical [derivative](../../calculus.md#derivative): the even spatial profile has a cusp there. The zero-slope boundary prescription is satisfied at regular times and in its almost-everywhere trace sense; it cannot be read as a globally smooth classical condition for this nonsmooth $f$.

<h3 id="section-d/d17">D17</h3>

↑ **Parent:** [Section D](#section-d)

<h4 id="section-d/d17/a">a</h4>

↑ **Parent:** [D17](#section-d/d17)

<h5 id="section-d/d17/a/solution">Solution</h5>

↑ **Parent:** [A](#section-d/d17/a)

**[Stokes theorem](../../multivariable-calculus.md#stokes-theorem) converts [circulation](../../vorticity.md#circulation-physics) around an oriented boundary into [curl](../../multivariable-calculus.md#curl) [flux](../../mathematical-physics.md#flux) through a spanning surface.** For a sufficiently smooth [vector field](../../multivariable-calculus.md#vector-field) on an oriented piecewise smooth surface $S$,

$$
\boxed{\oint_{\partial S}\mathbf A\cdot d\mathbf l=\int_S(\nabla\times\mathbf A)\cdot\mathbf n\,dS.}
$$

The boundary orientation follows the [right-hand rule](../../electromagnetism.md#right-hand-rule) relative to $\mathbf n$. The field must be smooth on the surface, not merely on its boundary; a singularity crossing the surface cannot be ignored. For a fixed loop, applying the theorem to Faraday's differential law gives the [integral](../../integral.md) [flux](../../mathematical-physics.md#flux) law of induction.

The planar form is [Green theorem](../../multivariable-calculus.md#green-theorem). For a region $D$ with positively oriented boundary and sufficiently smooth $P,Q$,

$$
\boxed{\oint_{\partial D}(P\,dx+Q\,dy)=\iint_D(Q_x-P_y)\,dx\,dy.}
$$

The outer boundary is counterclockwise and any holes have clockwise boundaries. For instance $P=-y/2,Q=x/2$ makes the area of $D$ equal to half the [line integral](../../multivariable-calculus.md#line-integral) of $x\,dy-y\,dx$; the unit circle gives area $\pi$.

A closely related use of “[Green's theorems](../../multivariable-calculus.md#green-theorem)” in field theory is [Green's identities](../../partial-differential-equation.md#green-s-identities), obtained by applying the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) to $\phi\nabla\psi$:

$$
\int_V(\phi\nabla^2\psi+\nabla\phi\cdot\nabla\psi)\,dV=\oint_{\partial V}\phi\,\partial_n\psi\,dS,
$$

and, after subtracting the expression with $\phi,\psi$ exchanged,

$$
\boxed{\int_V(\phi\nabla^2\psi-\psi\nabla^2\phi)\,dV=\oint_{\partial V}(\phi\partial_n\psi-\psi\partial_n\phi)\,dS.}
$$

These relate interior sources to boundary data in [electrostatics](../../electrostatics.md) and other boundary-value problems. For example, a [harmonic potential](../../energy.md#harmonic-potential) difference vanishing on a [Dirichlet boundary condition](../../differential-equation.md#dirichlet-boundary-condition) has zero [integral](../../integral.md) of its squared [gradient](../../multivariable-calculus.md#gradient) by the first identity, establishing uniqueness. Both the planar [circulation](../../vorticity.md#circulation-physics) theorem and the field identities are included here to make the convention clear.

<h4 id="section-d/d17/b">b</h4>

↑ **Parent:** [D17](#section-d/d17)

<h5 id="section-d/d17/b/solution">Solution</h5>

↑ **Parent:** [B](#section-d/d17/b)

**[Separation of variables](../../partial-differential-equation.md#separation-of-variables) replaces a compatible [partial differential equation](../../partial-differential-equation.md) by ordinary differential [eigenvalue](../../linear-operator-theory.md#eigenvalue) equations.** For example, with a thermally diffusive rod, $u_t=D u_{xx}$, try $u=X(x)T(t)$. Wherever division is valid,

$$
\frac{T'}{DT}=\frac{X''}{X}=-\lambda.
$$

The two sides depend on independent variables, so each must be constant. Homogeneous end temperatures $u(0,t)=u(L,t)=0$ give $X_n=\sin(n\pi x/L)$ and $\lambda_n=(n\pi/L)^2$. The general initial-temperature profile is represented by superposing these separated modes:

$$
\boxed{u(x,t)=\sum_{n=1}^\infty b_n\sin\frac{n\pi x}{L}\,e^{-D(n\pi/L)^2t},\qquad
b_n=\frac2L\int_0^L u(x,0)\sin\frac{n\pi x}{L}\,dx.}
$$

Each spatial mode decays at its own rate. For a fixed-end [wave equation](../../wave-equation.md) the same spatial [eigenfunctions](../../linear-operator-theory.md#eigenfunction) instead have oscillatory time factors $A_n\cos(cn\pi t/L)+B_n\sin(cn\pi t/L)$, with coefficients fixed by initial [displacement](../../classical-mechanics.md#displacement) and velocity. Similar constructions separate [Laplace's equation](../../partial-differential-equation.md#laplace-equation) in suitable coordinate systems.

A single product is usually only one mode, not the most general solution. Linear [superposition](../../vector-space.md#superposition-principle) and [completeness](../../topological-analysis.md#completeness) of the spatial [eigenfunctions](../../linear-operator-theory.md#eigenfunction) are what extend the method to general allowed data. Nonhomogeneous boundary values can first be removed by a known stationary or particular solution. Separation is effective when the geometry, coefficients and [boundary conditions](../../differential-equation.md#boundary-condition) admit a common separated eigenproblem; an arbitrary nonlinear equation or inseparable geometry need not do so. Self-adjoint [Sturm-Liouville problems](../../sturm-liouville-theory.md#sturm-liouville-problem) explain the weighted [orthogonality](../../inner-product.md#orthogonal-vectors) and [completeness](../../topological-analysis.md#completeness) in many physical applications.

<h4 id="section-d/d17/c">c</h4>

↑ **Parent:** [D17](#section-d/d17)

<h5 id="section-d/d17/c/solution">Solution</h5>

↑ **Parent:** [C](#section-d/d17/c)

**[Convolution](../../fourier-analysis.md#convolution) describes the response of a [linear time-invariant system](../../electrical-engineering.md#linear-time-invariant-system) to an arbitrary input.** If $h$ is its [impulse response](../../green-s-function.md#impulse-response) and $f$ its input,

$$
\boxed{g(t)=(h*f)(t)=\int_{-\infty}^{\infty}h(t-\tau)f(\tau)\,d\tau.}
$$

This is a weighted sum of responses to shifted [impulses](../../classical-mechanics.md#impulse). For integrable [functions](../../function.md) the operation is commutative and associative. A causal system has $h(t)=0$ for $t<0$, restricting the [integral](../../integral.md) to past inputs. With the Fourier convention $F(\omega)=\int f(t)e^{-i\omega t}dt$, the [convolution theorem](../../fourier-analysis.md#convolution-theorem) gives $G=HF$.

For example, an [RC low-pass frequency response](../../electrical-engineering.md#rc-low-pass-frequency-response) has $h(t)=\tau_0^{-1}e^{-t/\tau_0}\Theta(t)$ and $H(\omega)=(1+i\omega\tau_0)^{-1}$, where $\Theta$ is the [Heaviside step function](../../integral-transform.md#heaviside-step-function). Fast input variations are smoothed. The same mathematics describes optical blurring by a [point spread function](../../point-spread-function.md) and many other [linear response](../../statistical-physics.md#linear-response-theory) measurements.

[Deconvolution](../../fourier-analysis.md#deconvolution) tries to recover $f$ from measured $g$ and known $h$. In noise-free data one formally sets $F=G/H$ where $H\ne0$. Zeros of $H$ lose corresponding information; small values amplify measurement [noise](../../electrical-engineering.md#noise-signal-processing). If the measured spectrum is $G+N$, the direct estimate has error $N/H$, which can be very large at [frequencies](../../wave.md#frequency) strongly suppressed by the instrument. An inverse is therefore not automatically unique or stable.

One [regularized spectral deconvolution](../../fourier-analysis.md#regularized-spectral-deconvolution) reconstruction is

$$
\boxed{F_\lambda(\omega)=\frac{H(\omega)^*G(\omega)}{|H(\omega)|^2+\lambda},\qquad\lambda>0.}
$$

This minimizes $|HF-G|^2+\lambda|F|^2$ at each [frequency](../../wave.md#frequency) and limits [noise](../../electrical-engineering.md#noise-signal-processing) amplification, at the cost of bias and lost resolution. Choosing the regularization requires assumptions about [noise](../../electrical-engineering.md#noise-signal-processing) and the desired [signal](../../electrical-engineering.md#signal); [deconvolution](../../fourier-analysis.md#deconvolution) cannot restore components that the data do not determine without such additional information.

<h4 id="section-d/d17/d">d</h4>

↑ **Parent:** [D17](#section-d/d17)

<h5 id="section-d/d17/d/solution">Solution</h5>

↑ **Parent:** [D](#section-d/d17/d)

**[Orthogonality](../../inner-product.md#orthogonal-vectors) means zero [inner product](../../inner-product.md), not merely that two objects look different.** For complex [vectors](../../vector-space.md#vector), $\langle u,v\rangle=\sum_i u_i^*v_i$; for [functions](../../function.md) a common choice is $\langle u,v\rangle=\int w(x)u(x)^*v(x)dx$ with positive weight $w$. An [orthonormal set](../../inner-product.md#orthonormal-set) has $\langle u_m,u_n\rangle=\delta_{mn}$.

For an [orthogonal](../../inner-product.md#orthogonal-vectors) set, the component of $f$ along $u_n$ has coefficient

$$
\boxed{c_n=\frac{\langle u_n,f\rangle}{\langle u_n,u_n\rangle}.}
$$

A complete [orthonormal set](../../inner-product.md#orthonormal-set) gives $f=\sum_nc_nu_n$ in the appropriate [norm](../../normed-vector-space.md#norm) and [Parseval's identity](../../fourier-analysis.md#parseval-identity) $\|f\|^2=\sum_n|c_n|^2$. Without [completeness](../../topological-analysis.md#completeness) there can be a nonzero residual [orthogonal](../../inner-product.md#orthogonal-vectors) to the entire chosen set. [Orthogonal](../../inner-product.md#orthogonal-vectors) nonzero [vectors](../../vector-space.md#vector) are [linearly independent](../../vector-space.md#linear-independence), but independence alone does not imply [orthogonality](../../inner-product.md#orthogonal-vectors).

[Fourier coefficients](../../fourier-series.md#fourier-coefficient) are [projections](../../vector-space.md#projection-linear-algebra) because

$$
\int_0^T e^{-2\pi imt/T}e^{2\pi int/T}\,dt=T\delta_{mn}.
$$

Likewise, for a [self-adjoint operator](../../linear-operator-theory.md#self-adjoint-operator), $Au_n=\lambda_nu_n$ gives $(\lambda_n-\lambda_m)\langle u_m,u_n\rangle=0$, so distinct [eigenvalues](../../linear-operator-theory.md#eigenvalue) have [orthogonal](../../inner-product.md#orthogonal-vectors) [eigenvectors](../../linear-operator-theory.md#eigenvector). Degeneracy does not itself force a chosen pair to be [orthogonal](../../inner-product.md#orthogonal-vectors), but an [orthonormal basis](../../inner-product.md#orthonormal-basis) can be selected within each [eigenspace](../../linear-operator-theory.md#eigenspace). The differential version uses the correct Sturm-Liouville weight and [boundary conditions](../../differential-equation.md#boundary-condition).

For mechanical [normal modes](../../wave-equation.md#normal-mode) with unequal masses the relevant [inner product](../../inner-product.md) is $\langle u,v\rangle_{\mathsf M}=u^\dagger\mathsf Mv$. This makes the modes in D14 [orthogonal](../../inner-product.md#orthogonal-vectors) even when an ordinary unweighted dot product does not. Expanding in such coordinates diagonalizes the kinetic and potential [quadratic forms](../../quadratic-form.md), explaining why modal motions evolve independently and their [energies](../../energy.md) add.

## ↑ Ancestors (11)

1. [2010](../2010.md)
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

## ← Incoming links (1)

- [Paper 2B](paper-2b.md)
