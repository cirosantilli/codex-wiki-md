# Paper 1

↑ **Parent:** [2022](../2022.md)

[Original paper, released PDF pages 242–247](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e/response/2127325/attach/3/FOI%202022%20639%20Sullivan%20materials.pdf?cookie_passthrough=1#page=242)

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
    - [a](#section-b/b6/a)
      - [Solution](#section-b/b6/a/solution)
    - [b](#section-b/b6/b)
      - [Solution](#section-b/b6/b/solution)
    - [c](#section-b/b6/c)
      - [Solution](#section-b/b6/c/solution)
    - [d](#section-b/b6/d)
      - [Solution](#section-b/b6/d/solution)
    - [e](#section-b/b6/e)
      - [Solution](#section-b/b6/e/solution)
  - [B7](#section-b/b7)
    - [a](#section-b/b7/a)
      - [Solution](#section-b/b7/a/solution)
    - [b](#section-b/b7/b)
      - [Solution](#section-b/b7/b/solution)
    - [c](#section-b/b7/c)
      - [Solution](#section-b/b7/c/solution)
    - [d](#section-b/b7/d)
      - [Solution](#section-b/b7/d/solution)
    - [e](#section-b/b7/e)
      - [Solution](#section-b/b7/e/solution)
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
    - [f](#section-c/c9/f)
      - [Solution](#section-c/c9/f/solution)

## Section A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="section-a/a1">A1</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a1/solution">Solution</h4>

↑ **Parent:** [A1](#section-a/a1)

The transfer is a [Hohmann transfer orbit](../../celestial-mechanics.md#hohmann-transfer-orbit). Write $r_0$ for the original [circular Kepler orbit](../../celestial-mechanics.md#circular-kepler-orbit) radius and $a_t$ for the transfer [ellipse](../../euclidean-geometry.md#ellipse)'s [semi-major axis](../../celestial-mechanics.md#semi-major-axis). The diagram measures both radii from [Earth](../../planetary-science.md#earth)'s centre, giving $r_1=1.2r_0$, and hence

$$
a_t=\frac{r_0+r_1}{2}=1.1r_0.
$$

The [Hohmann transfer time](../../celestial-mechanics.md#hohmann-transfer-time) is half the transfer [orbital period](../../celestial-mechanics.md#orbital-period), taking the satellite to the opposite end of the [elliptic orbit](../../celestial-mechanics.md#elliptic-orbit). By [Kepler's third law](../../mathematical-physics.md#kepler-s-third-law), relative to the original [geostationary orbit](../../celestial-mechanics.md#geostationary-orbit)'s [orbital period](../../celestial-mechanics.md#orbital-period) $T_0$,

$$
\frac{T_t}{T_0}=\left(\frac{a_t}{r_0}\right)^{3/2},\qquad
\boxed{t=\frac{T_0}{2}(1.1)^{3/2}\simeq13.8\ \mathrm h.}
$$

Using one [sidereal day](../../astrophysics.md#sidereal-day), $T_0=86164\ \mathrm s$, gives $t=4.9703\times10^4\ \mathrm s=13.806\ \mathrm h$; the usual $24\ \mathrm h$ approximation gives $13.844\ \mathrm h$. The arrival impulse changes the [velocity](../../classical-mechanics.md#velocity) into that of the new [circular Kepler orbit](../../celestial-mechanics.md#circular-kepler-orbit) without adding coast time in the impulsive model.

There is a real discrepancy between the wording and the diagram: an increase in altitude above [Earth](../../planetary-science.md#earth)'s surface is different from the radius increase drawn. If altitude is interpreted literally, let $R_E$ be [Earth](../../planetary-science.md#earth)'s radius. Then

$$
r_1=R_E+1.2(r_0-R_E),\qquad
\boxed{t=\frac{T_0}{2}\left(1.1-0.1\frac{R_E}{r_0}\right)^{3/2}\simeq13.5\ \mathrm h,}
$$

using $R_E\simeq6371\ \mathrm{km}$ and $r_0\simeq42164\ \mathrm{km}$. Thus $13.8\ \mathrm h$ answers the explicitly labelled geometry; $13.5\ \mathrm h$ answers the literal altitude wording.

<h3 id="section-a/a2">A2</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a2/solution">Solution</h4>

↑ **Parent:** [A2](#section-a/a2)

To find the [two-mass three-spring normal modes](../../wave-equation.md#two-mass-three-spring-normal-modes), choose both displacements positive to the right, measured from [mechanical equilibrium](../../thermodynamics.md#mechanical-equilibrium). The middle [spring](../../elasticity-physics.md#spring)'s extension changes by $x_2-x_1$. [Hooke's law](../../elasticity-physics.md#hooke-s-law) and [Newton's second law](../../force.md#newton-s-second-law) therefore give

$$
m_1\ddot x_1=-kx_1+k(x_2-x_1)=-2kx_1+kx_2,\qquad
m_2\ddot x_2=-kx_2-k(x_2-x_1)=kx_1-2kx_2.
$$

In a [normal mode](../../wave-equation.md#normal-mode) both displacements have the same [angular frequency](../../lagrangian-mechanics.md#angular-frequency): take $x_j=A_j\cos(\omega t+\phi)$. A nonzero amplitude [vector](../../vector-space.md#vector) exists when the [determinant](../../multilinear-algebra.md#determinant) vanishes:

$$
\begin{vmatrix}2k-m_1\omega^2&-k\\-k&2k-m_2\omega^2\end{vmatrix}=0,
\qquad m_1m_2\omega^4-2k(m_1+m_2)\omega^2+3k^2=0.
$$

Writing $D=\sqrt{m_1^2-m_1m_2+m_2^2}$, the two [angular frequencies](../../lagrangian-mechanics.md#angular-frequency) are

$$
\boxed{\omega_\pm=\sqrt{\frac{k}{m_1m_2}(m_1+m_2\pm D)}.}
$$

The corresponding [eigenvectors](../../linear-operator-theory.md#eigenvector) can be specified by

$$
\frac{A_2}{A_1}=\frac{2k-m_1\omega_\pm^2}{k}
=\frac{m_2-m_1\mp D}{m_2}.
$$

Since $D>|m_2-m_1|$ for positive masses, the lower [normal mode](../../wave-equation.md#normal-mode) $\omega_-$ has $A_2/A_1>0$: both bodies move in the same direction at any instant. The higher [normal mode](../../wave-equation.md#normal-mode) $\omega_+$ has $A_2/A_1<0$: they move in opposite directions. Their amplitudes are generally unequal. For the useful check $m_1=m_2=m$, these reduce to $\omega_-=\sqrt{k/m}$ with $A_2=A_1$, and $\omega_+=\sqrt{3k/m}$ with $A_2=-A_1$. Each [angular frequency](../../lagrangian-mechanics.md#angular-frequency) has units $\mathrm{rad\,s^{-1}}$.

<h3 id="section-a/a3">A3</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a3/solution">Solution</h4>

↑ **Parent:** [A3](#section-a/a3)

An [electron](../../physics.md#electron) has [electric charge](../../electric-charge.md) $-e$, so its gain of [kinetic energy](../../energy.md#kinetic-energy) through an accelerating [electric potential difference](../../electric-field.md#electric-potential-difference) of magnitude $V$ is $eV$. Starting from rest, [conservation of energy](../../mathematical-physics.md#conservation-of-energy) gives

$$
\frac12m_ev^2=eV,\qquad
v=\sqrt{\frac{2eV}{m_e}}.
$$

With $e=1.60218\times10^{-19}\ \mathrm C$, [electron mass](../../physics.md#electron-mass) $m_e=9.10938\times10^{-31}\ \mathrm{kg}$, and $V=150\ \mathrm V$,

$$
\boxed{v=7.26\times10^6\ \mathrm{m\,s^{-1}}.}
$$

This is a speed; the [velocity](../../classical-mechanics.md#velocity) points along the accelerating path, opposite the [electric field](../../electric-field.md). Here $v/c\simeq0.0242$, where $c$ is the [speed of light](../../special-relativity.md#speed-of-light), so the classical [kinetic energy](../../energy.md#kinetic-energy) approximation is accurate. As a check, [special relativity](../../special-relativity.md) gives $\gamma=1+eV/(m_ec^2)$ and $v=c\sqrt{1-\gamma^{-2}}\simeq7.262\times10^6\ \mathrm{m\,s^{-1}}$, agreeing to the quoted precision.

<h3 id="section-a/a4">A4</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a4/solution">Solution</h4>

↑ **Parent:** [A4](#section-a/a4)

The quoted [capacitance](../../electromagnetism.md#capacitance) is that of the filled [parallel-plate capacitor](../../electromagnetism.md#parallel-plate-capacitor), $C_i=1.0\times10^{-6}\ \mathrm F$. Disconnecting the source imposes [charge conservation](../../electric-charge.md#charge-conservation) on the isolated plates:

$$
Q=C_iV_i=(1.0\times10^{-6})(2500)=2.50\times10^{-3}\ \mathrm C.
$$

On removing the [dielectric](../../permittivity.md#dielectric), the [capacitance](../../electromagnetism.md#capacitance) falls by its [relative permittivity](../../quantum-mechanics.md#relative-permittivity), so $C_f=C_i/5=2.0\times10^{-7}\ \mathrm F$. The [capacitor energy](../../electromagnetism.md#capacitor-energy) at fixed [electric charge](../../electric-charge.md) is $U=Q^2/(2C)$. Therefore

$$
U_i=\frac12C_iV_i^2=3.125\ \mathrm J,\qquad
U_f=\frac{Q^2}{2C_f}=5U_i=15.625\ \mathrm J,
$$

and

$$
\boxed{\Delta U=U_f-U_i=+12.5\ \mathrm J.}
$$

The increase is supplied by the external [work](../../energy.md#work) needed to withdraw the [dielectric](../../permittivity.md#dielectric) against its attraction into the [electric field](../../electric-field.md), in the lossless quasistatic limit. The final [electric potential difference](../../electric-field.md#electric-potential-difference) is $Q/C_f=12500\ \mathrm V$, not the original charging value.

<h3 id="section-a/a5">A5</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a5/solution">Solution</h4>

↑ **Parent:** [A5](#section-a/a5)

For the propagating mode of an air-filled or evacuated [rectangular electromagnetic waveguide](../../electromagnetic-wave.md#rectangular-electromagnetic-waveguide), the longitudinal [dispersion relation](../../dispersion-relation.md) is

$$
\omega^2=c^2k_z^2+\omega_c^2.
$$

The [phase velocity](../../dispersion-relation.md#phase-velocity) and [group velocity](../../dispersion-relation.md#group-velocity) along the guide are consequently

$$
v_p=\frac{\omega}{k_z}=\frac{c}{\sqrt{1-(f_c/f)^2}},\qquad
v_g=\frac{d\omega}{dk_z}=c\sqrt{1-(f_c/f)^2}.
$$

With [waveguide cutoff frequency](../../electromagnetic-wave.md#waveguide-cutoff-frequency) $f_c=10\ \mathrm{GHz}$ and carrier [frequency](../../wave.md#frequency) $f=30\ \mathrm{GHz}$, $\sqrt{1-(f_c/f)^2}=\sqrt8/3$. Thus

$$
\boxed{v_p=\frac{3c}{\sqrt8}=3.18\times10^8\ \mathrm{m\,s^{-1}},\qquad
v_g=\frac{\sqrt8\,c}{3}=2.83\times10^8\ \mathrm{m\,s^{-1}}.}
$$

The pulse envelope travels at the [group velocity](../../dispersion-relation.md#group-velocity) for a sufficiently narrow range of [frequencies](../../wave.md#frequency). The [phase velocity](../../dispersion-relation.md#phase-velocity) exceeding the [speed of light](../../special-relativity.md#speed-of-light) does not describe superluminal signal transport. The check $v_pv_g=c^2$ follows directly from the [dispersion relation](../../dispersion-relation.md). A different uniform filling medium would require replacing $c$ by its electromagnetic propagation speed; the stated numerical answer uses the usual empty-guide assumption.

## Section B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="section-b/b6">B6</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b6/a">a</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/a/solution">Solution</h5>

↑ **Parent:** [A](#section-b/b6/a)

Use orthonormal basis [vectors](../../vector-space.md#vector) $\mathbf e_i(t)$ fixed in the [rotating reference frame](../../mathematical-physics.md#rotating-reference-frame), and expand the [angular momentum](../../momentum.md#angular-momentum) as $\mathbf J=\sum_iJ_i\mathbf e_i$. Over time $dt$, the basis undergoes infinitesimal [rotation](../../riemannian-geometry.md#rotation-mathematics) $\boldsymbol\Omega\,dt$, so

$$
\left(\frac{d\mathbf e_i}{dt}\right)_{S_0}=\boldsymbol\Omega\times\mathbf e_i.
$$

The [product rule](../../calculus.md#product-rule) gives the [rotating-frame derivative formula](../../mathematical-physics.md#rotating-frame-derivative-formula):

$$
\left(\frac{d\mathbf J}{dt}\right)_{S_0}
=\sum_i\dot J_i\mathbf e_i+\sum_iJ_i\boldsymbol\Omega\times\mathbf e_i
=\left(\frac{d\mathbf J}{dt}\right)_S+\boldsymbol\Omega\times\mathbf J.
$$

Since the applied [couple](../../momentum.md#couple-mechanics) is the rate of change of [angular momentum](../../momentum.md#angular-momentum) in the [inertial frame](../../mathematical-physics.md#inertial-frame),

$$
\boxed{\mathbf G=\left(\frac{d\mathbf J}{dt}\right)_S+\boldsymbol\Omega\times\mathbf J.}
$$

The second term accounts for the changing basis, even when the components of [angular momentum](../../momentum.md#angular-momentum) are constant in the [rotating reference frame](../../mathematical-physics.md#rotating-reference-frame).

<h4 id="section-b/b6/b">b</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/b/solution">Solution</h5>

↑ **Parent:** [B](#section-b/b6/b)

One application is the slow steady [precession](../../rigid-body-dynamics.md#precession) of a rapidly spinning [gyroscope](../../momentum.md#gyroscope) supported at one point. Let its [centre of mass](../../classical-mechanics.md#center-of-mass) be a distance $\ell$ from the pivot along its spin axis, at angle $\alpha$ to the upward vertical. Write $J\simeq I_1\omega$ for its dominant spin [angular momentum](../../momentum.md#angular-momentum). In a [reference frame](../../mathematical-physics.md#reference-frame) precessing steadily about the vertical with [angular velocity](../../rigid-body-dynamics.md#angular-velocity) $\boldsymbol\Omega_p$, the spin [angular momentum](../../momentum.md#angular-momentum) is approximately stationary, so

$$
\mathbf G\simeq\boldsymbol\Omega_p\times\mathbf J.
$$

The gravitational [torque](../../momentum.md#torque) has magnitude $mg\ell\sin\alpha$. The [cross product](../../vector-space.md#cross-product) on the right has magnitude $\Omega_pJ\sin\alpha$, giving, for a nonvertical axis,

$$
\boxed{\Omega_p\simeq\frac{mg\ell}{I_1\omega}.}
$$

Its direction follows from the [torque](../../momentum.md#torque) equation. This is the slow [precession](../../rigid-body-dynamics.md#precession) approximation: the additional [angular momentum](../../momentum.md#angular-momentum) associated with [precession](../../rigid-body-dynamics.md#precession) is small compared with the spin contribution.

<h4 id="section-b/b6/c">c</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/c/solution">Solution</h5>

↑ **Parent:** [C](#section-b/b6/c)

For this [gyrocompass](../../momentum.md#gyrocompass), let $\mathbf n,\mathbf w,\mathbf z$ be local north, west and upward unit [vectors](../../vector-space.md#vector), forming a right-handed basis. [Earth's rotation](../../planetary-science.md#earth-s-rotation) has local components

$$
\boldsymbol\Omega_E=\Omega_E\cos\lambda\,\mathbf n+\Omega_E\sin\lambda\,\mathbf z.
$$

Let the spin axis point along $\mathbf u=\cos\theta\,\mathbf n+\sin\theta\,\mathbf w$, and write its dominant [angular momentum](../../momentum.md#angular-momentum) as $J_s\mathbf u$, where $J_s=I_1\omega>0$. In [mechanical equilibrium](../../thermodynamics.md#mechanical-equilibrium) relative to [Earth](../../planetary-science.md#earth), this leading [angular momentum](../../momentum.md#angular-momentum) is fixed in the terrestrial [rotating reference frame](../../mathematical-physics.md#rotating-reference-frame). The bearings can exert horizontal [torques](../../momentum.md#torque) to keep the axle horizontal, but free rotation about the vertical implies $G_z=0$. The vertical component of the [rotating-frame derivative formula](../../mathematical-physics.md#rotating-frame-derivative-formula) therefore requires

$$
0=(\boldsymbol\Omega_E\times J_s\mathbf u)\cdot\mathbf z
=\Omega_EJ_s\cos\lambda\sin\theta.
$$

Away from either geographical pole, $\cos\lambda\ne0$, hence

$$
\boxed{\theta=0\ \text{or}\ \pi:\quad\text{the axle lies north--south}.}
$$

This is a necessary [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) condition; the next part distinguishes its stable and unstable spin orientations. The rapid-spin approximation neglects [angular momentum](../../momentum.md#angular-momentum) terms of order $I_2\Omega_E$ compared with $I_1\omega$. At either pole the horizontal component of [Earth's rotation](../../planetary-science.md#earth-s-rotation) vanishes, and this north-seeking mechanism gives no preferred horizontal direction. The paper explicitly excludes $90^\circ$; if latitude is signed, $-90^\circ$ must likewise be excluded.

<h4 id="section-b/b6/d">d</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/d/solution">Solution</h5>

↑ **Parent:** [D](#section-b/b6/d)

For the [gyrocompass oscillation](../../momentum.md#gyrocompass-oscillation), use the same local basis and define $\theta$ about the stable orientation, with spin [angular momentum](../../momentum.md#angular-momentum) directed north at $\theta=0$. Because the vertical is perpendicular to the horizontal axle, the extra vertical [angular momentum](../../momentum.md#angular-momentum) from the slow azimuthal motion is $I_2\dot\theta$. To leading order in [Earth](../../planetary-science.md#earth)'s small [angular velocity](../../rigid-body-dynamics.md#angular-velocity),

$$
\mathbf J\simeq J_s\mathbf u+I_2\dot\theta\,\mathbf z,\qquad J_s=I_1\omega.
$$

A constant vertical contribution $I_2\Omega_E\sin\lambda$ from [Earth's rotation](../../planetary-science.md#earth-s-rotation) has zero terrestrial time [derivative](../../calculus.md#derivative); the transverse terrestrial contributions affect the following equation only at order $\Omega_E^2$. Taking the vertical component of the [torque](../../momentum.md#torque) equation gives

$$
0=I_2\ddot\theta+J_s\Omega_E\cos\lambda\sin\theta.
$$

The terrestrial [derivative](../../calculus.md#derivative) of $J_s\mathbf u$ is horizontal, as is $\boldsymbol\Omega_E\times(I_2\dot\theta\mathbf z)$, so neither contributes to this component. Thus the small [angle](../../geometry-and-topology.md#angle) satisfies, using the [small-angle approximation](../../geometry-and-topology.md#small-angle-approximation) $\sin\theta\simeq\theta$,

$$
\ddot\theta+\frac{I_1}{I_2}\omega\Omega_E\cos\lambda\,\theta\simeq0,
\qquad
\boxed{\omega_{\rm shm}^2\simeq\frac{I_1}{I_2}\omega\Omega_E\cos\lambda.}
$$

This is [simple harmonic motion](../../classical-mechanics.md#simple-harmonic-motion), $\theta=A\cos(\omega_{\rm shm}t+\phi)$, with positive squared [angular frequency](../../lagrangian-mechanics.md#angular-frequency) away from the poles. The approximation requires rapid spin, small angular displacement and negligible bearing [friction](../../newtonian-mechanics.md#friction). Near the opposite orientation, putting $\theta=\pi+\delta$ instead yields $\ddot\delta-\omega_{\rm shm}^2\delta\simeq0$, which is unstable. Consequently, the paper's oscillation claim applies to the stable [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system), not both north--south spin directions. Without [damping](../../wave-equation.md#damping) the ideal [gyrocompass](../../momentum.md#gyrocompass) continues to oscillate rather than settling.

<h4 id="section-b/b6/e">e</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/e/solution">Solution</h5>

↑ **Parent:** [E](#section-b/b6/e)

For a thin [gyrocompass](../../momentum.md#gyrocompass) flywheel with rotational [symmetry](../../physics.md#symmetry-physics), the [perpendicular axis theorem](../../rigid-body-dynamics.md#perpendicular-axis-theorem) gives $I_1=I_x+I_y=2I_2$. This does not require the mass to be concentrated at the rim. Convert the specified spin to [angular velocity](../../rigid-body-dynamics.md#angular-velocity) and use one [sidereal day](../../astrophysics.md#sidereal-day) for [Earth's rotation](../../planetary-science.md#earth-s-rotation):

$$
\omega=5000\frac{2\pi}{60}=523.6\ \mathrm{rad\,s^{-1}},\qquad
\Omega_E=\frac{2\pi}{86164\ \mathrm s}=7.2921\times10^{-5}\ \mathrm{rad\,s^{-1}}.
$$

At the given latitude,

$$
\omega_{\rm shm}=\sqrt{2(523.6)(7.2921\times10^{-5})\cos52.2^\circ},\qquad
\boxed{\omega_{\rm shm}\simeq0.216\ \mathrm{rad\,s^{-1}}.}
$$

The associated [oscillation period](../../classical-mechanics.md#period-of-an-oscillation) is $T=2\pi/\omega_{\rm shm}\simeq29.0\ \mathrm s$. This uses the stated neglect of the support assembly's contribution to the [moment of inertia](../../rigid-body-dynamics.md#moment-of-inertia); a substantial additional vertical [moment of inertia](../../rigid-body-dynamics.md#moment-of-inertia) would lengthen the [oscillation period](../../classical-mechanics.md#period-of-an-oscillation).

<h3 id="section-b/b7">B7</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b7/a">a</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/a/solution">Solution</h5>

↑ **Parent:** [A](#section-b/b7/a)

The [bending moment](../../elasticity-physics.md#bending-moment) $B(x)$ is the internal [torque](../../momentum.md#torque) transmitted across a cut through an [elastic beam](../../elasticity-physics.md#elastic-beam), about the transverse bending axis. It balances the moments of the external [forces](../../force.md) on the isolated portion on one side of the cut. Its sign depends on the chosen convention, and its units are $\mathrm{N\,m}$.

The relevant “moment of area” is the [second moment of area](../../elasticity-physics.md#second-moment-of-area) of the cross-section about its [neutral axis](../../elasticity-physics.md#neutral-axis):

$$
\boxed{I=\int_A z^2\,dA,}
$$

where $z$ is perpendicular distance from that axis within the section. It has units $\mathrm{m^4}$ and is a geometrical quantity, unlike a mass [moment of inertia](../../rigid-body-dynamics.md#moment-of-inertia). For a homogeneous beam under pure bending, the [neutral axis](../../elasticity-physics.md#neutral-axis) passes through the section's [centroid](../../euclidean-geometry.md#centroid), and its longitudinal [strain](../../continuum-mechanics.md#strain) is zero.

<h4 id="section-b/b7/b">b</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/b/solution">Solution</h5>

↑ **Parent:** [B](#section-b/b7/b)

Assume a slender homogeneous [elastic beam](../../elasticity-physics.md#elastic-beam) obeying [linear elasticity](../../elasticity-physics.md#linear-elasticity), with plane sections remaining plane and no resultant longitudinal [force](../../force.md). A length element of its [neutral axis](../../elasticity-physics.md#neutral-axis) subtending a small [angle](../../geometry-and-topology.md#angle) $d\phi$ has length $R\,d\phi$. A neighbouring fibre at distance $z$ from that axis has a length change of magnitude $z\,d\phi$, giving longitudinal [strain](../../continuum-mechanics.md#strain) $\varepsilon=z/R$ with signs chosen consistently for tensile and compressed fibres. By [Hooke's law](../../elasticity-physics.md#hooke-s-law), its longitudinal [stress](../../continuum-mechanics.md#stress) is $\sigma=E\varepsilon=Ez/R$.

The [torque](../../momentum.md#torque) of these longitudinal [forces](../../force.md) about the [neutral axis](../../elasticity-physics.md#neutral-axis) is therefore

$$
B=\int_A z\sigma\,dA=\frac E R\int_Az^2\,dA=\frac{EI}{R},
\qquad
\boxed{R=\frac{EI}{B}.}
$$

Here $E$ is [Young's modulus](../../elasticity-physics.md#young-s-modulus) and $I$ the [second moment of area](../../elasticity-physics.md#second-moment-of-area). The displayed relation uses a signed radius and [bending moment](../../elasticity-physics.md#bending-moment); an unsigned geometrical radius is $|R|=EI/|B|$. For consistency with the negative [bending moments](../../elasticity-physics.md#bending-moment) in the later parts, take the deflection $y$ positive downward and the signed [curvature](../../differential-geometry.md#curvature) as $1/R\simeq y''$. Then the small-slope [Euler-Bernoulli beam equation](../../elasticity-physics.md#euler-bernoulli-beam-equation) reads $EIy''=B$. Reversing the vertical coordinate reverses the corresponding sign relation but leaves the physical deflection unchanged.

<h4 id="section-b/b7/c">c</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/c/solution">Solution</h5>

↑ **Parent:** [C](#section-b/b7/c)

By vertical [force](../../force.md) balance and reflection [symmetry](../../physics.md#symmetry-physics), each support exerts an upward [force](../../force.md) $W/2$. Use the paper's convention in which the sagging [bending moment](../../elasticity-physics.md#bending-moment) is negative. For a cut at $0<x<L/2$, the left support's moment about that cut gives

$$
B(x)=-\frac W2x.
$$

For $L/2<x<L$, include the central downward [force](../../force.md) when taking moments of all loads to the left:

$$
B(x)=-\frac W2x+W\left(x-\frac L2\right)=-\frac W2(L-x).
$$

Thus

$$
\boxed{B(x)=\begin{cases}-Wx/2,&0<x<L/2,\\-W(L-x)/2,&L/2<x<L.\end{cases}}
$$

The [bending moment](../../elasticity-physics.md#bending-moment) is continuous at the load, with $B(L/2)=-WL/4$, and vanishes at both freely rotating supports. The jump is in its first [derivative](../../calculus.md#derivative), reflecting the concentrated transverse [force](../../force.md).

<h4 id="section-b/b7/d">d</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/d/solution">Solution</h5>

↑ **Parent:** [D](#section-b/b7/d)

The uniform weight per unit length is $q=\rho abg$, where $\rho$ is the [mass density](../../fluid-mechanics.md#density) and $g$ the [gravitational acceleration](../../newton-s-law-of-universal-gravitation.md#gravitational-acceleration). The total weight is $qL$, so each support provides an upward [force](../../force.md) $qL/2$. The weight on the portion from $0$ to $x$ is $qx$ acting at that portion's midpoint, a distance $x/2$ from the cut. In the same [bending moment](../../elasticity-physics.md#bending-moment) convention as part (c),

$$
B(x)=-\frac{qL}{2}x+(qx)\frac x2,
\qquad
\boxed{B(x)=-\frac12\rho abg\,x(L-x).}
$$

The units are $(\mathrm{N\,m^{-1}})\mathrm{m^2}=\mathrm{N\,m}$. Its greatest magnitude occurs at $x=L/2$, where $B=-qL^2/8$.

<h4 id="section-b/b7/e">e</h4>

↑ **Parent:** [B7](#section-b/b7)

<h5 id="section-b/b7/e/solution">Solution</h5>

↑ **Parent:** [E](#section-b/b7/e)

Take downward deflection $y(x)$ positive, with the support level $y=0$. The [rectangular section second moment of area](../../elasticity-physics.md#rectangular-section-second-moment-of-area) about the horizontal [neutral axis](../../elasticity-physics.md#neutral-axis) is

$$
I=a\int_{-b/2}^{b/2}z^2\,dz=\frac{ab^3}{12}.
$$

For small slopes the [curvature](../../differential-geometry.md#curvature) relation from part (b), with the stated sign convention, is

$$
EIy''=-\frac q2x(L-x).
$$

Integrating twice gives

$$
EIy'=-\frac{qLx^2}{4}+\frac{qx^3}{6}+C_1,\qquad
EIy=-\frac{qLx^3}{12}+\frac{qx^4}{24}+C_1x+C_2.
$$

The support [boundary conditions](../../differential-equation.md#boundary-condition) $y(0)=y(L)=0$ give $C_2=0$ and $C_1=qL^3/24$. Hence

$$
\boxed{y(x)=\frac{q}{24EI}\left(x^4-2Lx^3+L^3x\right)
=\frac{\rho g}{2Eb^2}\left(x^4-2Lx^3+L^3x\right),\quad0\le x\le L.}
$$

This is a downward displacement; its upward component is $-y(x)$. As checks, reflection [symmetry](../../physics.md#symmetry-physics) gives $y'(L/2)=0$, and the maximum downward deflection is

$$
\boxed{y_{\max}=y(L/2)=\frac{5qL^4}{384EI}=\frac{5\rho gL^4}{32Eb^2}.}
$$

The units are length: $\rho g/(Eb^2)$ has units $\mathrm{m^{-3}}$. The width $a$ cancels because both weight and bending resistance scale with it. The small-slope approximation requires $\rho gL^3/(Eb^2)\ll1$; [shear strain](../../continuum-mechanics.md#shear-strain) is also neglected, as appropriate for a slender [elastic beam](../../elasticity-physics.md#elastic-beam).

<a id="section-b/b7/e/image-calculated-deflection-of-a-simply-supported-beam-under-its-own-weight-downward-displacement-is-positive"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-1-b7-self-weight-deflection.png)

**[Figure 1](#section-b/b7/e/image-calculated-deflection-of-a-simply-supported-beam-under-its-own-weight-downward-displacement-is-positive). Calculated deflection of a simply supported beam under its own weight; downward displacement is positive**.

## Section C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="section-c/c8">C8</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c8/a">a</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/a/solution">Solution</h5>

↑ **Parent:** [A](#section-c/c8/a)

The [Poynting vector](../../electromagnetic-wave.md#poynting-vector) is the local [electromagnetic energy](../../electromagnetic-wave.md#electromagnetic-energy) flux density:

$$
\boxed{\mathbf N=\mathbf E\times\mathbf H.}
$$

Here $\mathbf E$ is the [electric field](../../electric-field.md) and $\mathbf H$ the [magnetic field intensity](../../electromagnetism.md#magnetic-field-intensity). For an oriented area element $d\mathbf S$, $\mathbf N\cdot d\mathbf S$ is the electromagnetic [power](../../energy.md#power) crossing that element in its positive normal direction. Thus $\int_S\mathbf N\cdot d\mathbf S$ is outward [power](../../energy.md#power) through a closed [surface](../../topological-surface.md), in watts. The [Poynting vector](../../electromagnetic-wave.md#poynting-vector) has units $\mathrm{W\,m^{-2}}$, and its direction describes local [electromagnetic energy](../../electromagnetic-wave.md#electromagnetic-energy) transport.

<h4 id="section-c/c8/b">b</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/b/solution">Solution</h5>

↑ **Parent:** [B](#section-c/c8/b)

The unit [relative permittivity](../../quantum-mechanics.md#relative-permittivity) and vacuum-valued [magnetic permeability](../../maxwell-equations.md#permeability-electromagnetism) imply $\mathbf D=\epsilon_0\mathbf E$ and $\mathbf B=\mu_0\mathbf H$. The [electromagnetic energy](../../electromagnetic-wave.md#electromagnetic-energy) per unit volume is

$$
\boxed{U=\frac12\epsilon_0\mathbf E\cdot\mathbf E+\frac12\mu_0\mathbf H\cdot\mathbf H,\qquad[U]=\mathrm{J\,m^{-3}}.}
$$

The two contributions are the stored electric and magnetic [energies](../../energy.md). Although called $U$ in this paper, this quantity is an [energy density](../../statistical-physics.md#energy-density); the total [electromagnetic energy](../../electromagnetic-wave.md#electromagnetic-energy) is $\int_VU\,dV$.

<h4 id="section-c/c8/c">c</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/c/solution">Solution</h5>

↑ **Parent:** [C](#section-c/c8/c)

Use the [divergence](../../multivariable-calculus.md#divergence) identity for a [cross product](../../vector-space.md#cross-product), followed by [Faraday's law of induction](../../maxwell-equations.md#faraday-s-law-of-induction) and the [Ampère-Maxwell equation](../../maxwell-equations.md#ampere-s-circuital-law):

$$
\nabla\cdot(\mathbf E\times\mathbf H)
=\mathbf H\cdot(\nabla\times\mathbf E)-\mathbf E\cdot(\nabla\times\mathbf H),
$$



$$
\nabla\times\mathbf E=-\mu_0\frac{\partial\mathbf H}{\partial t},\qquad
\nabla\times\mathbf H=\mathbf J+\epsilon_0\frac{\partial\mathbf E}{\partial t}.
$$

With the [electromagnetic energy](../../electromagnetic-wave.md#electromagnetic-energy) density of part (b), these give

$$
\nabla\cdot\mathbf N
=-\mathbf E\cdot\mathbf J-\mu_0\mathbf H\cdot\partial_t\mathbf H-\epsilon_0\mathbf E\cdot\partial_t\mathbf E
=-\mathbf E\cdot\mathbf J-\frac{\partial U}{\partial t}.
$$

Integrate over a fixed volume $V$ and apply the [divergence theorem](../../multivariable-calculus.md#divergence-theorem), choosing $d\mathbf S$ outward:

$$
\boxed{\oint_S\mathbf N\cdot d\mathbf S
=-\int_V\mathbf E\cdot\mathbf J\,dV-\frac d{dt}\int_VU\,dV.}
$$

This is [Poynting's theorem](../../electromagnetic-wave.md#poynting-theorem). The outward [electromagnetic energy](../../electromagnetic-wave.md#electromagnetic-energy) flux equals minus the [power](../../energy.md#power) transferred to matter and minus the rate at which [electromagnetic energy](../../electromagnetic-wave.md#electromagnetic-energy) accumulates inside. For the dissipative [electrical conductor](../../electric-charge.md#electrical-conductor) in this question, the matter term is [Ohmic heating](../../electric-charge.md#joule-heating).

<h4 id="section-c/c8/d">d</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/d/solution">Solution</h5>

↑ **Parent:** [D](#section-c/c8/d)

Take the [electric current](../../electric-charge.md#electric-current) along $+z$, and use [cylindrical coordinates](../../multivariable-calculus.md#cylindrical-coordinate-system). A [uniform current in a straight homogeneous wire](../../electric-charge.md#uniform-current-in-a-straight-homogeneous-wire) has

$$
\mathbf J=\frac I{\pi a^2}\widehat{\mathbf z}.
$$

The local [Ohm's law](../../electric-charge.md#ohm-s-law) $\mathbf J=\sigma\mathbf E$ gives the longitudinal [electric field](../../electric-field.md)

$$
\mathbf E=\frac I{\sigma\pi a^2}\widehat{\mathbf z}.
$$

For a circular [Amperian loop](../../maxwell-equations.md#amperian-loop) of radius $r\le a$, the enclosed [electric current](../../electric-charge.md#electric-current) is $I_{\rm enc}=Ir^2/a^2$. The [magnetostatic Ampère law](../../maxwell-equations.md#magnetostatic-ampere-law) gives $2\pi rH_\phi=I_{\rm enc}$, hence

$$
\mathbf H=\frac{Ir}{2\pi a^2}\widehat{\boldsymbol\phi}.
$$

Since $\widehat{\mathbf z}\times\widehat{\boldsymbol\phi}=-\widehat{\mathbf r}$, the [Poynting vector](../../electromagnetic-wave.md#poynting-vector) is

$$
\boxed{\mathbf N(r)=-\frac{I^2r}{2\sigma\pi^2a^4}\widehat{\mathbf r},\qquad0\le r\le a.}
$$

It is zero at the centre and points radially inward elsewhere. Its units are $\mathrm{W\,m^{-2}}$. These are the interior fields in the long-wire approximation, neglecting end and contact effects.

<h4 id="section-c/c8/e">e</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/e/solution">Solution</h5>

↑ **Parent:** [E](#section-c/c8/e)

The [Ohmic heating](../../electric-charge.md#joule-heating) per unit volume is $\mathbf E\cdot\mathbf J=J^2/\sigma$, uniform in this wire. Multiplying by its volume gives the dissipated [power](../../energy.md#power)

$$
\boxed{P_{\rm loss}=\frac1\sigma\left(\frac I{\pi a^2}\right)^2\pi a^2L
=\frac{I^2L}{\sigma\pi a^2}=I^2R_{\rm wire},}
$$

where the [electrical resistance](../../electric-charge.md#electrical-resistance) is $R_{\rm wire}=L/(\sigma\pi a^2)$. The result is in watts; over a time interval $\Delta t$ the dissipated [energy](../../energy.md) is $P_{\rm loss}\Delta t$.

<h4 id="section-c/c8/f">f</h4>

↑ **Parent:** [C8](#section-c/c8)

<h5 id="section-c/c8/f/solution">Solution</h5>

↑ **Parent:** [F](#section-c/c8/f)

On the curved wire [surface](../../topological-surface.md), the outward normal is $\widehat{\mathbf r}$ and the [Poynting vector](../../electromagnetic-wave.md#poynting-vector) has the constant radial value $N_r(a)=-I^2/(2\sigma\pi^2a^3)$. Its outward [flux](../../mathematical-physics.md#flux) is

$$
\Phi_N=\int_{\rm curved}\mathbf N\cdot d\mathbf S
=N_r(a)(2\pi aL)
=\boxed{-\frac{I^2L}{\sigma\pi a^2}=-P_{\rm loss}.}
$$

The [Poynting vector](../../electromagnetic-wave.md#poynting-vector) is radial, so it has zero normal component on the two end faces in this approximation. This is therefore also the outward [flux](../../mathematical-physics.md#flux) through the complete wire [surface](../../topological-surface.md). Equivalently, positive electromagnetic [power](../../energy.md#power) $P_{\rm loss}$ flows inward.

The fields are steady, so the stored [electromagnetic energy](../../electromagnetic-wave.md#electromagnetic-energy) does not change. [Poynting's theorem](../../electromagnetic-wave.md#poynting-theorem) consequently requires the incoming [power](../../energy.md#power) to equal the [Ohmic heating](../../electric-charge.md#joule-heating) in part (e), exactly as found. The energy reaches the wire through the surrounding [electromagnetic field](../../electromagnetism.md#electromagnetic-field). A local check is $\nabla\cdot\mathbf N=r^{-1}\partial_r(rN_r)=-I^2/(\sigma\pi^2a^4)=-\mathbf E\cdot\mathbf J$.

<h3 id="section-c/c9">C9</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c9/a">a</h4>

↑ **Parent:** [C9](#section-c/c9)

<h5 id="section-c/c9/a/solution">Solution</h5>

↑ **Parent:** [A](#section-c/c9/a)

Let the unit normal $\mathbf n$ point from material 1 to material 2, and let their relative [magnetic permeabilities](../../maxwell-equations.md#permeability-electromagnetism) be $\mu_1,\mu_2$, so $\mathbf B_i=\mu_0\mu_i\mathbf H_i$ for linear isotropic media. Apply [Gauss's law for magnetism](../../maxwell-equations.md#gauss-s-law-for-magnetism) to an infinitesimal [Gaussian pillbox](../../maxwell-equations.md#gaussian-pillbox) straddling the interface. The side contribution vanishes as its height tends to zero, leaving

$$
\boxed{\mathbf n\cdot(\mathbf B_2-\mathbf B_1)=0.}
$$

The normal [magnetic flux density](../../magnetic-field.md) is continuous.

Next use a narrow rectangular [Amperian loop](../../maxwell-equations.md#amperian-loop) crossing the interface. The two short-side contributions vanish in the zero-height limit. The [magnetostatic Ampère law](../../maxwell-equations.md#magnetostatic-ampere-law) for [magnetic field intensity](../../electromagnetism.md#magnetic-field-intensity) gives

$$
\boxed{\mathbf n\times(\mathbf H_2-\mathbf H_1)=\mathbf K_f,}
$$

where $\mathbf K_f$ is any free [surface current density](../../electric-charge.md#surface-current-density). Thus, if there is no free [surface current density](../../electric-charge.md#surface-current-density) on the interface, the tangential [magnetic field intensity](../../electromagnetism.md#magnetic-field-intensity) is continuous. In that case the component relations are

$$
\boxed{B_{1n}=B_{2n},\qquad H_{1t}=H_{2t},\qquad
\mu_1H_{1n}=\mu_2H_{2n},\qquad
\frac{B_{1t}}{\mu_1}=\frac{B_{2t}}{\mu_2}.}
$$

The distinction between free and bound [electric currents](../../electric-charge.md#electric-current) matters: bound currents due to [magnetization](../../electromagnetism.md#magnetization) are already incorporated in the definition of [magnetic field intensity](../../electromagnetism.md#magnetic-field-intensity). A change of [magnetic permeability](../../maxwell-equations.md#permeability-electromagnetism) alone does not make the tangential [magnetic flux density](../../magnetic-field.md) continuous.

<h4 id="section-c/c9/b">b</h4>

↑ **Parent:** [C9](#section-c/c9)

<h5 id="section-c/c9/b/solution">Solution</h5>

↑ **Parent:** [B](#section-c/c9/b)

The starting point is [Gauss's law for magnetism](../../maxwell-equations.md#gauss-s-law-for-magnetism), $\nabla\cdot\mathbf B=0$: a [flux tube](../../magnetic-field.md#flux-tube) carries the same [magnetic flux](../../magnetic-field.md#magnetic-flux) through successive transverse sections. To identify that tube approximately with the physical core, one must also make a negligible-leakage approximation. The large core [magnetic permeability](../../maxwell-equations.md#permeability-electromagnetism) makes the core route much less reluctant than competing paths through the surrounding air; the small gap further reduces the incentive for a long external return path. The gentle taper, $s\gg R-r$, lets the field follow the changing section with only small transverse corrections.

For two cuts and the intervening lateral [surface](../../topological-surface.md), the [divergence theorem](../../multivariable-calculus.md#divergence-theorem) gives $\Phi_2-\Phi_1=-\Phi_{\rm side}$. Neglecting lateral leakage gives

$$
\boxed{\Phi\simeq B(x)A(x)\simeq\text{constant}.}
$$

The normal [magnetic flux density](../../magnetic-field.md) is continuous at each core–air interface by part (a), so this same [magnetic flux](../../magnetic-field.md#magnetic-flux) crosses the gap. To use the gap's geometrical area $\pi r^2$ in the later formulas, the [magnetic fringing](../../electromagnetism.md#magnetic-fringing) must also be negligible, normally requiring $h\ll r$. This is the small-gap interpretation of the paper's approximation. Large [magnetic permeability](../../maxwell-equations.md#permeability-electromagnetism) alone does not eliminate leakage or [magnetic fringing](../../electromagnetism.md#magnetic-fringing) for arbitrary gap geometry.

<h4 id="section-c/c9/c">c</h4>

↑ **Parent:** [C9](#section-c/c9)

<h5 id="section-c/c9/c/solution">Solution</h5>

↑ **Parent:** [C](#section-c/c9/c)

For the closed untapered torus, apply the [magnetostatic Ampère law](../../maxwell-equations.md#magnetostatic-ampere-law) to a circular path through the core. It links all $N$ turns, each carrying [electric current](../../electric-charge.md#electric-current) $I$:

$$
\oint\mathbf H\cdot d\mathbf l=NI.
$$

Since $L\gg R$, variation of the path length and of the tangential [magnetic field intensity](../../electromagnetism.md#magnetic-field-intensity) across the section is negligible. Thus $H_{\rm in}L\simeq NI$, giving, within this thin-torus approximation,

$$
\boxed{H_{\rm in}=\frac{NI}{L}.}
$$

The units are $\mathrm{A\,m^{-1}}$. The core [magnetic flux density](../../magnetic-field.md) is $B_{\rm in}=\mu_0\mu NI/L$ in the linear material model.

<h4 id="section-c/c9/d">d</h4>

↑ **Parent:** [C9](#section-c/c9)

<h5 id="section-c/c9/d/solution">Solution</h5>

↑ **Parent:** [D](#section-c/c9/d)

With uniform section and negligible [magnetic fringing](../../electromagnetism.md#magnetic-fringing), constant [magnetic flux](../../magnetic-field.md#magnetic-flux) gives equal [magnetic flux densities](../../magnetic-field.md) in the core and gap:

$$
\mu_0\mu H_{\rm in}=\mu_0H_{\rm gap},\qquad H_{\rm in}=H_{\rm gap}/\mu.
$$

Here $L$ is the core arc length and $h$ the additional gap length. Applying the [magnetostatic Ampère law](../../maxwell-equations.md#magnetostatic-ampere-law) around the complete [magnetic circuit](../../electromagnetism.md#magnetic-circuit),

$$
H_{\rm in}L+H_{\rm gap}h=NI,
\qquad
H_{\rm gap}\left(\frac L\mu+h\right)=NI.
$$

Consequently,

$$
\boxed{H_{\rm gap}=\frac{\mu NI}{\mu h+L}.}
$$

This tends to $NI/h$ when the gap dominates the [magnetic reluctance](../../electromagnetism.md#magnetic-reluctance), $\mu h\gg L$, and reduces to the no-gap result as $h\to0$. The gap [magnetic flux density](../../magnetic-field.md) is $B_{\rm gap}=\mu_0H_{\rm gap}$.

<h4 id="section-c/c9/e">e</h4>

↑ **Parent:** [C9](#section-c/c9)

<h5 id="section-c/c9/e/solution">Solution</h5>

↑ **Parent:** [E](#section-c/c9/e)

Let the approximately conserved [magnetic flux](../../magnetic-field.md#magnetic-flux) be $\Phi$. Then

$$
\Phi=\mu_0H_{\rm gap}\pi r^2.
$$

The length $L$ shown in the original diagram is the untapered core arc; the two tapers are separate lengths $s$ each. In the untapered core, [flux](../../mathematical-physics.md#flux) conservation gives

$$
H_R=\frac{\Phi}{\mu_0\mu\pi R^2}
=\frac{H_{\rm gap}}\mu\frac{r^2}{R^2}.
$$

For one taper use distance $u$ from its narrow end. The straight taper in the diagram has local radius

$$
a(u)=r+\frac{R-r}{s}u,\qquad0\le u\le s,
$$

and [magnetic field intensity](../../electromagnetism.md#magnetic-field-intensity)

$$
H(u)=\frac{\Phi}{\mu_0\mu\pi a(u)^2}
=\frac{H_{\rm gap}}\mu\frac{r^2}{a(u)^2}.
$$

Its contribution to the [line integral](../../multivariable-calculus.md#line-integral) in the [magnetostatic Ampère law](../../maxwell-equations.md#magnetostatic-ampere-law) is found explicitly:

$$
\int_0^s\frac{du}{a(u)^2}
=\frac{s}{R-r}\left(\frac1r-\frac1R\right)=\frac{s}{rR},
\qquad
\int_0^sH(u)\,du=\frac{H_{\rm gap}}\mu\frac{sr}{R}.
$$

Adding the gap, the untapered arc and both tapers gives

$$
NI=H_{\rm gap}h+\frac{H_{\rm gap}}\mu\frac{r^2}{R^2}L
+2\frac{H_{\rm gap}}\mu\frac{sr}{R}.
$$

Therefore

$$
\boxed{H_{\rm gap}=\frac{\mu NI}{\mu h+L(r/R)^2+2s(r/R)}.}
$$

This uses a linear radius profile, approximately uniform [magnetic flux density](../../magnetic-field.md) over each section, a linear constant [magnetic permeability](../../maxwell-equations.md#permeability-electromagnetism), and negligible leakage and [magnetic fringing](../../electromagnetism.md#magnetic-fringing). For a non-linear taper profile $a(u)$ the honest generalization is

$$
H_{\rm gap}=\frac{\mu NI}{\mu h+Lr^2/R^2+2r^2\int_0^sdu/a(u)^2}.
$$

Thus an arbitrary smooth taper with the same end radii and length need not give the printed formula; the straight-sided geometry supplies the additional information.

<h4 id="section-c/c9/f">f</h4>

↑ **Parent:** [C9](#section-c/c9)

<h5 id="section-c/c9/f/solution">Solution</h5>

↑ **Parent:** [F](#section-c/c9/f)

Set $\alpha=r/R<1$. Comparing with the untapered expression in part (d), using the same $N,I,\mu,h,L$ and large radius $R$,

$$
\frac{H_{\rm gap,taper}}{H_{\rm gap,untaper}}
=\frac{\mu h+L}{\mu h+L\alpha^2+2s\alpha}.
$$

The stated limit $s/L\ll\alpha$ makes $2s\alpha\ll L\alpha^2$, so

$$
\boxed{\frac{H_{\rm gap,taper}}{H_{\rm gap,untaper}}\simeq
\frac{\mu h+L}{\mu h+L\alpha^2}>1.}
$$

The taper concentrates [magnetic flux](../../magnetic-field.md#magnetic-flux) into a smaller pole-face area, increasing the gap [magnetic field intensity](../../electromagnetism.md#magnetic-field-intensity) and [magnetic flux density](../../magnetic-field.md) for the same winding [electric current](../../electric-charge.md#electric-current). If $\mu h\ll L\alpha^2$, the enhancement approaches $1/\alpha^2=(R/r)^2$. If instead $\mu h\gg L$, the gap dominates the [magnetic reluctance](../../electromagnetism.md#magnetic-reluctance) and the enhancement approaches unity: both fields approach $NI/h$.

The benefit is therefore strongest when the untapered core's contribution is significant, while the taper lengths contribute little. The same-core-length convention is the comparison defined by parts (d) and (e); if one instead fixes the full iron path length, the untapered comparator has length $L+2s$, a difference negligible in the stated limit. A smaller gap area can increase the field even though the total [magnetic flux](../../magnetic-field.md#magnetic-flux) need not increase. [Magnetic saturation](../../electromagnetism.md#magnetic-saturation) and [magnetic fringing](../../electromagnetism.md#magnetic-fringing), excluded from this model, limit the ideal concentration.

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
