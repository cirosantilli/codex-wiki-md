# Rigid body dynamics

↑ **Parent:** [Classical mechanics](classical-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rigid_body_dynamics)

Rigid body dynamics studies translation and rotation of bodies whose internal distances are fixed.

**Table of contents**

- [Bell-clapper loss of contact](#bell-clapper-loss-of-contact)
- [Major-axis relaxation theorem](#major-axis-relaxation-theorem)
- [Centre of percussion](#centre-of-percussion)
  - [Hinge impulse of an edge-pivoted square plate](#hinge-impulse-of-an-edge-pivoted-square-plate)
- [Rotational equation of motion](#rotational-equation-of-motion)
- [Constant-power rotational acceleration](#constant-power-rotational-acceleration)
- [Vehicle rollover threshold](#vehicle-rollover-threshold)
- [Two hinged rods with both ends sliding on a floor](#two-hinged-rods-with-both-ends-sliding-on-a-floor)
- [Endpoint collision of two freely rotating equal rods](#endpoint-collision-of-two-freely-rotating-equal-rods)
- [Two hinged rods sliding on a floor](#two-hinged-rods-sliding-on-a-floor)
- [Solid-body rotation](#solid-body-rotation)
- [Symmetric top](#symmetric-top)
  - [Prolate symmetric top](#prolate-symmetric-top)
  - [Oblate symmetric top](#oblate-symmetric-top)
  - [Torque-free precession of a symmetric top](#torque-free-precession-of-a-symmetric-top)
    - [Body-frame and space-frame frequencies of free symmetric-top precession](#body-frame-and-space-frame-frequencies-of-free-symmetric-top-precession)
  - [Heavy symmetric top](#heavy-symmetric-top)
    - [Symmetry-axis equation of a heavy symmetric top](#symmetry-axis-equation-of-a-heavy-symmetric-top)
    - [Nutation](#nutation)
    - [Uniform precession of a heavy symmetric top](#uniform-precession-of-a-heavy-symmetric-top)
      - [Slow and fast steady precession](#slow-and-fast-steady-precession)
- [Precession](#precession)
  - [Precession period](#precession-period)
- [Angular velocity](#angular-velocity)
  - [Angular acceleration](#angular-acceleration)
  - [Angular speed](#angular-speed)
- [Fixed space frame](#fixed-space-frame)
- [Principal body frame](#principal-body-frame)
  - [Principal axis](#principal-axis)
  - [Derivative of a body-fixed basis vector](#derivative-of-a-body-fixed-basis-vector)
  - [Body-frame derivative of a space-fixed vector](#body-frame-derivative-of-a-space-fixed-vector)
- [Euler's equations (rigid body dynamics)](#euler-s-equations-rigid-body-dynamics)
  - [Euler equations for a torque-free rigid body](#euler-equations-for-a-torque-free-rigid-body)
    - [Torque-free rigid-body invariants](#torque-free-rigid-body-invariants)
      - [Quartic equation for one component of torque-free angular velocity](#quartic-equation-for-one-component-of-torque-free-angular-velocity)
    - [Coplanarity in a torque-free axisymmetric rigid body](#coplanarity-in-a-torque-free-axisymmetric-rigid-body)
    - [Intermediate axis theorem](#intermediate-axis-theorem)
      - [Fixed-angular-momentum energy test for principal-axis rotation](#fixed-angular-momentum-energy-test-for-principal-axis-rotation)
      - [Normalized intermediate-axis model](#normalized-intermediate-axis-model)
      - [Torque-free tumbling](#torque-free-tumbling)
      - [Spinning-book demonstration](#spinning-book-demonstration)
      - [Linear stability of principal-axis rotation](#linear-stability-of-principal-axis-rotation)
      - [Intermediate-axis separatrix](#intermediate-axis-separatrix)
- [Moment of inertia](#moment-of-inertia)
  - [Density-power cylindrical moment of inertia](#density-power-cylindrical-moment-of-inertia)
  - [Axial moment of inertia of a hollow cylinder](#axial-moment-of-inertia-of-a-hollow-cylinder)
  - [Axial moment of inertia of a solid of revolution](#axial-moment-of-inertia-of-a-solid-of-revolution)
  - [Moment-of-inertia triangle inequalities](#moment-of-inertia-triangle-inequalities)
  - [Moment of inertia of a uniform square plate](#moment-of-inertia-of-a-uniform-square-plate)
    - [Off-axis angular momentum of a square lamina](#off-axis-angular-momentum-of-a-square-lamina)
    - [In-plane inertia isotropy of a square plate](#in-plane-inertia-isotropy-of-a-square-plate)
  - [Moment of inertia of a uniform solid hemisphere](#moment-of-inertia-of-a-uniform-solid-hemisphere)
  - [Moment of inertia of a uniform solid cylinder](#moment-of-inertia-of-a-uniform-solid-cylinder)
  - [Reflected inertia of a no-slip wheel and roller](#reflected-inertia-of-a-no-slip-wheel-and-roller)
  - [Moment of inertia of a uniform annulus](#moment-of-inertia-of-a-uniform-annulus)
  - [Moment of inertia of a uniform disc](#moment-of-inertia-of-a-uniform-disc)
  - [Moment of inertia of a uniform solid sphere](#moment-of-inertia-of-a-uniform-solid-sphere)
  - [Mass second-moment tensor](#mass-second-moment-tensor)
  - [Inertia tensor](#inertia-tensor)
    - [Inertia tensor of a uniform cube](#inertia-tensor-of-a-uniform-cube)
    - [Inertia tensor of a displaced uniform ball](#inertia-tensor-of-a-displaced-uniform-ball)
    - [Positive second-moment matrix test for an inertia tensor](#positive-second-moment-matrix-test-for-an-inertia-tensor)
    - [Inertia tensor of a sheared rectangular lamina](#inertia-tensor-of-a-sheared-rectangular-lamina)
    - [Inertia tensor of paired point masses](#inertia-tensor-of-paired-point-masses)
    - [Rotational inertia measurement with a falling mass](#rotational-inertia-measurement-with-a-falling-mass)
      - [Rotary encoder](#rotary-encoder)
    - [Tensor parallel-axis theorem](#tensor-parallel-axis-theorem)
    - [Principal moment of inertia](#principal-moment-of-inertia)
      - [Rotational energy ellipsoid](#rotational-energy-ellipsoid)
      - [Degeneracy of principal moments of inertia](#degeneracy-of-principal-moments-of-inertia)
    - [Poinsot's ellipsoid](#poinsot-s-ellipsoid)
      - [Herpolhode](#herpolhode)
      - [Polhode](#polhode)
  - [Parallel axis theorem](#parallel-axis-theorem)
    - [Tangent-axis inertia of a spherical shell](#tangent-axis-inertia-of-a-spherical-shell)
  - [Perpendicular axis theorem](#perpendicular-axis-theorem)
  - [Angular rocket equation](#angular-rocket-equation)
  - [Moment of inertia of a solid cone about its vertex](#moment-of-inertia-of-a-solid-cone-about-its-vertex)
  - [Moment of inertia of a pointed cubic-profile solid of revolution](#moment-of-inertia-of-a-pointed-cubic-profile-solid-of-revolution)
- [Lagrange, Euler, and Kovalevskaya tops](#lagrange-euler-and-kovalevskaya-tops)
- [Euler angles](#euler-angles)
  - [Euler angles for a symmetric top](#euler-angles-for-a-symmetric-top)
    - [Heavy symmetric top Lagrangian](#heavy-symmetric-top-lagrangian)
      - [Lagrange top](#lagrange-top)
        - [Steady precession of a Lagrange top](#steady-precession-of-a-lagrange-top)
      - [Heavy symmetric top Hamiltonian](#heavy-symmetric-top-hamiltonian)
        - [Heavy symmetric top reduction](#heavy-symmetric-top-reduction)
          - [Gyroscopic stabilization of an inverted symmetric top](#gyroscopic-stabilization-of-an-inverted-symmetric-top)
- [Rolling without slipping](#rolling-without-slipping)
  - [Rolling-cylinder loop contact threshold](#rolling-cylinder-loop-contact-threshold)
    - [Finite-friction qualification of a marginal rolling loop](#finite-friction-qualification-of-a-marginal-rolling-loop)
  - [Rolling constraint inside a moving circular track](#rolling-constraint-inside-a-moving-circular-track)
  - [Impulse-driven slipping-to-rolling transition of a sphere](#impulse-driven-slipping-to-rolling-transition-of-a-sphere)
    - [Cue height for immediate rolling](#cue-height-for-immediate-rolling)
  - [Ball bearing](#ball-bearing)
    - [Rolling ball between concentric races](#rolling-ball-between-concentric-races)
  - [Effective mass of a rolling rigid body](#effective-mass-of-a-rolling-rigid-body)
    - [Pulley coupled to a rolling disc](#pulley-coupled-to-a-rolling-disc)
  - [Spring-mounted rolling cylinder](#spring-mounted-rolling-cylinder)
  - [Rolling-time factor on a straight incline](#rolling-time-factor-on-a-straight-incline)
  - [Rolling uniform solid hemisphere](#rolling-uniform-solid-hemisphere)
  - [Slipping solid cylinder on an incline](#slipping-solid-cylinder-on-an-incline)
  - [Rolling inside a fixed circular cylinder](#rolling-inside-a-fixed-circular-cylinder)
    - [Small oscillations inside a circular cylinder](#small-oscillations-inside-a-circular-cylinder)
- [Rigid body orientation](#rigid-body-orientation)

## Bell-clapper loss of contact

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

Let a bell have axial [moment of inertia](#moment-of-inertia) $Mk^2$ and [centre of mass](classical-mechanics.md#center-of-mass) h from its axle. A clapper of [point mass](classical-mechanics.md#point-mass) m at radius l touches the bell at fixed relative angle $\beta$. While they remain in contact, the clapper angle $\theta$ from the upward vertical obeys $(Mk^2+ml^2)\ddot\theta=Mgh\sin(\theta-\beta)+mgl\sin\theta$. The contact [force](force.md) opposing increasing angle is $N=mg\sin\theta-ml\ddot\theta$. Eliminating the [acceleration](classical-mechanics.md#acceleration) gives

$$
N=\frac{mMg}{Mk^2+ml^2}[k^2\sin\theta-lh\sin(\theta-\beta)].
$$

The first zero on the physical trajectory marks detachment, because a nonadhesive contact cannot support negative [normal force](force.md#normal-force). Selecting the correct trigonometric branch is part of the contact problem.

## Major-axis relaxation theorem

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

At fixed [angular momentum](momentum.md#angular-momentum), rotational [energy](energy.md) is minimized by [rotation](riemannian-geometry.md#rotation-mathematics) about the largest principal [moment of inertia](#moment-of-inertia). Indeed, $T=\sum_iL_i^2/(2I_i)\geq\sum_iL_i^2/(2I_{\max})$. Weak internal dissipation can therefore relax a nearly rigid isolated body towards that axis. A perfectly rigid torque-free body conserves [energy](energy.md) and does not settle; both extreme-inertia axes are stable in its ideal dynamics. The maximum-inertia axis need not be the geometrically longest axis.

## Centre of percussion

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

For a body constrained to rotate about a fixed pivot, a perpendicular [impulse](classical-mechanics.md#impulse) $K$ delivered at distance $b$ from the pivot produces $\omega=Kb/I_O$. If the [centre of mass](classical-mechanics.md#center-of-mass) is distance $h$ from the pivot, its [momentum](momentum.md) is $M\omega h$. The pivot [impulse](classical-mechanics.md#impulse) is $J_O=M\omega h-K$, and vanishes when $b=I_O/(Mh)$. This impact location is the [centre of percussion](#centre-of-percussion). The result assumes the stated planar rigid-body geometry and a short [impulse](classical-mechanics.md#impulse); it is not a claim that all [forces](force.md) at the pivot vanish afterward.

### Hinge impulse of an edge-pivoted square plate

↑ **Parent:** [Centre of percussion](#centre-of-percussion)

For a uniform square plate of side $l$ hinged along an edge, $h=l/2$ and $I_H=Ml^2/3$. An [impulse](classical-mechanics.md#impulse) $K$ normal to the plate, applied a distance $a$ below the centre, gives $v_G=3K(1+2a/l)/(4M)$ and signed hinge [impulse](classical-mechanics.md#impulse) $J_H=K(3a/(2l)-1/4)$. Therefore the hinge [impulse](classical-mechanics.md#impulse) vanishes at $a=l/6$ below the centre, a distance $2l/3$ from the hinge. The sign of $J_H$ identifies the reaction direction; its magnitude is $|J_H|$.

## Rotational equation of motion

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

The net external [torque](momentum.md#torque) about an inertial origin equals the time derivative of [angular momentum](momentum.md#angular-momentum). For rotation about a fixed axis with constant [moment of inertia](#moment-of-inertia), its axial component reduces to $I\dot\omega=\tau$.

## Constant-power rotational acceleration

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

A [rigid body](rigid-body-dynamics.md) with [moment of inertia](#moment-of-inertia) $I$, constant driving [power](energy.md#power) $P$ and linear resisting [torque](momentum.md#torque) $-\gamma\omega$ has an exponential approach of $\omega^2$ to $P/\gamma$. The ideal drive requires [torque](momentum.md#torque) $P/\omega$, so starting from rest is a limiting [energy](energy.md) model with singular initial [torque](momentum.md#torque).

## Vehicle rollover threshold

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

For a rigid vehicle turning on a level road, with [centre of mass](classical-mechanics.md#center-of-mass) height $h$, half track width $a$ and turn radius $R_b$, sufficient [static friction](force.md#static-friction) supplies [centripetal acceleration](classical-mechanics.md#centripetal-acceleration) $v^2/R_b$. The inner and outer wheel [normal forces](force.md#normal-force) obey $N_i+N_o=Mg$ and $a(N_o-N_i)=Mhv^2/R_b$. The inner contact force first vanishes at the displayed [speed](classical-mechanics.md#speed). The approximation neglects suspension movement and extra [torques](momentum.md#torque); inadequate [static friction](force.md#static-friction) can cause sliding before rollover.

## Two hinged rods with both ends sliding on a floor

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

Two identical uniform [rigid bodies](rigid-body-dynamics.md) of rod shape, each of length $2l$ and mass $M$, form a symmetric arch with a free common hinge and both outer ends sliding without friction on a horizontal floor. At angle $\theta$, each center has [speed](classical-mechanics.md#speed) $l|\dot\theta|$, giving total [kinetic energy](energy.md#kinetic-energy) $4Ml^2\dot\theta^2/3$. The total gravitational [potential energy](energy.md#potential-energy) is $2Mgl\sin\theta$. [Conservation of energy](mathematical-physics.md#conservation-of-energy) from rest at $\alpha$ gives the displayed hinge impact [speed](classical-mechanics.md#speed). Unlike fixing one outer endpoint, allowing both endpoints to slide keeps the arch center horizontally fixed. The floor reaction on each rod is $Mg[1+9\sin^2\theta-6\sin\alpha\sin\theta]/4$, nonnegative throughout this fall.

## Endpoint collision of two freely rotating equal rods

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

Each massless rod has endpoint masses $m$ at distance $\ell$ from its centre, hence total mass $2m$ and [moment of inertia](#moment-of-inertia) $2m\ell^2$. In a symmetric opposite-end collision with centres approaching at speed $V$, a horizontal [impulse](classical-mechanics.md#impulse) $J$ changes each centre speed by $J/(2m)$ and each contact-point speed by $J/m$. The [coefficient of restitution](classical-mechanics.md#coefficient-of-restitution) gives $2J/m-2V=2eV$. Both rods rotate in the same sense for the staggered vertical configuration; their centre speeds after impact are $V(3-e)/4$.

// Target: electromagnetism.bigb

## Two hinged rods sliding on a floor

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

Two equal uniform rods of length $2l$ and mass $M$, one pivoted to the floor and the other endpoint sliding on it, have arch coordinates $B=(2l\cos\theta,2l\sin\theta)$ and $C=(4l\cos\theta,0)$. The [kinetic energy decomposition about the center of mass](energy.md#kinetic-energy-decomposition-about-the-center-of-mass) gives $T=\tfrac43Ml^2(1+3\sin^2\theta)\dot\theta^2$, while gravitational [potential energy](energy.md#potential-energy) is $2Mgl\sin\theta$. [Conservation of energy](mathematical-physics.md#conservation-of-energy) from rest at angle $\alpha$ gives the displayed equation and hinge impact [speed](classical-mechanics.md#speed) $\sqrt{6gl\sin\alpha}$, provided contact is maintained. The endpoint's normal reaction becomes negative during this constrained fall if $\sin\alpha>35/54$; a unilateral floor then permits detachment and the constrained formula no longer describes the entire motion.

## Solid-body rotation

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

In solid-body rotation the [angular velocity](#angular-velocity) is independent of distance from the rotation axis, so tangential speed is proportional to cylindrical radius. A galactic region with this [galaxy rotation curve](galaxy.md#galaxy-rotation-curve) has [radial epicyclic frequency](astrophysical-disk.md#radial-epicyclic-frequency) $\kappa=2\Omega$.

## Symmetric top

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_top)

A symmetric top is a [rigid body](rigid-body-dynamics.md) with two equal principal moments of inertia, conventionally $I_1=I_2$. Its third principal axis is its symmetry axis.

### Prolate symmetric top

↑ **Parent:** [Symmetric top](#symmetric-top)

A rotor with two equal transverse moments and a smaller symmetry-axis moment, $I_a<I_b=I_c$. Its [rotational constants](molecule.md#rotational-constant) obey $A>B=C$.

### Oblate symmetric top

↑ **Parent:** [Symmetric top](#symmetric-top)

An [oblate symmetric top](#oblate-symmetric-top) has two equal smaller principal [moments of inertia](#moment-of-inertia) and a larger [moment of inertia](#moment-of-inertia) about its symmetry axis. A planar trigonal [molecule](molecule.md), such as [boron trifluoride](chemical-substance.md#boron-trifluoride), is an example. Its axial [rotational constant](molecule.md#rotational-constant) is smaller than its transverse [rotational constant](molecule.md#rotational-constant).

### Torque-free precession of a symmetric top

↑ **Parent:** [Symmetric top](#symmetric-top)

For an axially symmetric [rigid body](rigid-body-dynamics.md) with $I_1=I_2=I_\perp$ and $I_3=I_\parallel$, no external [torque](momentum.md#torque) means that [angular momentum](momentum.md#angular-momentum) $\mathbf L$ is fixed in an [inertial frame](mathematical-physics.md#inertial-frame). The axial [angular velocity](#angular-velocity) $\omega_3$ is constant by [Euler equations for a torque-free rigid body](#euler-equations-for-a-torque-free-rigid-body), and the symmetry axis obeys

$$
\dot{\mathbf e}_3=\frac{\mathbf L}{I_\perp}\times\mathbf e_3.
$$

Its angle to $\mathbf L$ is constant and it precesses in space at $L/I_\perp$. The transverse angular-velocity components instead rotate in body coordinates at signed rate $(I_\parallel-I_\perp)\omega_3/I_\perp$. These are different frame descriptions and must not be substituted for one another.

#### Body-frame and space-frame frequencies of free symmetric-top precession

↑ **Parent:** [Torque-free precession of a symmetric top](#torque-free-precession-of-a-symmetric-top)

For principal inertias $I_\perp,I_\perp,I_\parallel$, the transverse angular-velocity components rotate in body axes at signed rate $(I_\parallel-I_\perp)\omega_3/I_\perp$. The symmetry axis precesses about the inertially fixed [angular momentum](momentum.md#angular-momentum) at rate $L/I_\perp$. These are different frame-dependent descriptions of the same motion.

### Heavy symmetric top

↑ **Parent:** [Symmetric top](#symmetric-top)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heavy_symmetric_top)

A heavy symmetric top is a [symmetric top](#symmetric-top) with one point fixed in a uniform gravitational field. Its vertical and body-axis rotational symmetries give two cyclic Euler angles.

#### Symmetry-axis equation of a heavy symmetric top

↑ **Parent:** [Heavy symmetric top](#heavy-symmetric-top)

Writing the unit symmetry axis as $n$ and axial spin momentum as $s=I_3\omega_3$, [angular momentum](momentum.md#angular-momentum) is $L=I_1n\times\dot n+sn$. Taking its derivative and applying gravitational [torque](momentum.md#torque) gives $I_1n\times\ddot n+s\dot n=-mg\ell n\times\widehat z$.

#### Nutation

↑ **Parent:** [Heavy symmetric top](#heavy-symmetric-top)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nutation)

Variation in the inclination of a rotating body's axis, distinguished from its azimuthal [precession](#precession). For a [heavy symmetric top](#heavy-symmetric-top), the cyclic angular momenta reduce the motion to $\dot\mu^2=F(\mu)$ with $\mu=\cos\theta$ and $F$ cubic. Its admissible interval and turning points describe the nutation.

#### Uniform precession of a heavy symmetric top

↑ **Parent:** [Heavy symmetric top](#heavy-symmetric-top)

A [heavy symmetric top](#heavy-symmetric-top) precesses uniformly when its inclination is constant and its azimuthal speed is constant. For a nonvertical inclination, the condition is $I_1\cos\theta\,\Omega^2-I_3\omega_3\Omega+Mgl=0$. The real-root condition depends on whether the body axis points above or below the horizontal.

##### Slow and fast steady precession

↑ **Parent:** [Uniform precession of a heavy symmetric top](#uniform-precession-of-a-heavy-symmetric-top)

When $s^2\gg4mg\ell I_1\cos\theta$, the two nonvertical steady-precession roots are approximately $mg\ell/s$ and $s/(I_1\cos\theta)-mg\ell/s$. These asymptotic descriptions do not apply at a singular denominator without taking the original quadratic limit.

## Precession

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Precession)

Precession is the rotation of a body's spin axis about another direction, such as the vertical or the conserved angular-momentum vector.

### Precession period

↑ **Parent:** [Precession](#precession)

The time for a precessing orientation to turn through $2\pi$. An unlabelled line is unchanged by a $\pi$ turn, so its visible pattern can repeat after half the full [precession period](#precession-period).

## Angular velocity

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Angular_velocity)

Angular velocity is the vector whose direction gives the instantaneous rotation axis and whose magnitude gives the angular speed.

### Angular acceleration

↑ **Parent:** [Angular velocity](#angular-velocity)

Angular acceleration is the time derivative of [angular velocity](#angular-velocity), $\boldsymbol\alpha=d\boldsymbol\omega/dt$. For rotation about a fixed axis, its signed scalar component obeys $\tau=I\alpha$ when the axial [moment of inertia](#moment-of-inertia) is constant and $\tau$ is the total applied [torque](momentum.md#torque) about that axis.

### Angular speed

↑ **Parent:** [Angular velocity](#angular-velocity)

Angular speed is the nonnegative magnitude of [angular velocity](#angular-velocity): $\omega=|\boldsymbol\omega|$. It measures the rate of rotation about an instantaneous axis without specifying its direction. For uniform [circular motion](classical-mechanics.md#circular-motion) of radius $R$, the ordinary [speed](classical-mechanics.md#speed) is $v=R\omega$.

## Fixed space frame

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

A fixed space frame is an inertial orthonormal basis whose axes do not rotate with the body.

## Principal body frame

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

A principal body frame is an orthonormal basis fixed in the body and aligned with the principal axes of its inertia tensor. In this frame the inertia tensor is diagonal with principal moments $I_1,I_2,I_3$.

### Principal axis

↑ **Parent:** [Principal body frame](#principal-body-frame)

A principal axis is an [eigenvector](linear-operator-theory.md#eigenvector) direction of the [inertia tensor](#inertia-tensor). Choosing three orthogonal principal axes diagonalizes the inertia tensor.

### Derivative of a body-fixed basis vector

↑ **Parent:** [Principal body frame](#principal-body-frame)

If $e_i$ is fixed in a rigid body with [angular velocity](#angular-velocity) $\omega$, then its derivative in the fixed space frame is

$$
\dot e_i=\omega\times e_i.
$$

### Body-frame derivative of a space-fixed vector

↑ **Parent:** [Principal body frame](#principal-body-frame)

If a vector $k$ is fixed in space while a body frame rotates with [angular velocity](#angular-velocity) $\omega$, its body-frame components satisfy

$$
\left(\frac{dk}{dt}\right)_{\rm body}=-\omega\times k.
$$

<h2 id="euler-s-equations-rigid-body-dynamics">Euler's equations (rigid body dynamics)</h2>

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler's_equations_(rigid_body_dynamics))

In principal body coordinates, [Euler's equations](#euler-s-equations-rigid-body-dynamics) express [angular momentum](momentum.md#angular-momentum) balance as $I\dot\omega+\omega\times(I\omega)=\tau$, with applied [torque](momentum.md#torque) $\tau$. Setting the torque to zero gives the following torque-free specialization.

### Euler equations for a torque-free rigid body

↑ **Parent:** [Euler's equations (rigid body dynamics)](#euler-s-equations-rigid-body-dynamics)

In principal-axis body coordinates, torque-free angular velocity satisfies

$$
I_1\dot\omega_1=(I_2-I_3)\omega_2\omega_3,
\quad
I_2\dot\omega_2=(I_3-I_1)\omega_3\omega_1,
\quad
I_3\dot\omega_3=(I_1-I_2)\omega_1\omega_2.
$$

#### Torque-free rigid-body invariants

↑ **Parent:** [Euler equations for a torque-free rigid body](#euler-equations-for-a-torque-free-rigid-body)

The [Euler equations for a torque-free rigid body](#euler-equations-for-a-torque-free-rigid-body) conserve rotational kinetic energy and squared angular momentum,

$$
E=\frac12\sum_{i=1}^3I_i\omega_i^2,
\qquad
L^2=\sum_{i=1}^3I_i^2\omega_i^2.
$$

Their common level sets are the intersection of two ellipsoids in angular-velocity space.

##### Quartic equation for one component of torque-free angular velocity

↑ **Parent:** [Torque-free rigid-body invariants](#torque-free-rigid-body-invariants)

Eliminating $\omega_1^2$ and $\omega_2^2$ between the conserved energy and squared angular momentum gives

$$
\dot\omega_3^2=-\frac{
\left[L^2-2EI_2+I_3(I_2-I_3)\omega_3^2\right]
\left[L^2-2EI_1+I_3(I_1-I_3)\omega_3^2\right]
}{I_1I_2I_3^2}.
$$

The right-hand side is a quartic polynomial in $\omega_3$; its real turning points delimit the nutation of the body-frame angular velocity.

#### Coplanarity in a torque-free axisymmetric rigid body

↑ **Parent:** [Euler equations for a torque-free rigid body](#euler-equations-for-a-torque-free-rigid-body)

For principal moments $I_1=I_2=I$ and symmetry-axis unit vector $e_3$, angular momentum and angular velocity obey

$$
L=I\omega+(I_3-I)\omega_3e_3.
$$

Thus $L$, $\omega$, and the symmetry axis are coplanar at every instant.

#### Intermediate axis theorem

↑ **Parent:** [Euler equations for a torque-free rigid body](#euler-equations-for-a-torque-free-rigid-body)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Intermediate_axis_theorem)

For a [rigid body](rigid-body-dynamics.md) with three distinct positive [principal moments of inertia](#principal-moment-of-inertia) $0<I_1<I_2<I_3$ and zero external [torque](momentum.md#torque) about its [centre of mass](classical-mechanics.md#center-of-mass), steady rotation about the first or third [principal axis](#principal-axis) is [Lyapunov stable](dynamical-systems.md#lyapunov-stability) in [angular velocity](#angular-velocity), while rotation about the intermediate [principal axis](#principal-axis) is unstable. Here steady rotation means $\boldsymbol\omega=\Omega\hat e_i$ in the [principal body frame](#principal-body-frame), with constant $\Omega\ne0$. A small sideways [perturbation](asymptotic-expansion.md#perturbation) remains small about the extreme [principal moments of inertia](#principal-moment-of-inertia), but generically grows about the intermediate one. Stable does not mean that the wobble decays: without [damping](wave-equation.md#damping), there is no [asymptotic stability](dynamical-systems.md#asymptotic-stability). Coincident [principal moments of inertia](#principal-moment-of-inertia) and a stationary body are excluded.[Classical Dynamics by David Tong, §3.4.3, The Asymmetric Top: Stability, printed pp. 57–58, equations (3.40)–(3.45)](physics-bibliography.md#classical-dynamics-by-david-tong/3-the-motion-of-rigid-bodies)

No external [torque](momentum.md#torque) is needed for a body to tumble. [Conservation of angular momentum](momentum.md#conservation-of-angular-momentum) fixes $\mathbf L$ in the [fixed space frame](#fixed-space-frame), but the body can turn relative to $\mathbf L$, so its [angular velocity](#angular-velocity) components in the [principal body frame](#principal-body-frame) change. The [torque-free rigid-body invariants](#torque-free-rigid-body-invariants) constrain this motion. A supported [gyroscope](momentum.md#gyroscope) with gravitational [torque](momentum.md#torque) has different governing assumptions.

##### Fixed-angular-momentum energy test for principal-axis rotation

↑ **Parent:** [Intermediate axis theorem](#intermediate-axis-theorem)

For torque-free rotation, total [angular momentum](momentum.md#angular-momentum) magnitude $J$ and rotational [kinetic energy](energy.md#kinetic-energy) are conserved. Near rotation about principal axis three, eliminate $J_3^2=J^2-J_1^2-J_2^2$ from $T=\sum_iJ_i^2/(2I_i)$ to obtain the displayed energy difference from $J^2/(2I_3)$. If $I_3$ is largest, it is a constrained energy minimum; if smallest, a maximum. Both extrema are stable in the conservative problem. An intermediate moment gives opposite signs in the quadratic form, a saddle and instability. Dissipation changes the fixed-energy argument and must not be silently added to torque-free motion.

##### Normalized intermediate-axis model

↑ **Parent:** [Intermediate axis theorem](#intermediate-axis-theorem)

Choose an inertia unit $I_*$ and an [angular speed](#angular-speed) unit $\Omega_*>0$, so physical [principal moments of inertia](#principal-moment-of-inertia) are $I_*(1,2,3)$, physical [angular velocity](#angular-velocity) is $\Omega_*\boldsymbol\omega$, and normalized [time](classical-mechanics.md#time-in-physics) is $t=\Omega_*t_{\mathrm{physical}}$. The [Euler equations for a torque-free rigid body](#euler-equations-for-a-torque-free-rigid-body) become

$$
\dot\omega_1=-\omega_2\omega_3,\qquad
\dot\omega_2=\omega_3\omega_1,\qquad
\dot\omega_3=-\frac13\omega_1\omega_2.
$$

This is a physically admissible ideal planar [mass](classical-mechanics.md#mass) distribution: $I_3=I_1+I_2$ is the [perpendicular axis theorem](#perpendicular-axis-theorem). A book of finite thickness need not have these exact ratios.

For an original comparison, start with [angular velocity](#angular-velocity) $(1,\varepsilon,0)$, $(\varepsilon,1,0)$ or $(\varepsilon,0,1)$, respectively. With $\varepsilon=0.01$, the transverse [Euclidean norm](normed-vector-space.md#euclidean-norm) stays small about axes one and three, but becomes order one about axis two. For the intermediate-axis start, its [linearization](algebra.md#linearization) gives

$$
\omega_1\simeq\varepsilon\cosh(t/\sqrt3),\qquad
\omega_3\simeq-\frac{\varepsilon}{\sqrt3}\sinh(t/\sqrt3),\qquad
\omega_2\simeq1.
$$

The [hyperbolic functions](calculus.md#hyperbolic-function) contain a growing [exponential function](calculus.md#exponential-function) with rate $\lambda_2=1/\sqrt3$. Reducing $\varepsilon$ tenfold delays reaching the same small transverse amplitude by approximately $\sqrt3\log 10\simeq3.99$ normalized [time](classical-mechanics.md#time-in-physics) units, once the growing term dominates. That delays the instability. Once the transverse [angular velocity](#angular-velocity) is comparable to the main component, the [linearization](algebra.md#linearization) ceases to describe the motion.

<a id="image-small-perturbations-about-the-three-principal-axes"></a>
![](intermediate-axis-perturbation-growth.png)

**[Figure 1](#image-small-perturbations-about-the-three-principal-axes). Small perturbations about the three principal axes**. Original [Runge-Kutta method](runge-kutta-method.md) calculations for the [normalized intermediate-axis model](#normalized-intermediate-axis-model), with initial [angular velocity](#angular-velocity) $(1,0.01,0)$, $(0.01,1,0)$ and $(0.01,0,1)$. Left: transverse [Euclidean norm](normed-vector-space.md#euclidean-norm) relative to each initial [principal axis](#principal-axis). Right: full [Euler equations for a torque-free rigid body](#euler-equations-for-a-torque-free-rigid-body) compared with the displayed [linearization](algebra.md#linearization), also using $(0.001,1,0)$. Dashed curves are linear predictions. These are model curves, not measured throws.

##### Torque-free tumbling

↑ **Parent:** [Intermediate axis theorem](#intermediate-axis-theorem)

A useful readout of a tumble is the alignment of the intermediate [principal axis](#principal-axis) $\hat e_2$ with the conserved [angular momentum](momentum.md#angular-momentum) direction $\hat L$. In the [principal body frame](#principal-body-frame), write $L_i=I_i\omega_i$ and $L=|\mathbf L|$. Then

$$
c_2(t)=\hat e_2(t)\cdot\hat L=\frac{L_2(t)}L.
$$

A change from $c_2\simeq+1$ to $c_2\simeq-1$ means that the directed body axis has turned nearly $180^\circ$ relative to $\mathbf L$. It does not mean that $\mathbf L$ reversed in the [fixed space frame](#fixed-space-frame). The unsigned line through that [principal axis](#principal-axis) hides this distinction, so a marked end matters in an actual demonstration.

For the [normalized intermediate-axis model](#normalized-intermediate-axis-model) with $\boldsymbol\omega(0)=(0.01,1,0)$, the [rotational kinetic energy](energy.md#rotational-kinetic-energy) and squared [angular momentum](momentum.md#angular-momentum) are $E=1.00005$ and $L^2=4.0001$. Hence $L^2-2EI_2=-0.0001$: this initial condition lies close to, but off, the [intermediate-axis separatrix](#intermediate-axis-separatrix). An independent calculation evolves $\dot{\mathbf L}_{\mathrm{body}}=\mathbf L_{\mathrm{body}}\times I^{-1}\mathbf L_{\mathrm{body}}$ and a [rotation matrix](linear-algebra.md#rotation-matrix) taking body components to space components. The intermediate [principal axis](#principal-axis) crosses $c_2=0$ at normalized [times](classical-mechanics.md#time-in-physics) approximately $10.3773$ and $31.1319$, alternating long nearly aligned intervals with quicker reversals.

<a id="image-torque-free-reversals-of-a-nearly-aligned-body-axis"></a>
![](intermediate-axis-body-alignment-and-phase.png)

**[Figure 2](#image-torque-free-reversals-of-a-nearly-aligned-body-axis). Torque-free reversals of a nearly aligned body axis**. Original independent [Runge-Kutta method](runge-kutta-method.md) calculation in [angular momentum](momentum.md#angular-momentum) and [rotation matrix](linear-algebra.md#rotation-matrix) variables, starting with $(L_1,L_2,L_3)=(0.01,2,0)$ in the [normalized intermediate-axis model](#normalized-intermediate-axis-model). Left: body-frame orbit projected onto $(L_1/L,L_3/L)$; dashed lines are the [intermediate-axis separatrix](#intermediate-axis-separatrix) projections $L_3=\pm\sqrt3L_1$. The red point is the initial condition; the inset resolves its separation from those lines. Right: $c_2=L_2/L$, with dotted lines at the first two zero crossings. The full [angular momentum](momentum.md#angular-momentum) vector remains fixed in space.

Both calculations use step size $0.005$ without rescaling either invariant. Over $0\le t\le50$, the tumbling calculation changes [rotational kinetic energy](energy.md#rotational-kinetic-energy) and squared [angular momentum](momentum.md#angular-momentum) by less than $4\times10^{-13}$ relative to their initial values. Reconstructing $\mathbf L$ in the [fixed space frame](#fixed-space-frame) gives relative error below $3\times10^{-12}$. Halving the step changes the body components and [rotation matrix](linear-algebra.md#rotation-matrix) entries by less than $3\times10^{-10}$. These checks distinguish physical tumbling from numerical drift. On the exact [intermediate-axis separatrix](#intermediate-axis-separatrix), approach to an intermediate-axis rotation takes infinite [time](classical-mechanics.md#time-in-physics); the recurrent off-separatrix example here is different.

##### Spinning-book demonstration

↑ **Parent:** [Intermediate axis theorem](#intermediate-axis-theorem)

Clemson's documented apparatus is a book held tightly closed with several rubber bands. Toss it freely with spin about each [principal axis](#principal-axis) in turn: the stated visual readout is steady orientation for the smallest and largest [principal moments of inertia](#principal-moment-of-inertia), but a flip before the catch for the intermediate one. The same book and the two extreme-axis throws provide comparison controls; the bands support the [rigid body](rigid-body-dynamics.md) approximation by restraining the pages. This is a documented qualitative demonstration, not a measurement of $\lambda_2$.[Spinning Book by Clemson University, physics lecture demonstrations, 1Q60.40: Purpose, Description and Equipment](physics-bibliography.md#spinning-book-by-clemson-university)

For a rectangular book with length $a$, width $b$ and thickness $c$, where $a>b>c$, a uniform [mass](classical-mechanics.md#mass) model gives [principal moments of inertia](#principal-moment-of-inertia) $M(b^2+c^2)/12$, $M(a^2+c^2)/12$ and $M(a^2+b^2)/12$. The intermediate [principal axis](#principal-axis) runs across the width through the [centre of mass](classical-mechanics.md#center-of-mass); the maximum is normal to the cover. A marked cover or end helps distinguish ordinary spin from reversal of a directed body axis.

Interpret only the interval after release and before the catch: hand contact applies [torque](momentum.md#torque), whereas [gravity](physics.md#gravity) in a [uniform gravitational field](classical-mechanics.md#uniform-gravitational-field) has zero net [torque](momentum.md#torque) about the [centre of mass](classical-mechanics.md#center-of-mass) because $\int\mathbf r\,dm=0$. Air resistance, page motion, an imperfect release and short flight limit the approximation. A toss ending before the [perturbation](asymptotic-expansion.md#perturbation) grows need not reveal instability. Comparable initial [angular speeds](#angular-speed) and flight durations would improve the comparison; these are suggested controls, not quantified controls reported by Clemson.

##### Linear stability of principal-axis rotation

↑ **Parent:** [Intermediate axis theorem](#intermediate-axis-theorem)

For $0<I_1<I_2<I_3$, the transverse [linear stability](dynamical-systems.md#linear-stability) rates about steady rotation with signed component $\Omega\ne0$ are

$$
\nu_1=|\Omega|\sqrt{\frac{(I_2-I_1)(I_3-I_1)}{I_2I_3}},\qquad
\nu_3=|\Omega|\sqrt{\frac{(I_3-I_2)(I_3-I_1)}{I_1I_2}},\qquad
\lambda_2=|\Omega|\sqrt{\frac{(I_2-I_1)(I_3-I_2)}{I_1I_3}}.
$$

Axes one and three have transverse [eigenvalues](linear-operator-theory.md#eigenvalue) $\pm i\nu_1$ and $\pm i\nu_3$, producing bounded [oscillations](wave.md#oscillation). Axis two has transverse [eigenvalues](linear-operator-theory.md#eigenvalue) $\pm\lambda_2$, giving growing and decaying [exponential functions](calculus.md#exponential-function). A neutral longitudinal [perturbation](asymptotic-expansion.md#perturbation) corresponds to a small change of $\Omega$. Generic intermediate-axis disturbances contain a growing component; a precisely chosen decaying direction is exceptional. For the [normalized intermediate-axis model](#normalized-intermediate-axis-model) with $|\Omega|=1$, the values are $\nu_1=1/\sqrt3$, $\nu_3=1$ and $\lambda_2=1/\sqrt3$.

Proof outline: the [linearization](algebra.md#linearization) of the [Euler equations for a torque-free rigid body](#euler-equations-for-a-torque-free-rigid-body) about the third [principal axis](#principal-axis) gives transverse [perturbations](asymptotic-expansion.md#perturbation) obeying

$$
\dot\omega_1=\frac{I_2-I_3}{I_1}\Omega\omega_2,\qquad
\dot\omega_2=\frac{I_3-I_1}{I_2}\Omega\omega_1,
$$

and hence

$$
\ddot\omega_1=-\Omega^2\frac{(I_3-I_2)(I_3-I_1)}{I_1I_2}\omega_1.
$$

Cyclic permutation gives the other rates. For nonlinear [Lyapunov stability](dynamical-systems.md#lyapunov-stability) of the extreme rotations, use the [torque-free rigid-body invariants](#torque-free-rigid-body-invariants): the conserved [quadratic forms](quadratic-form.md) $L^2-2I_1E$ and $2I_3E-L^2$ have strictly positive transverse coefficients about axes one and three respectively. They bound transverse [angular velocity](#angular-velocity), while $E$ bounds its longitudinal change near nonzero rotation. Imaginary transverse [eigenvalues](linear-operator-theory.md#eigenvalue) alone would not establish this nonlinear conclusion.[Classical Dynamics by David Tong, §3.4.3, equations (3.41)–(3.45), and §3.4.4, invariants (3.46)–(3.47); the invariant-bound argument here is an original short derivation](physics-bibliography.md#classical-dynamics-by-david-tong/3-the-motion-of-rigid-bodies)

The practical lesson is to choose a stable [principal axis](#principal-axis) when using rotation to maintain an instrument's pointing direction. Both extreme [principal moments of inertia](#principal-moment-of-inertia) are stable in the ideal torque-free model; if internal [damping](wave-equation.md#damping) lowers [rotational kinetic energy](energy.md#rotational-kinetic-energy) while approximately preserving [angular momentum](momentum.md#angular-momentum), the minimum energy $E=L^2/(2I_3)$ instead favors the largest [principal moment of inertia](#principal-moment-of-inertia). A control system must account for [torque](momentum.md#torque), changing [mass](classical-mechanics.md#mass) distributions and flexibility before applying this ideal result.

##### Intermediate-axis separatrix

↑ **Parent:** [Intermediate axis theorem](#intermediate-axis-theorem)

On the invariant level $L^2=2EI_2$, the torque-free rigid-body orbit is a separatrix joining the two intermediate-axis rotations. With

$$
\mu=\sqrt{\frac{2E}{I_2}},
\qquad
\lambda=\mu\sqrt{\frac{(I_3-I_2)(I_2-I_1)}{I_1I_3}},
$$

one orientation has $\omega_2(t)=\mu\tanh(\lambda(t-t_0))$; the other components are constant multiples of $\operatorname{sech}(\lambda(t-t_0))$.

## Moment of inertia

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moment_of_inertia)

The [moment of inertia](#moment-of-inertia) about a specified axis measures how a [mass](classical-mechanics.md#mass) distribution resists changes of [angular velocity](#angular-velocity) about that axis. For [point masses](classical-mechanics.md#point-mass) $m_i$ at perpendicular distances $r_{\perp i}$, or a continuous distribution with [mass density](fluid-mechanics.md#density) $\rho$,

$$
I=\sum_i m_i r_{\perp i}^2,
\qquad I=\int r_\perp^2\,dm=\int r_\perp^2\rho\,dV.
$$

Its [SI](physics.md#international-system-of-units) unit is $\mathrm{kg\,m^2}$. The distance is to the entire axis, not to one point on it: moving a [point mass](classical-mechanics.md#point-mass) along the axis leaves its contribution unchanged. The [moment of inertia](#moment-of-inertia) depends on both the distribution and the chosen axis; it is not determined by total [mass](classical-mechanics.md#mass) alone. About an axis fixed in an [inertial frame](mathematical-physics.md#inertial-frame), a [rigid body](rigid-body-dynamics.md) with larger [moment of inertia](#moment-of-inertia) has smaller [angular acceleration](#angular-acceleration) under the same net axial [torque](momentum.md#torque), and greater [rotational kinetic energy](energy.md#rotational-kinetic-energy) at the same [angular speed](#angular-speed).[Chapter 19: Center of Mass; Moment of Inertia](physics-bibliography.md#the-feynman-lectures-on-physics-volume-i-by-richard-feynman-and-others/chapter-19-center-of-mass-moment-of-inertia)

For a simple model, put four equal [point masses](classical-mechanics.md#point-mass) of total [mass](classical-mechanics.md#mass) $M$ on light rigid spokes at radius $a$. Their [moment of inertia](#moment-of-inertia) is $Ma^2$. Doubling $a$ quadruples the [moment of inertia](#moment-of-inertia) without changing $M$. The illustrated placements $a=R/3$ and $a=R$ give $MR^2/9$ and $MR^2$. Actual spokes and finite-sized weights contribute their own [moments of inertia](#moment-of-inertia); the [point mass](classical-mechanics.md#point-mass) model neglects them. Repositioning weights during rotation also breaks the fixed-distribution assumption, so it requires a separate [work](energy.md#work) and [angular momentum](momentum.md#angular-momentum) calculation.

<a id="image-same-total-mass-different-radial-placement-and-moment-of-inertia"></a>
![](rotational-inertia-energy-mass-distribution.png)

**[Figure 3](#image-same-total-mass-different-radial-placement-and-moment-of-inertia). Same total mass, different radial placement and moment of inertia**. Original model diagrams, not experimental data. The upper pair has four equal [point masses](classical-mechanics.md#point-mass) on negligible-mass spokes, at $R/3$ and $R$ from a perpendicular central axis. The lower pair compares a uniform disc with an ideal thin ring of the same [mass](classical-mechanics.md#mass) $M$ and outer radius $R$. The displayed [moments of inertia](#moment-of-inertia) determine [rotational kinetic energy](energy.md#rotational-kinetic-energy) at a shared [angular speed](#angular-speed). The visible thickness of the ring and size of the point markers are only drawing conventions.

The [moment of inertia of a uniform disc](#moment-of-inertia-of-a-uniform-disc) follows by dividing it into concentric [annuli](topology.md#annulus-mathematics): $dm=(2M/R^2)r\,dr$ and $I=\int_0^R r^2(2M/R^2)r\,dr=MR^2/2$. For an ideal thin ring every [mass](classical-mechanics.md#mass) element is at $R$, so $I=MR^2$. A ring of finite radial thickness instead uses the [moment of inertia of a uniform annulus](#moment-of-inertia-of-a-uniform-annulus), $I=M(R^2+b^2)/2$, with inner radius $b$. A [moment of inertia](#moment-of-inertia) is thus a compact summary of radial placement rather than a complete description of shape. For several joined pieces, their [moments of inertia](#moment-of-inertia) add only when each is calculated about the same axis.[§10.5](physics-bibliography.md#university-physics-volume-1-by-william-moebs-and-others/10-5-calculating-moments-of-inertia)

A [physical pendulum](mathematical-physics.md#physical-pendulum) makes the [moment of inertia](#moment-of-inertia) measurable through timing. Martín Monteiro, Cecilia Stari, Cecilia Cabeza and Arturo C. Martí used a metal bar with suspension holes $1.0\,\mathrm{cm}$ apart and an attached smartphone. They report bar length $1.199\,\mathrm m$, bar [mass](classical-mechanics.md#mass) $0.2518\,\mathrm{kg}$ and phone [mass](classical-mechanics.md#mass) $0.1311\,\mathrm{kg}$. Changing the suspension hole changes the pivot axis. Their readouts were phone [gyroscope](momentum.md#gyroscope) [angular velocity](#angular-velocity) records, analyzed by [autocorrelation](time-series.md#autocorrelation) or a fit to a [sinusoid](geometry-and-topology.md#sinusoid), and an independent photogate; the logged records for the [sinusoid](geometry-and-topology.md#sinusoid) fits lasted $10\,\mathrm s$. They observed agreement between the three timing methods and the geometry-based model, including a minimum of [oscillation period](classical-mechanics.md#period-of-an-oscillation) as the suspension point varied. These are reported apparatus details and observations, not measurements made for this article.[Experimental analysis of a physical pendulum with variable suspension point by Martín Monteiro and others](physics-bibliography.md#experimental-analysis-of-a-physical-pendulum-with-variable-suspension-point-by-martin-monteiro-and-others)

To infer a [moment of inertia](#moment-of-inertia) from such a measurement, determine the total [mass](classical-mechanics.md#mass) $M_{\mathrm{tot}}$ including every attached part, locate the assembly's [centre of mass](classical-mechanics.md#center-of-mass) $G$, and measure its distance $h>0$ below the horizontal pivot $O$. Record successive crossings in the same direction, or the elapsed [time](classical-mechanics.md#time-in-physics) $t_N$ for $N$ complete [oscillations](wave.md#oscillation), giving [oscillation period](classical-mechanics.md#period-of-an-oscillation) $P=t_N/N$. The [physical pendulum](mathematical-physics.md#physical-pendulum) model with a fixed pivot, a [uniform gravitational field](classical-mechanics.md#uniform-gravitational-field), negligible [friction](newtonian-mechanics.md#friction) and the [small-angle approximation](geometry-and-topology.md#small-angle-approximation) gives

$$
I_O\ddot\theta=-M_{\mathrm{tot}}gh\sin\theta,
\qquad P\simeq2\pi\sqrt{\frac{I_O}{M_{\mathrm{tot}}gh}},
\qquad I_{O,\mathrm{inferred}}=M_{\mathrm{tot}}gh\left(\frac{P}{2\pi}\right)^2.
$$

The crossing times, [masses](classical-mechanics.md#mass) and geometric distances are the measured inputs; $I_{O,\mathrm{inferred}}$ is an inference conditional on this model, while an [integral](integral.md) over the assumed shape supplies an independent model prediction. The [parallel axis theorem](#parallel-axis-theorem) converts the inferred pivot [moment of inertia](#moment-of-inertia) to one about a parallel axis through $G$. The controls and interpretation of that comparison are described there. An axial measurement determines one scalar [moment of inertia](#moment-of-inertia), not the complete [inertia tensor](#inertia-tensor) needed for general rotation.

### Density-power cylindrical moment of inertia

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

For a solid cylinder with [mass density](fluid-mechanics.md#density) $\rho(r)=kr^p$ and $p>-2$, integrating cylindrical shells gives $M=2\pi LkR^{p+2}/(p+2)$ and axial [moment of inertia](#moment-of-inertia) $I_z=2\pi LkR^{p+4}/(p+4)$. Their ratio proves the displayed formula. It gives the uniform-cylinder result $MR^2/2$ at p=0 and $2MR^2/3$ at p=2. The radial density weighting must enter both mass and inertia integrals.

### Axial moment of inertia of a hollow cylinder

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

For a cylinder of uniform [mass density](fluid-mechanics.md#density) $\rho$, length $L$, inner radius $R_i$ and outer radius $R_o$, an annular element has $dm=2\pi\rho Lr\,dr$. Thus the axial [moment of inertia](#moment-of-inertia) is $I=\int r^2dm=\pi\rho L(R_o^4-R_i^4)/2$. Dividing by $M=\pi\rho L(R_o^2-R_i^2)$ yields the displayed result. At fixed [mass](classical-mechanics.md#mass), the solid-cylinder limit is $MR_o^2/2$ and the thin-shell limit is $MR^2$.

### Axial moment of inertia of a solid of revolution

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

A uniform solid with circular cross-sectional radius $r(z)$ can be sliced into thin [discs](topology.md#topological-disc). A slice of thickness $dz$ has [mass](classical-mechanics.md#mass) $dm=\rho\pi r(z)^2dz$ and axial [moment of inertia](#moment-of-inertia) $dI_z=\tfrac12r(z)^2dm$. Thus

$$
M=\rho\pi\int r(z)^2dz,\qquad I_z=\frac{\rho\pi}{2}\int r(z)^4dz.
$$

All slice axes coincide, so no [parallel axis theorem](#parallel-axis-theorem) correction is needed. For a linearly tapered section of length $l$ with end radii $r_0,r_1$, direct [integration](integral.md) gives $M=\rho\pi l(r_0^2+r_0r_1+r_1^2)/3$ and $I_z=\rho\pi l(r_0^4+r_0^3r_1+r_0^2r_1^2+r_0r_1^3+r_1^4)/10$.

### Moment-of-inertia triangle inequalities

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

For three mutually perpendicular axes through one point of a nonnegative [mass distribution](classical-mechanics.md#mass-distribution), $I_x+I_y-I_z=2\int z^2\,dm\ge0$, with cyclic counterparts. Equality holds precisely when the [mass distribution](classical-mechanics.md#mass-distribution) is supported in the plane $z=0$, giving the [perpendicular axis theorem](#perpendicular-axis-theorem). The point need not be the [centre of mass](classical-mechanics.md#center-of-mass), and the axes need not be [principal axes](#principal-axis).

### Moment of inertia of a uniform square plate

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

A uniform square of side $s$ has the displayed [moment of inertia](#moment-of-inertia) about the perpendicular axis through its centre. Integrating $x^2+y^2$ over $[-s/2,s/2]^2$ gives $s^4/6$; multiplying by the [surface mass density](fluid-mechanics.md#projected-surface-mass-density) $M/s^2$ gives the result. A square prism of any uniform thickness has the same axial formula when expressed in terms of its total mass. If the side is denoted $2a$ instead, the result is $2Ma^2/3$, so the side-length convention must be specified before substituting numerical data into a [normal mode](wave-equation.md#normal-mode) calculation.

#### Off-axis angular momentum of a square lamina

↑ **Parent:** [Moment of inertia of a uniform square plate](#moment-of-inertia-of-a-uniform-square-plate)

For a uniform square of side $a$, the principal [inertia tensor](#inertia-tensor) is $\operatorname{diag}(ma^2/12,ma^2/12,ma^2/6)$. A rotation axis tilted $45^\circ$ to the surface has equal in-plane and normal angular-velocity components. Multiplying each by its own principal moment gives the stated magnitude. In general $I_{\rm axis}\omega$ is only the axial projection of [angular momentum](momentum.md#angular-momentum).

#### In-plane inertia isotropy of a square plate

↑ **Parent:** [Moment of inertia of a uniform square plate](#moment-of-inertia-of-a-uniform-square-plate)

A uniform thin square of side $l$ and [mass](classical-mechanics.md#mass) $M$ has $I_z=Ml^2/6$ about the perpendicular central axis. Any central in-plane axis and its perpendicular in-plane partner have equal moments by $90^\circ$ rotational symmetry. The [perpendicular axis theorem](#perpendicular-axis-theorem) says their sum is $I_z$, proving $I_\phi=Ml^2/12$ for every angle $\phi$. A non-square rectangle generally lacks this angle independence.

### Moment of inertia of a uniform solid hemisphere

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

The centroid of a uniform solid hemisphere of radius $a$ lies $3a/8$ from its flat face. About a diameter of the underlying sphere parallel to that face, its [moment of inertia](#moment-of-inertia) is $2ma^2/5$. The [parallel axis theorem](#parallel-axis-theorem) therefore gives $I_G=2ma^2/5-m(3a/8)^2=83ma^2/320$ about the parallel centroidal axis. A thin hemispherical shell has a different centroid and inertia.

### Moment of inertia of a uniform solid cylinder

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

For a uniform solid cylinder of radius $a$, length $L$ and [mass density](fluid-mechanics.md#density) $\rho$, a coaxial shell carries [mass](classical-mechanics.md#mass) $dm=2\pi\rho Lr\,dr$. The axial [moment of inertia](#moment-of-inertia) is $I=\int_0^a r^2dm=\pi\rho La^4/2=ma^2/2$. The axial [moment of inertia](#moment-of-inertia) is independent of the length once [mass](classical-mechanics.md#mass) and radius are fixed. A thin cylindrical shell instead has $I=ma^2$, demonstrating why the uniform solid assumption matters.

### Reflected inertia of a no-slip wheel and roller

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

If a fixed-axis wheel of radius $R$ drives a fixed-axis roller of radius $S$ without slip, their angular-speed magnitudes satisfy $\sigma=(R/S)\omega$. Their [kinetic energy](energy.md#kinetic-energy) is $\tfrac12[I+J(R/S)^2]\omega^2$, so the displayed reflected [moment of inertia](#moment-of-inertia) governs the wheel coordinate. A roller resisting torque of magnitude $\gamma\sigma^2$ consumes power $\gamma\sigma^3$ and therefore reflects to wheel torque $\gamma(R/S)^3\omega^2$. The squared ratio belongs to inertia; the cubed ratio belongs to this quadratic resisting torque.

### Moment of inertia of a uniform annulus

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

A uniform planar annulus of outer radius $a$, inner radius $b<a$ and mass $M$ has surface density $M/[\pi(a^2-b^2)]$. Integrating $r^2$ over its mass gives the axial [moment of inertia](#moment-of-inertia) $I=M(a^2+b^2)/2$. Subtracting the inner disc from a complete disc gives the same result, provided their surface densities match.

// Target: electromagnetism.bigb

### Moment of inertia of a uniform disc

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

For a uniform disc of radius $a$ and mass $M$, annuli of radius $r$ and thickness $dr$ have mass $(M/\pi a^2)2\pi r\,dr$. Their axial [moment of inertia](#moment-of-inertia) sums to $I=\int_0^a r^2\,dm=Ma^2/2$.

### Moment of inertia of a uniform solid sphere

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

A uniform solid sphere of mass $M$ and radius $a$ has the indicated [moment of inertia](#moment-of-inertia) about any diameter. Integrating the squared perpendicular distance against uniform [mass density](fluid-mechanics.md#density) gives $I=8\pi\rho a^5/15=2Ma^2/5$. It is different from the value for a thin spherical shell and determines the rotational contribution to [kinetic energy](energy.md#kinetic-energy) during [rolling without slipping](#rolling-without-slipping).

### Mass second-moment tensor

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

The mass second-moment tensor about a [centre of mass](classical-mechanics.md#center-of-mass) is $I_{jk}=\int y_jy_k\,dm$. It measures the shape of a mass distribution and appears in [tidal torque theory](large-scale-structure-of-the-universe.md#tidal-torque-theory). It differs from the mechanical [inertia tensor](#inertia-tensor), which is $\mathcal I_{jk}=\operatorname{tr}(I)\delta_{jk}-I_{jk}$. For a uniform [ellipsoid](euclidean-geometry.md#ellipsoid) of mass $M$ and semiaxes $a_1,a_2,a_3$, its principal values are $Ma_j^2/5$.

### Inertia tensor

↑ **Parent:** [Moment of inertia](#moment-of-inertia)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inertia_tensor)

The [inertia tensor](#inertia-tensor) packages the [moments of inertia](#moment-of-inertia) about every axis through a specified point $O$ into one [symmetric matrix](linear-algebra.md#symmetric-matrix). An axis still needs a direction: if $\mathbf n$ is a [unit vector](vector-space.md#unit-vector), its scalar [moment of inertia](#moment-of-inertia) is $I_{O,\mathbf n}=\mathbf n^T\mathbf I_O\mathbf n$. The same [mass](classical-mechanics.md#mass) layout can therefore be easy to spin about one direction and harder about another. The [inertia tensor](#inertia-tensor) also determines [rotational kinetic energy](energy.md#rotational-kinetic-energy) and relates [angular velocity](#angular-velocity) to [angular momentum](momentum.md#angular-momentum) in the appropriate [rigid body](rigid-body-dynamics.md) model.

Take [position](classical-mechanics.md#position) vectors $\mathbf r=(x,y,z)$ relative to $O$, expressed in an [orthonormal basis](inner-product.md#orthonormal-basis). For [point masses](classical-mechanics.md#point-mass) $m_a$, or a continuous distribution with [mass density](fluid-mechanics.md#density) $\rho$ and $dm=\rho\,dV$,

$$
(\mathbf I_O)_{ij}=\sum_a m_a\bigl(|\mathbf r_a|^2\delta_{ij}-r_{ai}r_{aj}\bigr),
\qquad
(\mathbf I_O)_{ij}=\int\bigl(|\mathbf r|^2\delta_{ij}-r_ir_j\bigr)\,dm.
$$

Here $\delta_{ij}$ is the [Kronecker delta](multilinear-algebra.md#kronecker-delta). Equivalently, using the [identity matrix](vector-space.md#identity-matrix) $\mathbf1$ and an [outer product](vector-space.md#outer-product),

$$
\mathbf I_O=\int\bigl(|\mathbf r|^2\mathbf1-\mathbf r\mathbf r^T\bigr)\,dm
=\int\begin{pmatrix}
y^2+z^2&-xy&-xz\\
-xy&x^2+z^2&-yz\\
-xz&-yz&x^2+y^2
\end{pmatrix}\,dm.
$$

Every entry has [SI](physics.md#international-system-of-units) units $\mathrm{kg\,m^2}$. The diagonal entries are axial [moments of inertia](#moment-of-inertia); the off-diagonal entries carry a minus sign in this convention. Some texts instead define the integrals without the prefixed minus sign $\int xy\,dm$, $\int xz\,dm$, $\int yz\,dm$ as their named off-diagonal quantities and put the minus signs into the displayed [matrix](vector-space.md#matrix). Check that convention before combining formulas. [Moment of Inertia Tensor](physics-bibliography.md#newtonian-dynamics-by-richard-fitzpatrick/moment-of-inertia-tensor) [Lecture L26 - 3D Rigid Body Dynamics: The Inertia Tensor](physics-bibliography.md#16-07-dynamics/lecture-l26-3d-rigid-body-dynamics-the-inertia-tensor)

The [symmetric matrix](linear-algebra.md#symmetric-matrix) is [positive semidefinite](quadratic-form.md#positive-semidefinite-matrix), because its [quadratic form](quadratic-form.md) is

$$
\mathbf u^T\mathbf I_O\mathbf u
=\int\bigl(|\mathbf u|^2|\mathbf r|^2-(\mathbf u\cdot\mathbf r)^2\bigr)\,dm
=\int|\mathbf u\times\mathbf r|^2\,dm\geq0.
$$

The [dot product](inner-product.md#dot-product) and [cross product](vector-space.md#cross-product) identify this as a sum of squared distances when $\mathbf u$ is a [unit vector](vector-space.md#unit-vector). A zero [moment of inertia](#moment-of-inertia) occurs precisely when all the [mass](classical-mechanics.md#mass) lies on that axis, up to sets of zero [mass](classical-mechanics.md#mass). A genuine three-dimensional body with positive [mass density](fluid-mechanics.md#density) in a volume has strictly positive axial [moments of inertia](#moment-of-inertia). Do not confuse this [inertia tensor](#inertia-tensor) with the [mass second-moment tensor](#mass-second-moment-tensor) $\mathbf S=\int\mathbf r\mathbf r^T\,dm$: they obey $\mathbf I_O=\operatorname{tr}(\mathbf S)\mathbf1-\mathbf S$, where $\operatorname{tr}$ denotes the [matrix trace](linear-algebra.md#matrix-trace).

If $O$ is fixed in an [inertial frame](mathematical-physics.md#inertial-frame) and each [velocity](classical-mechanics.md#velocity) is $\mathbf v=\boldsymbol\omega\times\mathbf r$, summing the individual [kinetic energies](energy.md#kinetic-energy) and [angular momenta](momentum.md#angular-momentum) gives

$$
\mathbf L_O=\mathbf I_O\boldsymbol\omega,
\qquad
K=\frac12\boldsymbol\omega^T\mathbf I_O\boldsymbol\omega
=\frac12\boldsymbol\omega\cdot\mathbf L_O.
$$

These formulas also describe [angular momentum](momentum.md#angular-momentum) and [rotational kinetic energy](energy.md#rotational-kinetic-energy) relative to the [centre of mass](classical-mechanics.md#center-of-mass) $G$ of a translating [rigid body](rigid-body-dynamics.md). In that case the total [kinetic energy](energy.md#kinetic-energy) in the [inertial frame](mathematical-physics.md#inertial-frame) is $K_{\mathrm{total}}=\tfrac12M|\mathbf V_G|^2+\tfrac12\boldsymbol\omega^T\mathbf I_G\boldsymbol\omega$. For a general moving point $O$, the body's actual [velocities](classical-mechanics.md#velocity) include $\mathbf V_O$, so $\mathbf I_O\boldsymbol\omega$ alone need not be its [angular momentum](momentum.md#angular-momentum) about $O$. [Rotational Kinetic Energy](physics-bibliography.md#newtonian-dynamics-by-richard-fitzpatrick/rotational-kinetic-energy) [Lecture L26 - 3D Rigid Body Dynamics: The Inertia Tensor](physics-bibliography.md#16-07-dynamics/lecture-l26-3d-rigid-body-dynamics-the-inertia-tensor)

Changing the [orthonormal basis](inner-product.md#orthonormal-basis) changes components, rather than the physical distribution: if the columns of an [orthogonal matrix](linear-algebra.md#orthogonal-matrix) $Q$ are the new basis vectors expressed in the old basis, then $\mathbf I'_O=Q^T\mathbf I_OQ$. Changing the reference point is a different operation, governed by the [tensor parallel-axis theorem](#tensor-parallel-axis-theorem). Both [principal axes](#principal-axis) and [principal moments of inertia](#principal-moment-of-inertia) must therefore be quoted with their reference point.

#### Inertia tensor of a uniform cube

↑ **Parent:** [Inertia tensor](#inertia-tensor)

For a uniform [cube](euclidean-geometry.md#cube) of side $s$ and [mass](classical-mechanics.md#mass) $M$, reflection [symmetry](physics.md#symmetry-physics) makes central off-diagonal inertia components zero. Equal coordinate second moments are $\langle x^2\rangle=\langle y^2\rangle=\langle z^2\rangle=s^2/12$, so each diagonal component is $Ms^2/6$. Thus every central axis is a [principal axis](#principal-axis). A nonspherical shape can have an isotropic central [inertia tensor](#inertia-tensor): that tensor measures only quadratic moments of the [mass](classical-mechanics.md#mass) distribution, not the whole shape.

#### Inertia tensor of a displaced uniform ball

↑ **Parent:** [Inertia tensor](#inertia-tensor)

For a uniform ball of radius $R>0$ and positive [mass](classical-mechanics.md#mass) $M$, let $G$ be its [centre of mass](classical-mechanics.md#center-of-mass). Spherical symmetry gives the second-moment matrix $\int uu^Tdm=(MR^2/5)I$, so the central [inertia tensor](#inertia-tensor) is $(2MR^2/5)I$. The [tensor parallel-axis theorem](#tensor-parallel-axis-theorem) gives the displayed shifted tensor. For $X\ne0$ its [eigenvector](linear-operator-theory.md#eigenvector) along $X$ has [eigenvalue](linear-operator-theory.md#eigenvalue) $2MR^2/5$, while the two-dimensional [orthogonal complement](hilbert-space.md#orthogonal-complement) has repeated eigenvalue $M(2R^2/5+|X|^2)$. Thus it is an [isotropic tensor](multilinear-algebra.md#isotropic-tensor) exactly at $P=G$. Displacement along a chosen axis does not change that axis's moment; the transverse moments increase by $M|X|^2$.

#### Positive second-moment matrix test for an inertia tensor

↑ **Parent:** [Inertia tensor](#inertia-tensor)

For a nonnegative [mass distribution](classical-mechanics.md#mass-distribution) relative to an origin, the second-moment matrix is $\mathsf S=\int\mathbf r\mathbf r^{\mathsf T}\,dm$ and the [inertia tensor](#inertia-tensor) is $\mathsf I=\operatorname{tr}(\mathsf S)\mathsf 1-\mathsf S$. Taking the trace gives the displayed inverse formula, which must be [positive semidefinite](quadratic-form.md#positive-semidefinite-matrix). Conversely, any such $\mathsf S$ can be realized by pairs of point masses along its orthogonal principal directions. Thus this is also a realizability test when total mass and dimensions are unrestricted. In principal coordinates it is equivalent to the [moment-of-inertia triangle inequalities](#moment-of-inertia-triangle-inequalities): $I_2+I_3-I_1=2S_{11}\ge0$, with cyclic counterparts. A symmetric positive definite matrix alone need not be a physical [inertia tensor](#inertia-tensor).

#### Inertia tensor of a sheared rectangular lamina

↑ **Parent:** [Inertia tensor](#inertia-tensor)

For a uniform planar lamina with $|x_1-sx_2|\leq a$ and $|x_2|\leq b$, put $u=x_1-sx_2$, $v=x_2$. The [Jacobian determinant](multivariable-calculus.md#jacobian-determinant) is one, the mass is $M=4ab\sigma$, and symmetry puts the centre of mass at zero. Uniform rectangular moments give $\langle u^2\rangle=a^2/3$, $\langle v^2\rangle=b^2/3$, $\langle uv\rangle=0$. Substitution into $I_{ij}=\int(|x|^2\delta_{ij}-x_ix_j)dm$ yields the displayed [inertia tensor](#inertia-tensor). The in-plane [principal moments of inertia](#principal-moment-of-inertia) are $M[a^2+(1+s^2)b^2\pm\sqrt{(a^2+(s^2-1)b^2)^2+4s^2b^4}]/6$; the perpendicular moment is their sum. This separates the geometric shear from the elementary rectangular integrals.

#### Inertia tensor of paired point masses

↑ **Parent:** [Inertia tensor](#inertia-tensor)

An exact planar example makes the off-diagonal entries tangible. Join four equal [point masses](classical-mechanics.md#point-mass) $m$ with negligible-mass rigid connectors at $a(2,1,0)$, $a(-2,-1,0)$, $a(1,-1,0)$ and $a(-1,1,0)$, where $a>0$ is a length. Their [centre of mass](classical-mechanics.md#center-of-mass) is $O=(0,0,0)$. Summing $x^2$, $y^2$ and $xy$ gives $10a^2$, $4a^2$ and $2a^2$, respectively, so

$$
\mathbf I_{\mathrm{planar}}=ma^2\begin{pmatrix}4&-2&0\\-2&10&0\\0&0&14\end{pmatrix}.
$$

The $z$ axis is a [principal axis](#principal-axis), and $I_{zz}=I_{xx}+I_{yy}$ illustrates the [perpendicular axis theorem](#perpendicular-axis-theorem). The $x$ axis is not a [principal axis](#principal-axis): [angular velocity](#angular-velocity) $\boldsymbol\omega=(\Omega,0,0)$ gives [angular momentum](momentum.md#angular-momentum) $ma^2\Omega(4,-2,0)$, which points in a different direction. A bearing can enforce fixed-axis rotation despite this difference, supplying the necessary transverse [torque](momentum.md#torque).

<a id="image-paired-point-masses-and-direction-dependent-rotational-kinetic-energy"></a>
![](inertia-tensor-paired-masses-rotational-energy.png)

**[Figure 4](#image-paired-point-masses-and-direction-dependent-rotational-kinetic-energy). Paired point masses and direction-dependent rotational kinetic energy**. Original exact model. Four equal [point masses](classical-mechanics.md#point-mass) lie in the $xy$ plane with negligible-mass connectors. The curves use [angular velocity](#angular-velocity) $\boldsymbol\omega=\Omega(\cos\theta,\sin\theta,0)$ and plot $2K/(ma^2\Omega^2)$. Adding two more equal [point masses](classical-mechanics.md#point-mass) at $a(0,0,\pm1)$ raises this curve by two. Markers depict ideal [point masses](classical-mechanics.md#point-mass), not finite-sized weights; no experimental data are plotted.

For an in-plane [unit vector](vector-space.md#unit-vector) $\mathbf n=(\cos\theta,\sin\theta,0)$, the planar model has

$$
\frac{I_{O,\mathbf n}}{ma^2}=4\cos^2\theta+10\sin^2\theta-4\sin\theta\cos\theta.
$$

Its extrema are the [principal moments of inertia](#principal-moment-of-inertia) $(7-\sqrt{13})ma^2$ and $(7+\sqrt{13})ma^2$; the remaining [principal moment of inertia](#principal-moment-of-inertia) is $14ma^2$. These values follow from the two-by-two [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) $(4-\lambda)(10-\lambda)-4$, so they can be checked without trusting a numerical [eigenvalue](linear-operator-theory.md#eigenvalue) routine. At a stipulated [angular speed](#angular-speed) $\Omega=1\,\mathrm{rad/s}$, with $m=1\,\mathrm{kg}$ and $a=1\,\mathrm m$, rotation about $x$, $y$ or $z$ has [rotational kinetic energy](energy.md#rotational-kinetic-energy) $2$, $5$ or $7\,\mathrm J$, respectively.

A truly three-dimensional example adds two more equal [point masses](classical-mechanics.md#point-mass) at $a(0,0,1)$ and $a(0,0,-1)$. Each contributes $ma^2\operatorname{diag}(1,1,0)$ to the [inertia tensor](#inertia-tensor), giving

$$
\mathbf I_{\mathrm{3D}}=ma^2\begin{pmatrix}6&-2&0\\-2&12&0\\0&0&14\end{pmatrix},
\qquad
(I_1,I_2,I_3)=ma^2(9-\sqrt{13},9+\sqrt{13},14).
$$

The in-plane [principal axes](#principal-axis) stay the same while their [principal moments of inertia](#principal-moment-of-inertia) each increase by $2ma^2$. The $z$ [moment of inertia](#moment-of-inertia) stays unchanged because the added [point masses](classical-mechanics.md#point-mass) lie on that axis. This comparison changes the total [mass](classical-mechanics.md#mass) from $4m$ to $6m$; it holds the original four [point masses](classical-mechanics.md#point-mass) fixed rather than redistributing a fixed total [mass](classical-mechanics.md#mass).

#### Rotational inertia measurement with a falling mass

↑ **Parent:** [Inertia tensor](#inertia-tensor)

PASCO's [PASPORT Rotary Motion Sensor Experiment Guide](physics-bibliography.md#pasport-rotary-motion-sensor-experiment-guide), Experiment 1, specifies a PS-2120A sensor, a rod carrying two equal-radius weights, a three-step drive wheel, a thread and hanging [mass](classical-mechanics.md#mass), a clamp-on guide wheel, a support, a balance and calipers. The thread leaves the drive wheel tangentially. The sensor records [angular velocity](#angular-velocity) against [time](classical-mechanics.md#time-in-physics); a [linear regression](linear-regression.md) over the accelerating interval supplies [angular acceleration](#angular-acceleration) $\alpha$. The guide measures the drive radius with calipers and repeats the run with the weights removed to subtract the apparatus's own [moment of inertia](#moment-of-inertia). Its tables are blank: it prescribes a measurement and does not report an observed numerical agreement. [PASPORT Rotary Motion Sensor Experiment Guide](physics-bibliography.md#pasport-rotary-motion-sensor-experiment-guide)

With hanging [mass](classical-mechanics.md#mass) $m_h$ including its hanger, effective drive radius $b$, no thread slip and negligible guide-wheel inertia, [Newton's second law](force.md#newton-s-second-law) gives thread [tension](force.md#tension) $F=m_h(g-b\alpha)$. The axial [torque](momentum.md#torque) is $bF$. Under negligible [friction](newtonian-mechanics.md#friction), the inference is therefore

$$
I_{\mathrm{loaded}}=\frac{m_hgb}{\alpha}-m_hb^2.
$$

Repeat the inference for the unloaded assembly and subtract: $I_{\mathrm{weights}}=I_{\mathrm{loaded}}-I_{\mathrm{empty}}$. Omitting the $m_hb^2$ term incorrectly treats thread [tension](force.md#tension) as the hanging weight. Comparing with $(M_1+M_2)R^2$ tests the [point mass](classical-mechanics.md#point-mass) approximation; finite-sized weights also have their own [moments of inertia](#moment-of-inertia) about their [centres of mass](classical-mechanics.md#center-of-mass). [PASPORT Rotary Motion Sensor Experiment Guide](physics-bibliography.md#pasport-rotary-motion-sensor-experiment-guide)

Useful proposed checks go beyond that ideal inference. Verify the [rotary encoder](#rotary-encoder)'s angle scale by turning the shaft through a marked full revolution; check the recorded [time](classical-mechanics.md#time-in-physics) against an independent clock and the balance against a known [mass](classical-mechanics.md#mass). Measure $b$ at the thread's running surface, including thread thickness; avoid overlapping wraps that change $b$. Release without a push, inspect the [angular velocity](#angular-velocity) record for a straight interval, and stop before the hanger lands or the thread runs out. Repeat with several hanging [masses](classical-mechanics.md#mass), weight radii and rotation directions. A consistent inferred [moment of inertia](#moment-of-inertia) across drive [torques](momentum.md#torque) supports the model; curvature, direction dependence or drift indicates a limitation rather than a new [principal moment of inertia](#principal-moment-of-inertia).

For approximately constant resisting [torque](momentum.md#torque) $\tau_f\geq0$ in one rotation direction, an original calibration model is

$$
m_hgb-m_hb^2\alpha=I\alpha+\tau_f.
$$

Fit the left-hand quantity against $\alpha$ across several drives: the slope estimates the axial [moment of inertia](#moment-of-inertia) and the intercept estimates $\tau_f$. This calibration is conditional on [friction](newtonian-mechanics.md#friction) remaining constant over the fitted [angular speeds](#angular-speed); a freely slowing run can expose speed dependence. Sensor differentiation noise, guide-wheel [moment of inertia](#moment-of-inertia), thread slip, flexing connectors and uncertain weight radii limit the inference. Removing weights can also change bearing loads, so empty-apparatus subtraction does not automatically cancel [friction](newtonian-mechanics.md#friction). These are proposed controls and a model extension, not results claimed by PASCO.

A fixed-axis readout measures $\mathbf n^T\mathbf I_O\mathbf n$, not the full [inertia tensor](#inertia-tensor). In a proposed generalization, repeat about $x$, $y$, $z$ and the three diagonal directions $(\mathbf e_x+\mathbf e_y)/\sqrt2$, $(\mathbf e_x+\mathbf e_z)/\sqrt2$, $(\mathbf e_y+\mathbf e_z)/\sqrt2$, all through the same $O$. For example,

$$
I_{xy}=I_{O,(\mathbf e_x+\mathbf e_y)/\sqrt2}-\frac{I_{xx}+I_{yy}}2.
$$

Six independent scalar readings then determine the six entries of a [symmetric matrix](linear-algebra.md#symmetric-matrix). Each mounting needs its own apparatus correction, and different reference points require the [tensor parallel-axis theorem](#tensor-parallel-axis-theorem) before the readings can be combined.

##### Rotary encoder

↑ **Parent:** [Rotational inertia measurement with a falling mass](#rotational-inertia-measurement-with-a-falling-mass)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rotary_encoder)

A [rotary encoder](#rotary-encoder) converts shaft rotation into a readout of [angle](geometry-and-topology.md#angle) or changes in [angle](geometry-and-topology.md#angle). The PS-2120A uses interruptions of a [light](optics.md#light) beam to encode shaft motion; its product specification gives 4000 divisions per revolution. That count is a resolution specification, not a guarantee of the precision of an inferred [angular acceleration](#angular-acceleration) or [moment of inertia](#moment-of-inertia). [PASPORT Rotary Motion Sensor - PS-2120A](physics-bibliography.md#pasport-rotary-motion-sensor-ps-2120a)

#### Tensor parallel-axis theorem

↑ **Parent:** [Inertia tensor](#inertia-tensor)

If $G$ is the [center of mass](classical-mechanics.md#center-of-mass) and $X=P-G$, expanding the defining [inertia tensor](#inertia-tensor) about $P$ gives the displayed formula. The cross terms vanish because $\int r\,dm=0$ in coordinates centred at $G$. Contracting with a unit axis $u$ gives the [parallel axis theorem](#parallel-axis-theorem), with the squared distance between the parallel axes equal to $|X|^2-(u\cdot X)^2$.

#### Principal moment of inertia

↑ **Parent:** [Inertia tensor](#inertia-tensor)

The [principal moments of inertia](#principal-moment-of-inertia) about a specified point $O$ are the [eigenvalues](linear-operator-theory.md#eigenvalue) $I_1,I_2,I_3$ of the [inertia tensor](#inertia-tensor) $\mathbf I_O$. Their associated [unit vectors](vector-space.md#unit-vector) that are [eigenvectors](linear-operator-theory.md#eigenvector) specify [principal axes](#principal-axis) through $O$. The [spectral theorem for real symmetric matrices](linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) guarantees an [orthonormal basis](inner-product.md#orthonormal-basis) of these [eigenvectors](linear-operator-theory.md#eigenvector), even for an irregular [rigid body](rigid-body-dynamics.md). Choose their signs to make a right-handed basis and collect them as the columns of an [orthogonal matrix](linear-algebra.md#orthogonal-matrix) $Q$:

$$
\mathbf I_O\mathbf e_i=I_i\mathbf e_i,
\qquad Q^T\mathbf I_OQ=\operatorname{diag}(I_1,I_2,I_3).
$$

Thus [diagonalization](linear-operator-theory.md#diagonalization-of-a-matrix) removes the off-diagonal coupling in the [rotational kinetic energy](energy.md#rotational-kinetic-energy). The [eigenvalues](linear-operator-theory.md#eigenvalue) belong to the [mass](classical-mechanics.md#mass) distribution and reference point, independently of which [orthonormal basis](inner-product.md#orthonormal-basis) initially describes them. [Principal Axes of Rotation](physics-bibliography.md#newtonian-dynamics-by-richard-fitzpatrick/principal-axes-of-rotation)

In this [principal body frame](#principal-body-frame), write [angular velocity](#angular-velocity) as $\boldsymbol\omega=\sum_i\omega_i\mathbf e_i$. Then

$$
\mathbf L_O=\sum_i I_i\omega_i\mathbf e_i,
\qquad
K=\frac12\sum_i I_i\omega_i^2.
$$

Use these as total [angular momentum](momentum.md#angular-momentum) and [kinetic energy](energy.md#kinetic-energy) only under the reference-point conditions stated under [inertia tensor](#inertia-tensor). Along a single [principal axis](#principal-axis) with $I_i>0$, [angular momentum](momentum.md#angular-momentum) is parallel to [angular velocity](#angular-velocity). For a mixture of directions with different [principal moments of inertia](#principal-moment-of-inertia), it generally is not. A [principal axis](#principal-axis) need not be a geometric symmetry axis: it is selected by the complete [mass](classical-mechanics.md#mass) distribution. A [principal axis](#principal-axis) also need not give stable free rotation; for three distinct [principal moments of inertia](#principal-moment-of-inertia), the [intermediate axis theorem](#intermediate-axis-theorem) supplies the stability distinction.

For any [unit vector](vector-space.md#unit-vector) $\mathbf n=\sum_i n_i\mathbf e_i$,

$$
I_{O,\mathbf n}=\sum_i I_i n_i^2,
\qquad \sum_i n_i^2=1,
\qquad \min_i I_i\leq I_{O,\mathbf n}\leq\max_i I_i.
$$

The axial [moment of inertia](#moment-of-inertia) is a weighted average of the [principal moments of inertia](#principal-moment-of-inertia). At fixed [angular speed](#angular-speed), the least and greatest [rotational kinetic energies](energy.md#rotational-kinetic-energy) occur in the corresponding [eigenspaces](linear-operator-theory.md#eigenspace). At fixed nonzero [angular momentum](momentum.md#angular-momentum) magnitude $L$, instead, $K=\tfrac12\sum_i L_i^2/I_i$, so the largest [principal moment of inertia](#principal-moment-of-inertia) gives the smallest [rotational kinetic energy](energy.md#rotational-kinetic-energy). These comparisons hold the reference point fixed.

There is an additional physical restriction beyond [positive semidefiniteness](quadratic-form.md#positive-semidefinite-matrix). In [principal axes](#principal-axis) coordinates,

$$
I_1+I_2-I_3=2\int z^2\,dm\geq0,
$$

with two analogous cyclic inequalities. Therefore three arbitrary positive numbers do not always represent a possible [inertia tensor](#inertia-tensor). For a distribution in the $xy$ plane through $O$, $I_3=I_1+I_2$, as in the planar [inertia tensor of paired point masses](#inertia-tensor-of-paired-point-masses). A uniform solid [ellipsoid](euclidean-geometry.md#ellipsoid) of [mass](classical-mechanics.md#mass) $M$ and semiaxes $a,b,c$ supplies a continuous three-dimensional example: using its [mass second-moment tensor](#mass-second-moment-tensor), its central [principal moments of inertia](#principal-moment-of-inertia) are $M(b^2+c^2)/5$, $M(a^2+c^2)/5$, $M(a^2+b^2)/5$. Setting $a=b=c=R$ recovers the [moment of inertia of a uniform solid sphere](#moment-of-inertia-of-a-uniform-solid-sphere).

##### Rotational energy ellipsoid

↑ **Parent:** [Principal moment of inertia](#principal-moment-of-inertia)

For strictly positive [principal moments of inertia](#principal-moment-of-inertia) and a fixed [rotational kinetic energy](energy.md#rotational-kinetic-energy) $K_0>0$, the allowed [angular velocity](#angular-velocity) components form an [ellipsoid](euclidean-geometry.md#ellipsoid):

$$
I_1\omega_1^2+I_2\omega_2^2+I_3\omega_3^2=2K_0,
\qquad
s_i=\sqrt{\frac{2K_0}{I_i}}.
$$

Its semiaxis lengths $s_i$ have units of [angular speed](#angular-speed). The longest semiaxis corresponds to the smallest [principal moment of inertia](#principal-moment-of-inertia): that direction permits the greatest [angular speed](#angular-speed) for the same [rotational kinetic energy](energy.md#rotational-kinetic-energy). This is a surface in [angular velocity](#angular-velocity) space, not the physical outline of the body. If one [principal moment of inertia](#principal-moment-of-inertia) vanishes in an ideal line-mass model, this constant-energy surface is unbounded in that direction and is no longer an [ellipsoid](euclidean-geometry.md#ellipsoid).

<a id="image-principal-axes-and-the-constant-rotational-kinetic-energy-ellipsoid"></a>
![](inertia-tensor-principal-axis-energy-ellipsoid.png)

**[Figure 5](#image-principal-axes-and-the-constant-rotational-kinetic-energy-ellipsoid). Principal axes and the constant-rotational kinetic energy ellipsoid**. Original exact model using the six [point masses](classical-mechanics.md#point-mass) in [inertia tensor of paired point masses](#inertia-tensor-of-paired-point-masses). With $K_0=ma^2\Omega_0^2$, the displayed surface in $\boldsymbol\omega/\Omega_0$ has semiaxes $\sqrt{2/(9-\sqrt{13})}$, $\sqrt{2/(9+\sqrt{13})}$ and $\sqrt{2/14}$. The left view uses the original coordinate directions and the right view the [principal body frame](#principal-body-frame). Colors identify the same [principal axes](#principal-axis) in both views; the surface describes possible [angular velocities](#angular-velocity), not a material shell or a measured trajectory.

The [rotational energy ellipsoid](#rotational-energy-ellipsoid) gives the geometry behind [Poinsot's ellipsoid](#poinsot-s-ellipsoid), but a constant-energy surface alone does not determine a free-rotation trajectory. A torque-free trajectory must also satisfy the conserved [angular momentum](momentum.md#angular-momentum) constraint and the [Euler equations for a torque-free rigid body](#euler-equations-for-a-torque-free-rigid-body).

##### Degeneracy of principal moments of inertia

↑ **Parent:** [Principal moment of inertia](#principal-moment-of-inertia)

If two [principal moments of inertia](#principal-moment-of-inertia) coincide, for example $I_1=I_2\ne I_3$, every direction in their two-dimensional [eigenspace](linear-operator-theory.md#eigenspace) is a [principal axis](#principal-axis). The perpendicular axis is determined, but there is no privileged orthogonal pair within that plane. Rotating the pair in the plane leaves the diagonal [inertia tensor](#inertia-tensor) unchanged. If all three [principal moments of inertia](#principal-moment-of-inertia) coincide, $\mathbf I_O=I_0\mathbf1$ and every axis through $O$ is principal. This follows from the [eigenvalue multiplicity](linear-operator-theory.md#eigenvalue-multiplicity) and [eigenspace](linear-operator-theory.md#eigenspace), rather than from a failure of [diagonalization](linear-operator-theory.md#diagonalization-of-a-matrix). [Matrix Eigenvalue Theory](physics-bibliography.md#newtonian-dynamics-by-richard-fitzpatrick/matrix-eigenvalue-theory)

Equal [principal moments of inertia](#principal-moment-of-inertia) do not prove that a body's outline has continuous rotational symmetry. For example, six equal [point masses](classical-mechanics.md#point-mass) at $(\pm a,0,0)$, $(0,\pm a,0)$ and $(0,0,\pm a)$ have $\mathbf I_O=4ma^2\mathbf1$. This discrete layout has the same axial [moment of inertia](#moment-of-inertia) in every direction, although its actual [mass](classical-mechanics.md#mass) distribution changes under most rotations. Conversely, even when all three [principal moments of inertia](#principal-moment-of-inertia) are distinct, [principal axes](#principal-axis) are unoriented lines: reversing an [eigenvector](linear-operator-theory.md#eigenvector)'s sign gives the same axis. Near repeated [eigenvalues](linear-operator-theory.md#eigenvalue), small measurement errors can rotate fitted [principal axes](#principal-axis) substantially within the nearly degenerate [eigenspace](linear-operator-theory.md#eigenspace), so quoted directions need an uncertainty assessment as well as quoted [principal moments of inertia](#principal-moment-of-inertia).

<h4 id="poinsot-s-ellipsoid">Poinsot's ellipsoid</h4>

↑ **Parent:** [Inertia tensor](#inertia-tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poinsot's_ellipsoid)

For torque-free rigid-body motion, the kinetic-energy ellipsoid fixed in the body rolls without slipping on the invariable plane perpendicular to the conserved angular momentum. Its point of contact is the angular-velocity vector.

##### Herpolhode

↑ **Parent:** [Poinsot's ellipsoid](#poinsot-s-ellipsoid)

The [herpolhode](#herpolhode) is the contact curve traced on the fixed invariable plane in Poinsot's torque-free construction. It is distinct from the [polhode](#polhode), which is described in body coordinates.

##### Polhode

↑ **Parent:** [Poinsot's ellipsoid](#poinsot-s-ellipsoid)

The [polhode](#polhode) is the contact curve traced on the body's [energy](energy.md) [ellipsoid](euclidean-geometry.md#ellipsoid) during Poinsot's torque-free rolling construction.

### Parallel axis theorem

↑ **Parent:** [Moment of inertia](#moment-of-inertia)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parallel_axis_theorem)

The [parallel axis theorem](#parallel-axis-theorem) transfers a [moment of inertia](#moment-of-inertia) from an axis through the [centre of mass](classical-mechanics.md#center-of-mass) $G$ to a parallel axis through $O$:

$$
I_O=I_G+Md^2.
$$

Here $M$ is the total [mass](classical-mechanics.md#mass) and $d$ is the shortest perpendicular distance between the two axes. Both [moments of inertia](#moment-of-inertia) concern the same [mass](classical-mechanics.md#mass) distribution and the same axis direction. The axis for $I_G$ must pass through the [centre of mass](classical-mechanics.md#center-of-mass); $I_O$ may refer to an axis outside the body. No uniform-density or planar-shape assumption is needed. Within any family of parallel axes, the [centre of mass](classical-mechanics.md#center-of-mass) axis minimizes the [moment of inertia](#moment-of-inertia).[§10.5](physics-bibliography.md#university-physics-volume-1-by-william-moebs-and-others/10-5-calculating-moments-of-inertia)

A short proof isolates why the [centre of mass](classical-mechanics.md#center-of-mass) matters. Choose parallel axes perpendicular to an $xy$ plane, put $G$ at the origin, and place $O$ at $(d,0)$. Then

$$
I_O=\int\bigl[(x-d)^2+y^2\bigr]\,dm
=I_G-2d\int x\,dm+d^2\int dm
=I_G+Md^2,
$$

because $\int x\,dm=0$ in [centre of mass](classical-mechanics.md#center-of-mass) coordinates. Individual [mass](classical-mechanics.md#mass) elements can move closer to the new axis, but their weighted cross terms cancel. For arbitrary parallel axes $A$ and $B$, use $I_B-I_A=M(d_B^2-d_A^2)$, where each distance is measured from the parallel [centre of mass](classical-mechanics.md#center-of-mass) axis; adding $M$ times the squared separation of $A$ and $B$ is generally incorrect. A displacement along the axis has $d=0$. Changing the axis direction instead requires the [inertia tensor](#inertia-tensor) or, in its applicable planar setting, the [perpendicular axis theorem](#perpendicular-axis-theorem).

For a uniform disc, [mass](classical-mechanics.md#mass) $M$ and radius $R$, the central perpendicular [moment of inertia](#moment-of-inertia) is $I_G=MR^2/2$. Shifting that axis to the rim gives $d=R$ and $I_O=3MR^2/2$, three times $I_G$. In the computed $M=2\,\mathrm{kg}$, $R=0.30\,\mathrm m$ example, $I_G=0.090\,\mathrm{kg\,m^2}$, $Md^2=0.180\,\mathrm{kg\,m^2}$ and $I_O=0.270\,\mathrm{kg\,m^2}$. At [angular speed](#angular-speed) $10\,\mathrm{rad/s}$ the rim-pivoted disc has [rotational kinetic energy](energy.md#rotational-kinetic-energy) $13.5\,\mathrm J$. Its [centre of mass](classical-mechanics.md#center-of-mass) now moves, so $\tfrac12I_O\omega^2$ already includes that translation; adding a separate [centre of mass](classical-mechanics.md#center-of-mass) translation term to it would count that contribution twice.

<a id="image-parallel-axis-theorem-a-uniform-disc-s-central-and-rim-axes"></a>
![](rotational-inertia-energy-parallel-axis-shift.png)

**[Figure 6](#image-parallel-axis-theorem-a-uniform-disc-s-central-and-rim-axes). Parallel axis theorem: a uniform disc's central and rim axes**. Original geometric and numerical model, not measured data. Both axes are perpendicular to the disc; the separation is $d=R$. The bar chart separates $I_G=MR^2/2$ from the additional $Md^2=MR^2$ in $I_O=3MR^2/2$, normalized by $MR^2$. All parts of the disc remain in the calculation, including those nearer to the shifted axis.

The [physical pendulum](mathematical-physics.md#physical-pendulum) measurement described under [moment of inertia](#moment-of-inertia) provides a practical check: infer $I_O=Mgh(P/2\pi)^2$ at several pivot positions, then subtract $Mh^2$ to obtain $I_G$. Keep all pivot axes parallel and measure $h$ to the [centre of mass](classical-mechanics.md#center-of-mass) of the entire moving assembly. The same assembly should yield the same $I_G$ within measurement precision. If a smartphone is attached, its [mass](classical-mechanics.md#mass) and its own [moment of inertia](#moment-of-inertia) belong in both the geometric prediction and the [centre of mass](classical-mechanics.md#center-of-mass) calculation. The published bar-and-phone study explicitly adds both contributions using the [parallel axis theorem](#parallel-axis-theorem).[equations 2-4](physics-bibliography.md#experimental-analysis-of-a-physical-pendulum-with-variable-suspension-point-by-martin-monteiro-and-others)

For a careful replication, release small swings without a push, repeat timings at several small [amplitudes](wave.md#wave-amplitude), and check that the extrapolated [oscillation period](classical-mechanics.md#period-of-an-oscillation) is stable as [amplitude](wave.md#wave-amplitude) decreases. Time many complete [oscillations](wave.md#oscillation) and repeat the run; two crossings of a photogate per cycle must not be mistaken for two cycles. Inspect decay of [amplitude](wave.md#wave-amplitude) and compare early and late timings to detect significant pivot [friction](newtonian-mechanics.md#friction) or air [drag](fluid-mechanics.md#drag-physics). Mark the bar and phone mount to detect relative slip, tighten the attachment, and check that the pivot support does not rock or migrate between holes. Repeat with an independent photogate or video readout to check the phone's timing. These are proposed controls for the replication, not additional results reported by the authors. The ideal model excludes appreciable [damping](wave-equation.md#damping), large swings and flexing; subtraction of $Mh^2$ also magnifies relative errors when $I_G$ is much smaller than $I_O$.

The [oscillation period](classical-mechanics.md#period-of-an-oscillation) need not increase monotonically with pivot distance: the shift raises the [moment of inertia](#moment-of-inertia) but also increases the gravitational restoring [torque](momentum.md#torque). For a computed slender uniform bar model of length $L$, $I_G=ML^2/12$ and

$$
\frac{P^2}{4\pi^2}=\frac1g\left(h+\frac{L^2}{12h}\right),
\qquad h>0.
$$

This expression has its minimum at $h=L/\sqrt{12}$. With $L=1\,\mathrm m$, $h=0.50\,\mathrm m$ and stipulated $g=9.81\,\mathrm{m/s^2}$, the prediction is $P\simeq1.638\,\mathrm s$; it is not a recorded timing or a prediction for the bar with a phone attached. The competing terms explain why a timing experiment can reveal a [mass](classical-mechanics.md#mass) distribution rather than merely its weight.

#### Tangent-axis inertia of a spherical shell

↑ **Parent:** [Parallel axis theorem](#parallel-axis-theorem)

For uniform [density](fluid-mechanics.md#density) between concentric radii $R_1,R_2$, subtract the missing solid core's central [moment of inertia](#moment-of-inertia) and then shift the axis by $R_2$. Here $M=4\pi\rho(R_2^3-R_1^3)/3$. The thin-shell limit gives $I=5MR_2^2/3$, while a full solid sphere gives $7MR_2^2/5$.

### Perpendicular axis theorem

↑ **Parent:** [Moment of inertia](#moment-of-inertia)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perpendicular_axis_theorem)

For a planar lamina in the $xy$-plane, the moments about three mutually perpendicular axes through one point satisfy

$$
I_z=I_x+I_y.
$$

This follows pointwise from $x^2+y^2=y^2+x^2$ in the defining mass integrals.

### Angular rocket equation

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

For a uniformly filled, negligibly light disc of fixed radius $R$, remaining mass $m(t)$, angular velocity $\omega(t)$, and tangential exhaust speed $u$ relative to its rim, angular-momentum balance gives

$$
m\dot\omega=\dot m\left(\omega+\frac{2u}{R}\right).
$$

At zero relative exhaust speed, $\omega/m$ is constant.

### Moment of inertia of a solid cone about its vertex

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

For a uniform solid cone of height $l$, base radius $R$, and mass $M$, whose symmetry axis points from vertex to base, the centre of mass lies at $3l/4$ from the vertex. The principal moments at the vertex are

$$
I_1=I_2=\frac{3M}{20}(R^2+4l^2),
\qquad I_3=\frac{3MR^2}{10}.
$$

### Moment of inertia of a pointed cubic-profile solid of revolution

↑ **Parent:** [Moment of inertia](#moment-of-inertia)

Consider the uniform [solid of revolution](differential-geometry.md#solid-of-revolution) about the $x_3$-axis whose boundary is

$$
x_1^2+x_2^2=x_3^2-\frac{x_3^3}{h},
\qquad 0\leq x_3\leq h.
$$

For total mass $M$, the center of mass lies a distance $3h/5$ from the pointed origin, and the principal moments about that origin are

$$
I_1=I_2=\frac37Mh^2,
\qquad
I_3=\frac2{35}Mh^2.
$$

## Lagrange, Euler, and Kovalevskaya tops

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lagrange,_Euler,_and_Kovalevskaya_tops)

The [Lagrange, Euler, and Kovalevskaya tops](#lagrange-euler-and-kovalevskaya-tops) are three integrable cases of fixed-point [rigid body dynamics](rigid-body-dynamics.md). The Euler top has no external torque; the Lagrange top has axial symmetry and its center of mass on the symmetry axis; the Kovalevskaya top has two equal principal moments twice the third and its center of mass in the corresponding principal plane.

## Euler angles

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_angles)

[Euler angles](#euler-angles) describe the orientation of a [rigid body](rigid-body-dynamics.md) through three successive angular rotations. Their convention specifies the axes and order of the rotations. For a symmetric top, a common convention takes $\theta$ as the inclination, $\phi$ as precession and $\psi$ as spin about the body axis.

### Euler angles for a symmetric top

↑ **Parent:** [Euler angles](#euler-angles)

With the convention in which $\theta$ is inclination, $\phi$ is precession, and $\psi$ is body-axis spin, an axisymmetric body's kinetic energy is

$$
T=\frac I2(\dot\theta^2+\sin^2\theta\dot\phi^2)
+\frac J2(\dot\psi+\cos\theta\dot\phi)^2.
$$

#### Heavy symmetric top Lagrangian

↑ **Parent:** [Euler angles for a symmetric top](#euler-angles-for-a-symmetric-top)

For a fixed point a distance $a$ from the centre of mass and inclination measured from the upward vertical,

$$
L=T-Mga\cos\theta.
$$

The spin and precession angles are cyclic.

This is the Lagrangian of a [Lagrange top](#lagrange-top), one of the [Lagrange, Euler, and Kovalevskaya tops](#lagrange-euler-and-kovalevskaya-tops).

##### Lagrange top

↑ **Parent:** [Heavy symmetric top Lagrangian](#heavy-symmetric-top-lagrangian)

A Lagrange top is an axisymmetric rigid body with one point fixed on its symmetry axis, moving in a uniform gravitational field with its center of mass on that axis.

###### Steady precession of a Lagrange top

↑ **Parent:** [Lagrange top](#lagrange-top)

For a Lagrange top whose inclination $\theta$ is measured from the upward vertical, steady precession at angular speed $\Omega$ obeys

$$
I_1\Omega^2\cos\theta-p_\psi\Omega+Mgl=0.
$$

Thus steady precession at a prescribed $0<\theta<\pi/2$ exists precisely when

$$
p_\psi^2\geq4MglI_1\cos\theta.
$$

##### Heavy symmetric top Hamiltonian

↑ **Parent:** [Heavy symmetric top Lagrangian](#heavy-symmetric-top-lagrangian)

With transverse and axial moments $I,J$, the Hamiltonian is

$$
H=\frac{p_\theta^2}{2I}
+\frac{(p_\phi-p_\psi\cos\theta)^2}{2I\sin^2\theta}
+\frac{p_\psi^2}{2J}+Mga\cos\theta.
$$

###### Heavy symmetric top reduction

↑ **Parent:** [Heavy symmetric top Hamiltonian](#heavy-symmetric-top-hamiltonian)

Fixing the cyclic momenta $p_\psi=\lambda$ and $p_\phi=\mu$ leaves the canonical pair $(\theta,p_\theta)$ and a one-degree-of-freedom Hamiltonian with effective potential

$$
V_{\lambda,\mu}(\theta)
=\frac{(\mu-\lambda\cos\theta)^2}{2I\sin^2\theta}
+\frac{\lambda^2}{2J}+Mga\cos\theta.
$$

###### Gyroscopic stabilization of an inverted symmetric top

↑ **Parent:** [Heavy symmetric top reduction](#heavy-symmetric-top-reduction)

At the upright spinning state, $p_\phi=p_\psi=\lambda$. The reduced potential is locally minimized at zero inclination when

$$
\lambda^2>4IMga,
$$

so sufficiently large axial angular momentum stabilizes the gravitationally inverted top.

## Rolling without slipping

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rolling_without_slipping)

Rolling without slipping imposes that the contact point is instantaneously at rest, giving v=R omega.

### Rolling-cylinder loop contact threshold

↑ **Parent:** [Rolling without slipping](#rolling-without-slipping)

A solid cylinder rolling inside a circular loop has centre-path [radius](topology.md#radius) $\ell=R-a$, [kinetic energy](energy.md#kinetic-energy) $3mv^2/4$, and [speed](classical-mechanics.md#speed) $v^2=4g[h-\ell(1-\cos\theta)]/3$ at angle $\theta$ from the bottom. The normal contact [force](force.md) is smallest at the top. Requiring $v_t^2\ge g\ell$ gives the displayed necessary contact threshold under imposed no-slip rolling. The centre's maximum [acceleration](classical-mechanics.md#acceleration) on the circle is at the bottom, and at the threshold it is $11g/3$ upward. This is a limiting contact condition, not a guarantee for arbitrary finite [static friction](force.md#static-friction) or an unspecified approach curvature.

#### Finite-friction qualification of a marginal rolling loop

↑ **Parent:** [Rolling-cylinder loop contact threshold](#rolling-cylinder-loop-contact-threshold)

At the limiting release height for a solid cylinder, the loop [normal force](force.md#normal-force) is $N=(7mg/3)(1+\cos\theta)$ and the required static-friction magnitude is $mg|\sin\theta|/3$. Thus $|f|/N=|\sin\theta|/[7(1+\cos\theta)]$ diverges near the top, even though both [forces](force.md) vanish there. A finite [friction](newtonian-mechanics.md#friction) coefficient therefore requires a height above the ideal contact threshold to maintain no-slip rolling throughout. A question imposing rolling but giving no coefficient determines the ideal limiting bound, not a realistic friction-dependent minimum.

### Rolling constraint inside a moving circular track

↑ **Parent:** [Rolling without slipping](#rolling-without-slipping)

A circular body of radius $r$ rolls inside a circular track of radius $R$. Let $\theta$ be the track's material [rotation](riemannian-geometry.md#rotation-mathematics), $\phi$ the absolute angle of the line joining the two centres, and $\psi$ the inner body's absolute spin angle, all with one consistent orientation. Equating contact-point velocities gives the displayed constraint. [Translation](geometry-and-topology.md#translation-geometry) of the track's centre cancels from that equality. A stationary track gives $\dot\psi=-(R-r)\dot\phi/r$.

### Impulse-driven slipping-to-rolling transition of a sphere

↑ **Parent:** [Rolling without slipping](#rolling-without-slipping)

For a uniform sphere struck horizontally with [impulse](classical-mechanics.md#impulse) $J$ at height $d$ above its centre, $u_0=J/M$ and clockwise spin $\Omega_0=5Jd/(2Ma^2)$. [friction](newtonian-mechanics.md#friction) brings the contact slip $u-a\Omega$ to zero. The final rolling [speed](classical-mechanics.md#speed) is $u_f=5J(1+d/a)/(7M)$, independent of a positive constant [friction](newtonian-mechanics.md#friction) coefficient; [friction](newtonian-mechanics.md#friction) can accelerate an initially overspinning [centre of mass](classical-mechanics.md#center-of-mass).

#### Cue height for immediate rolling

↑ **Parent:** [Impulse-driven slipping-to-rolling transition of a sphere](#impulse-driven-slipping-to-rolling-transition-of-a-sphere)

For the ideal uniform solid sphere with negligible table [impulse](classical-mechanics.md#impulse) during the cue strike, immediate rolling requires $u_0=a\Omega_0$, hence the horizontal cue line lies $2a/5$ above the centre. A different inertia distribution changes this height.

### Ball bearing

↑ **Parent:** [Rolling without slipping](#rolling-without-slipping)

A [ball bearing](#ball-bearing) transfers loads through rolling spherical elements between two races. The no-slip conditions at both contacts determine the translation and spin of each ball; these are generally not the same [angular velocity](#angular-velocity).

#### Rolling ball between concentric races

↑ **Parent:** [Ball bearing](#ball-bearing)

If an inner race of radius $R$ rotates at [angular velocity](#angular-velocity) $\omega$ and an outer race is stationary, a ball of radius $r$ rolling at both contacts has centre speed $R\omega/2$ and spin $-R\omega/(2r)$. Its centre follows a circle of radius $R+r$. The [angular momentum](momentum.md#angular-momentum) about the common race axis includes both orbital [angular momentum](momentum.md#angular-momentum) and spin.

### Effective mass of a rolling rigid body

↑ **Parent:** [Rolling without slipping](#rolling-without-slipping)

For [rolling without slipping](#rolling-without-slipping) with contact radius $r$, substitute $\omega=v/r$ into translational plus rotational [kinetic energy](energy.md#kinetic-energy):

$$
T=\frac12Mv^2+\frac12I\omega^2=\frac12\left(M+\frac I{r^2}\right)v^2.
$$

The coefficient acts as an effective inertia for a translation coordinate. It is not additional gravitational [mass](classical-mechanics.md#mass). A quadratic [potential energy](energy.md#potential-energy) $Kx^2/2$ then gives small-oscillation frequency $\omega_0=\sqrt{K/M_{\rm eff}}$ when this coefficient is constant.

#### Pulley coupled to a rolling disc

↑ **Parent:** [Effective mass of a rolling rigid body](#effective-mass-of-a-rolling-rigid-body)

A hanging [mass](classical-mechanics.md#mass) $m$ pulls the centre of a uniform disc of [mass](classical-mechanics.md#mass) $M$ up an incline of angle $\theta$, using a light string and light frictionless pulley. If the disc rolls without slipping and the string is parallel to the slope, its effective translational [mass](classical-mechanics.md#mass) is $M+I/a^2=3M/2$. With downward hanging [acceleration](classical-mechanics.md#acceleration) $q$, $q=g(m-M\sin\theta)/(m+3M/2)$. [Static friction](force.md#static-friction) has signed downslope component $Mq/2$ and supplies the rolling [torque](momentum.md#torque). The [acceleration](classical-mechanics.md#acceleration) threshold is unchanged from a sliding block, although rotational inertia reduces the magnitude.

### Spring-mounted rolling cylinder

↑ **Parent:** [Rolling without slipping](#rolling-without-slipping)

Attach a [spring](elasticity-physics.md#spring) of [spring constant](elasticity-physics.md#spring-constant) $k$ to the axle of a round body of [mass](classical-mechanics.md#mass) $m$, radius $R$ and axial [moment of inertia](#moment-of-inertia) $I$. Assume [rolling without slipping](#rolling-without-slipping), a horizontal [drag force](fluid-mechanics.md#drag-physics) $-b\dot x$ applied through the axle, and no additional resisting [torque](momentum.md#torque). The translational [force](force.md) equation is $m\ddot x=-kx-b\dot x+f$, where $f$ is signed [static friction](force.md#static-friction). The rotational equation and rolling constraint give $f=-I\ddot x/R^2$, yielding the displayed equation. Equivalently, the [kinetic energy](energy.md#kinetic-energy) is $(m+I/R^2)\dot x^2/2$. This added effective inertia lowers the undamped [angular frequency](lagrangian-mechanics.md#angular-frequency) to $\sqrt{k/(m+I/R^2)}$. A distributed viscous [torque](momentum.md#torque) would add a separate damping term and cannot be inferred from the drag force alone.

### Rolling-time factor on a straight incline

↑ **Parent:** [Rolling without slipping](#rolling-without-slipping)

For a rigid body rolling from rest down a straight incline with fixed rolling radius $R$ and axial [moment of inertia](#moment-of-inertia) $I$, [translation](geometry-and-topology.md#translation-geometry) and [rotation](riemannian-geometry.md#rotation-mathematics) give $(M+I/R^2)\ddot s=Mg\sin\theta$. A smooth slide has $\ddot s=g\sin\theta$. Travel over the same distance from rest therefore gives the displayed time ratio. [Static friction](force.md#static-friction) must suffice for [rolling without slipping](#rolling-without-slipping); its contact point is at rest, so this ideal friction does no work. A uniform solid cylinder has $I=MR^2/2$ and ratio $\sqrt{3/2}$.

### Rolling uniform solid hemisphere

↑ **Parent:** [Rolling without slipping](#rolling-without-slipping)

Let the flat face make angle $\theta$ with horizontal while the rounded face contacts a horizontal plane. The centroid has height $a-(3a/8)\cos\theta$ and contact distance squared $b^2=a^2+(3a/8)^2-2a(3a/8)\cos\theta$. For [rolling without slipping](#rolling-without-slipping), its speed is $b|\dot\theta|$. Combining translation and rotation gives kinetic energy $\tfrac12(I_G+mb^2)\dot\theta^2$. Conservation from rest at $\theta=\pi/2$ gives the displayed result until the flat-face/contact geometry changes.

### Slipping solid cylinder on an incline

↑ **Parent:** [Rolling without slipping](#rolling-without-slipping)

For a uniform solid cylinder, take $s$ positive uphill and $\omega$ positive for uphill [rolling without slipping](#rolling-without-slipping). The velocity of the contact point is $w=\dot s-a\omega$. Uphill [kinetic friction](newtonian-mechanics.md#kinetic-friction) gives $\ddot s=-g(\sin\alpha-\mu\cos\alpha)$ and $a\dot\omega=-2\mu g\cos\alpha$. Starting from $\dot s(0)=a\omega(0)$, one obtains $w=-gt(\sin\alpha-3\mu\cos\alpha)$. Thus $\tan\alpha>3\mu$ makes the assumed uphill [kinetic friction](newtonian-mechanics.md#kinetic-friction) self-consistent for the entire ascent and descent. Without slip the required uphill [static friction](force.md#static-friction) is $mg\sin\alpha/3$; it is available exactly when $\tan\alpha\leq3\mu$ under the same limiting coefficient.

### Rolling inside a fixed circular cylinder

↑ **Parent:** [Rolling without slipping](#rolling-without-slipping)

A round body of radius $R_0$ in a fixed cylinder of radius $R_1$ has [center of mass](classical-mechanics.md#center-of-mass) path radius $a=R_1-R_0$. With orbital angle $\theta$ and spin [angular velocity](#angular-velocity) $\Omega$ both positive about the same axis, [rolling without slipping](#rolling-without-slipping) gives $a\dot\theta+R_0\Omega=0$. For [moment of inertia](#moment-of-inertia) $I=\gamma mR_0^2$, its [kinetic energy](energy.md#kinetic-energy) is $\frac12ma^2(1+\gamma)\dot\theta^2$. Release from rest at angle $\alpha$ gives, by [conservation of energy](mathematical-physics.md#conservation-of-energy), a descent time $\sqrt{1+\gamma}$ times that of frictionless sliding along the same [center of mass](classical-mechanics.md#center-of-mass) path. The spin sign reverses if its positive direction is chosen opposite to the orbital angle.

#### Small oscillations inside a circular cylinder

↑ **Parent:** [Rolling inside a fixed circular cylinder](#rolling-inside-a-fixed-circular-cylinder)

For [rolling without slipping](#rolling-without-slipping) inside a stationary circular cylinder, take the inner body's axial [moment of inertia](#moment-of-inertia) to be $I=\gamma mr^2$. Its [center of mass](classical-mechanics.md#center-of-mass) follows a circle of radius $d=R-r$, and the reduced [Lagrangian](calculus-of-variations.md#lagrangian) is $L=m(1+\gamma)d^2\dot\theta^2/2-mgd(1-\cos\theta)$. The [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) gives $(1+\gamma)d\ddot\theta+g\sin\theta=0$. Linearizing near the lowest position yields the displayed [small oscillation](lagrangian-mechanics.md#small-oscillation) frequency. A uniform solid cylinder has $\gamma=1/2$. This reduction requires sustained contact and enough [static friction](force.md#static-friction) to prevent slipping.

## Rigid body orientation

↑ **Parent:** [Rigid body dynamics](rigid-body-dynamics.md)

The rotational configuration of a [rigid body](rigid-body-dynamics.md) relative to a reference frame. In three dimensions, one marked direction leaves rotation about that direction undetermined.

## ↑ Ancestors (4)

1. [Classical mechanics](classical-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Lagrange, Euler, and Kovalevskaya tops](#lagrange-euler-and-kovalevskaya-tops)
