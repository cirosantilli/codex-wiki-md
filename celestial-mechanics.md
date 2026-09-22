# Celestial mechanics

↑ **Parent:** [Classical mechanics](classical-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Celestial_mechanics)

Celestial mechanics studies motion under gravitational forces.

**Table of contents**

- [Orbital speed](#orbital-speed)
- [Binary system](#binary-system)
- [Orbital energy](#orbital-energy)
- [Stellar orbit](#stellar-orbit)
- [Radial orbit time transformation](#radial-orbit-time-transformation)
  - [Angular reconstruction of a radial orbit transformation](#angular-reconstruction-of-a-radial-orbit-transformation)
  - [Kepler–isochrone radial transformation](#kepler-isochrone-radial-transformation)
    - [Attractive branch of the Kepler–isochrone transformation](#attractive-branch-of-the-kepler-isochrone-transformation)
  - [Kepler–harmonic radial duality](#kepler-harmonic-radial-duality)
- [Two-body problem](#two-body-problem)
  - [Equal-mass Coulomb circular orbit](#equal-mass-coulomb-circular-orbit)
  - [Laboratory paths of an equal-mass binary](#laboratory-paths-of-an-equal-mass-binary)
  - [Equal-mass circular binary](#equal-mass-circular-binary)
  - [Negative-energy gravitational collision](#negative-energy-gravitational-collision)
- [Kepler orbit](#kepler-orbit)
  - [Asymptotic minimum speed of an unbound Kepler orbit](#asymptotic-minimum-speed-of-an-unbound-kepler-orbit)
  - [Pericentre-speed qualification of Kepler orbit classes](#pericentre-speed-qualification-of-kepler-orbit-classes)
  - [Kepler velocity hodograph](#kepler-velocity-hodograph)
  - [Apsidal speed sum for an attractive inverse-square orbit](#apsidal-speed-sum-for-an-attractive-inverse-square-orbit)
  - [Velocity kick on a circular Kepler orbit](#velocity-kick-on-a-circular-kepler-orbit)
    - [Kick-orbit distribution](#kick-orbit-distribution)
  - [Kepler radial energy equation](#kepler-radial-energy-equation)
  - [Two-body orbital energy](#two-body-orbital-energy)
  - [Polar equation of a Kepler orbit](#polar-equation-of-a-kepler-orbit)
  - [Circumplanetary orbit](#circumplanetary-orbit)
    - [Planet-synchronous orbit](#planet-synchronous-orbit)
      - [Planet-stationary orbit](#planet-stationary-orbit)
    - [Radiation pressure on circumplanetary dust](#radiation-pressure-on-circumplanetary-dust)
      - [Shadowing of circumplanetary dust](#shadowing-of-circumplanetary-dust)
  - [Circumstellar orbit](#circumstellar-orbit)
  - [Binet equation](#binet-equation)
    - [Circular orbit through an inverse-fifth-power singularity](#circular-orbit-through-an-inverse-fifth-power-singularity)
    - [Orbit equation for combined inverse-square and inverse-cube attraction](#orbit-equation-for-combined-inverse-square-and-inverse-cube-attraction)
      - [Apsidal invariant on an unbound central-force branch](#apsidal-invariant-on-an-unbound-central-force-branch)
      - [Closed orbits with an inverse-cube perturbation](#closed-orbits-with-an-inverse-cube-perturbation)
      - [Inverse-cube perturbation of Kepler apsidal motion](#inverse-cube-perturbation-of-kepler-apsidal-motion)
        - [Inferring an inverse-cube perturbation from apsidal precession](#inferring-an-inverse-cube-perturbation-from-apsidal-precession)
    - [Inferring an inverse-square force from Kepler laws](#inferring-an-inverse-square-force-from-kepler-laws)
    - [Damped Binet equation](#damped-binet-equation)
      - [Circularization under radial inverse-square drag](#circularization-under-radial-inverse-square-drag)
    - [Shifted inverse-radius potential](#shifted-inverse-radius-potential)
  - [Orbital eccentricity](#orbital-eccentricity)
    - [Eccentricity vector](#eccentricity-vector)
      - [Perturbed Kepler-orbit conservation laws](#perturbed-kepler-orbit-conservation-laws)
    - [Thermal eccentricity distribution](#thermal-eccentricity-distribution)
      - [Delaunay phase-volume proof of the thermal eccentricity distribution](#delaunay-phase-volume-proof-of-the-thermal-eccentricity-distribution)
        - [Finite normalization of an energy-only Kepler distribution](#finite-normalization-of-an-energy-only-kepler-distribution)
  - [Elliptic orbit](#elliptic-orbit)
  - [Hyperbolic Kepler orbit](#hyperbolic-kepler-orbit)
    - [Gravitational scattering angle](#gravitational-scattering-angle)
      - [Non-colliding gravitational velocity-kick bound](#non-colliding-gravitational-velocity-kick-bound)
    - [Gravitational assist](#gravitational-assist)
  - [Parabolic trajectory](#parabolic-trajectory)
    - [Barker equation](#barker-equation)
      - [Radius-time relation for a parabolic Kepler orbit](#radius-time-relation-for-a-parabolic-kepler-orbit)
      - [Pericentre-to-crossover flight time](#pericentre-to-crossover-flight-time)
  - [Periapsis](#periapsis)
    - [Pericentre distance](#pericentre-distance)
  - [Apoapsis](#apoapsis)
    - [Apocentre distance](#apocentre-distance)
  - [Semi-major axis](#semi-major-axis)
  - [Semi-minor axis](#semi-minor-axis)
  - [Orbital element](#orbital-element)
    - [Radial-velocity semi-amplitude](#radial-velocity-semi-amplitude)
    - [Argument of periapsis](#argument-of-periapsis)
    - [True longitude](#true-longitude)
    - [Orbital plane](#orbital-plane)
    - [Osculating orbital element](#osculating-orbital-element)
      - [Astrocentric osculating-element oscillations](#astrocentric-osculating-element-oscillations)
    - [True anomaly](#true-anomaly)
    - [Orbital phase](#orbital-phase)
      - [Phase-mixed orbit](#phase-mixed-orbit)
        - [Line density on a Kepler orbit](#line-density-on-a-kepler-orbit)
          - [Cross-sectional-area current](#cross-sectional-area-current)
        - [Phase-mixed radial probability of a Kepler orbit](#phase-mixed-radial-probability-of-a-kepler-orbit)
    - [Mean anomaly](#mean-anomaly)
      - [Kepler's equation](#kepler-s-equation)
    - [Eccentric anomaly](#eccentric-anomaly)
    - [Orbital node](#orbital-node)
      - [Ascending node](#ascending-node)
        - [Longitude of ascending node](#longitude-of-ascending-node)
    - [Orbital inclination](#orbital-inclination)
      - [Orbital-frame rotation from inclination and node](#orbital-frame-rotation-from-inclination-and-node)
      - [Mutual inclination](#mutual-inclination)
        - [Mutual inclination of nearly edge-on orbits](#mutual-inclination-of-nearly-edge-on-orbits)
      - [Invariable plane](#invariable-plane)
        - [Inclination to the invariable plane of two orbital planes](#inclination-to-the-invariable-plane-of-two-orbital-planes)
      - [Edge-on orbit](#edge-on-orbit)
      - [Orbital-plane orientation degeneracy](#orbital-plane-orientation-degeneracy)
    - [Longitude of periapsis](#longitude-of-periapsis)
    - [Mean longitude](#mean-longitude)
    - [Mean motion](#mean-motion)
      - [Orbital period](#orbital-period)
        - [Low circular-orbit period measures mean density](#low-circular-orbit-period-measures-mean-density)
      - [Synodic period](#synodic-period)
  - [Specific orbital energy](#specific-orbital-energy)
    - [Orbit-averaged drag work](#orbit-averaged-drag-work)
    - [Vis-viva equation](#vis-viva-equation)
  - [Specific angular momentum](#specific-angular-momentum)
    - [High-eccentricity angular-speed crossover](#high-eccentricity-angular-speed-crossover)
    - [Periapsis angular speed](#periapsis-angular-speed)
  - [Circular Kepler orbit](#circular-kepler-orbit)
    - [Synchronous circular orbit](#synchronous-circular-orbit)
      - [Geostationary orbit](#geostationary-orbit)
  - [Hohmann transfer orbit](#hohmann-transfer-orbit)
    - [Reversed circularization burn in a Hohmann transfer](#reversed-circularization-burn-in-a-hohmann-transfer)
    - [Hohmann transfer impulse fractions](#hohmann-transfer-impulse-fractions)
    - [Hohmann transfer time](#hohmann-transfer-time)
- [Restricted three-body problem](#restricted-three-body-problem)
  - [Circular restricted three-body problem](#circular-restricted-three-body-problem)
    - [Hill equations](#hill-equations)
      - [Free solution of Hill equations](#free-solution-of-hill-equations)
        - [Orbital elements from Hill coordinates](#orbital-elements-from-hill-coordinates)
    - [Photogravitational restricted three-body problem](#photogravitational-restricted-three-body-problem)
    - [Lagrange point](#lagrange-point)
      - [Effective-potential geometry of Lagrange points](#effective-potential-geometry-of-lagrange-points)
      - [Collinear Lagrange point](#collinear-lagrange-point)
        - [Small-mass-ratio collinear Lagrange points](#small-mass-ratio-collinear-lagrange-points)
        - [Inner Lagrange point](#inner-lagrange-point)
        - [L2 Lagrange point](#l2-lagrange-point)
          - [Linearization at L2](#linearization-at-l2)
            - [L2 escape e-folding time](#l2-escape-e-folding-time)
        - [L3 Lagrange point](#l3-lagrange-point)
      - [Triangular Lagrange point](#triangular-lagrange-point)
    - [Hill sphere](#hill-sphere)
      - [Hill radius](#hill-radius)
        - [Mutual Hill radius](#mutual-hill-radius)
    - [Jacobi constant](#jacobi-constant)
- [Orbital resonance](#orbital-resonance)
  - [Mean-motion resonance](#mean-motion-resonance)
    - [Interior eccentricity-type mean-motion resonance](#interior-eccentricity-type-mean-motion-resonance)
    - [Inclination-type mean-motion resonance](#inclination-type-mean-motion-resonance)
    - [Exterior mean-motion resonance](#exterior-mean-motion-resonance)
      - [Resonant semi-major axis](#resonant-semi-major-axis)
      - [Radiation-pressure shift of a mean-motion resonance](#radiation-pressure-shift-of-a-mean-motion-resonance)
    - [First-order mean-motion resonance](#first-order-mean-motion-resonance)
      - [Resonance-overlap encounter estimate](#resonance-overlap-encounter-estimate)
    - [Resonant argument](#resonant-argument)
      - [Resonant conjunction geometry](#resonant-conjunction-geometry)
        - [Phase protection of interior integer resonances](#phase-protection-of-interior-integer-resonances)
        - [Conjunction-pattern precession near a mean-motion resonance](#conjunction-pattern-precession-near-a-mean-motion-resonance)
          - [Conjunction-longitude sensitivity to an encounter](#conjunction-longitude-sensitivity-to-an-encounter)
      - [Resonant-argument libration](#resonant-argument-libration)
        - [Pendulum approximation of a mean-motion resonance](#pendulum-approximation-of-a-mean-motion-resonance)
          - [Resonant pendulum energy](#resonant-pendulum-energy)
        - [Asymmetric resonant-argument libration](#asymmetric-resonant-argument-libration)
        - [Symmetric libration centres of an eccentricity resonance](#symmetric-libration-centres-of-an-eccentricity-resonance)
          - [Low-eccentricity correction to a first-order resonance center](#low-eccentricity-correction-to-a-first-order-resonance-center)
        - [Libration amplitude of a resonant argument](#libration-amplitude-of-a-resonant-argument)
        - [Resonance protection](#resonance-protection)
    - [Resonance capture](#resonance-capture)

## Orbital speed

↑ **Parent:** [Celestial mechanics](celestial-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orbital_speed)

Orbital [speed](classical-mechanics.md#speed) is the magnitude of the [velocity](classical-mechanics.md#velocity) of an orbiting body in a specified reference frame. For a Newtonian [circular orbit](classical-mechanics.md#circular-orbit) around a point source of [mass](classical-mechanics.md#mass) $M$, equating $v^2/r$ to $GM/r^2$ gives $v=\sqrt{GM/r}$. In a curved [spacetime](special-relativity.md#spacetime), a speed inferred from coordinate radius and coordinate time generally differs from a speed measured by a local observer. For a circular orbit in the [Schwarzschild metric](schwarzschild-spacetime.md), a static local observer measures $v_{\rm local}=r|d\phi/dt|/\sqrt{1-2GM/(c^2r)}$; $r|d\phi/dt|$ uses the clock normalization at infinity instead.

## Binary system

↑ **Parent:** [Celestial mechanics](celestial-mechanics.md)

Two objects orbiting their common [center of mass](classical-mechanics.md#center-of-mass) under their mutual [gravity](physics.md#gravity).

## Orbital energy

↑ **Parent:** [Celestial mechanics](celestial-mechanics.md)

## Stellar orbit

↑ **Parent:** [Celestial mechanics](celestial-mechanics.md)

## Radial orbit time transformation

↑ **Parent:** [Celestial mechanics](celestial-mechanics.md)

For a central-force radial [energy](energy.md) equation, choose a monotone radius $q=q(r)$ and clock $\tau$ such that $d\tau/dt=(q/r)dq/dr$. Then $q'=(r/q)\dot r$, and multiplying the old [energy](energy.md) equation by $r^2/q^2$ preserves the centrifugal form $L^2/(2q^2)$. A split of the remaining terms into constant [energy](energy.md) and a new [Newtonian gravitational potential](newton-s-law-of-universal-gravitation.md#newtonian-gravitational-potential) produces a transformed radial orbit.

### Angular reconstruction of a radial orbit transformation

↑ **Parent:** [Radial orbit time transformation](#radial-orbit-time-transformation)

A transformed radial equation containing $L^2/(2q^2)$ becomes a full planar central-force orbit by choosing $d\bar\theta/d\tau=L/q^2$. For $d\tau/dt=(q/r)dq/dr$ and old [angular velocity](rigid-body-dynamics.md#angular-velocity) $L/r^2$, this gives $d\bar\theta/d\theta=(r/q)dq/dr$. Keeping the old angle generally fails to preserve the stated transformed [angular momentum](momentum.md#angular-momentum).

<h3 id="kepler-isochrone-radial-transformation">Kepler–isochrone radial transformation</h3>

↑ **Parent:** [Radial orbit time transformation](#radial-orbit-time-transformation)

With $a=(1-\lambda)GM$, $h=\lambda E>0$ and $\bar E>0$, set $\bar E q^2=hr^2+ar$. If $a\geq0$, its positive-radius root is $r=\sqrt{\bar E/h}(\sqrt{q^2+b^2}-b)$, with $b=a/(2\sqrt{h\bar E})$. The transformed [Newtonian gravitational potential](newton-s-law-of-universal-gravitation.md#newtonian-gravitational-potential) is an additive constant plus $-G\bar M/(b+\sqrt{q^2+b^2})$, the [spherical isochrone model](galaxy.md#spherical-isochrone-model). The [mass](classical-mechanics.md#mass) sign and branch conditions must be checked.

<h4 id="attractive-branch-of-the-kepler-isochrone-transformation">Attractive branch of the Kepler–isochrone transformation</h4>

↑ **Parent:** [Kepler–isochrone radial transformation](#kepler-isochrone-radial-transformation)

For bound old [Kepler orbits](#kepler-orbit), $E<0$, $\lambda<0$ and $\bar E>0$ give a positive radius, positive isochrone scale $b$, and positive transformed [mass](classical-mechanics.md#mass). The shifted [energy](energy.md) is $\bar E-k=\bar E/\lambda<0$. For unbound old orbits with $E>0$, $1/2<\lambda\leq1$ gives an attractive unbound isochrone branch. The case $\lambda=0$ is handled by the separate [Kepler–harmonic radial duality](#kepler-harmonic-radial-duality).

<h3 id="kepler-harmonic-radial-duality">Kepler–harmonic radial duality</h3>

↑ **Parent:** [Radial orbit time transformation](#radial-orbit-time-transformation)

Taking $\bar E=GM\,r/q^2>0$ in a [radial orbit time transformation](#radial-orbit-time-transformation) gives $r=(\bar E/GM)q^2$ and $\bar\Phi(q)=-E(\bar E/GM)^2q^2$. Bound [Kepler orbits](#kepler-orbit) with $E<0$ map to a confining [harmonic oscillator](classical-mechanics.md#simple-harmonic-motion); positive [energy](energy.md) maps to an inverted oscillator. Full angular reconstruction halves the original orbital angle.

## Two-body problem

↑ **Parent:** [Celestial mechanics](celestial-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Two-body_problem)

The two-body problem determines the motion of two particles interacting only with one another. For a central force it separates into uniform centre-of-mass motion and one relative-coordinate problem with the reduced mass.

### Equal-mass Coulomb circular orbit

↑ **Parent:** [Two-body problem](#two-body-problem)

For two particles of equal [mass](classical-mechanics.md#mass) $m$ and opposite charges $\pm q$ separated by $s$, the [centre of mass](classical-mechanics.md#center-of-mass) lies halfway between them. In a nonradiating classical model, each radius is $s/2$ and $k_eq^2/s^2=m\omega^2s/2$. Hence $\omega^2=2k_eq^2/(ms^3)$ and $T=2\pi\sqrt{ms^3/(2k_eq^2)}$. Equivalently, relative motion has [reduced mass](classical-mechanics.md#reduced-mass) $m/2$. Radiation and quantum binding invalidate an indefinitely stable classical orbit for actual microscopic charges.

### Laboratory paths of an equal-mass binary

↑ **Parent:** [Two-body problem](#two-body-problem)

For equal masses and relative [position](classical-mechanics.md#position) $\mathbf r$, the individual positions are $\mathbf r_A=\mathbf R-\mathbf r/2$ and $\mathbf r_B=\mathbf R+\mathbf r/2$, where the [center of mass](classical-mechanics.md#center-of-mass) has uniform [velocity](classical-mechanics.md#velocity) in an isolated system. Bound [inverse-square force](classical-mechanics.md#inverse-square-force) motion makes $\mathbf r$ an [ellipse](euclidean-geometry.md#ellipse); each mass follows a half-size ellipse in the center-of-mass frame. Adding a nonzero center-of-mass drift generally makes their laboratory [trajectories](classical-mechanics.md#trajectory) nonclosed. The relative orbital period is not necessarily a period of either laboratory position.

### Equal-mass circular binary

↑ **Parent:** [Two-body problem](#two-body-problem)

Two equal point [masses](classical-mechanics.md#mass) can move around the same fixed circle of radius $a$ in diametrically opposite positions. Their stationary [centre of mass](classical-mechanics.md#center-of-mass) is the circle's center. A separation $2a$ gives gravitational [force](force.md) $Gm^2/(4a^2)$ on each [mass](classical-mechanics.md#mass), and [Newton's second law](force.md#newton-s-second-law) equates it to $ma\omega^2$. The common [angular speed](rigid-body-dynamics.md#angular-speed) is therefore fixed by the displayed relation. Opposite tangential [velocities](classical-mechanics.md#velocity) produce the same sense of angular rotation.

### Negative-energy gravitational collision

↑ **Parent:** [Two-body problem](#two-body-problem)

Two point [masses](classical-mechanics.md#mass) released from rest at separation $a$ have negative [mechanical energy](energy.md#mechanical-energy) $-Gm_1m_2/a$ but collide in time $\pi\sqrt{a^3/[8G(m_1+m_2)]}$. Their separation approaches zero along a regular trajectory before collision. The [energy](energy.md) sign alone therefore does not supply a positive lower separation bound.

## Kepler orbit

↑ **Parent:** [Celestial mechanics](celestial-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kepler_orbit)

An inverse-square central force produces conic-section trajectories with the force centre at a focus.

### Asymptotic minimum speed of an unbound Kepler orbit

↑ **Parent:** [Kepler orbit](#kepler-orbit)

For a positive-mass object in the inverse-square attractive field with potential zero at infinity, energy conservation gives $v^2(r)=2E/m+2GM/r$. Along the outgoing unbound branch, speed decreases toward the displayed limiting value. It is positive for a hyperbola and zero for a parabola. This is an infimum approached at infinite separation, not a finite-radius stopping point or the local [escape velocity](energy.md#escape-velocity).

### Pericentre-speed qualification of Kepler orbit classes

↑ **Parent:** [Kepler orbit](#kepler-orbit)

At a genuine [pericentre](#periapsis), the radial velocity vanishes and the radial acceleration is nonnegative. The radial equation therefore requires $v_p^2\ge GM/r_p$. In terms of the displayed factor k, a circle has k=1, a noncircular ellipse has $1<k<\sqrt2$, a parabola has $k=\sqrt2$ and a hyperbola has $k>\sqrt2$. If $0<k<1$ at a tangential turning point, that point is the apocentre, despite the negative orbital energy. Bound-energy classification alone does not establish which turning point is being specified.

### Kepler velocity hodograph

↑ **Parent:** [Kepler orbit](#kepler-orbit)

In axes directed along the [periapsis](#periapsis) and transverse to it, a [Kepler orbit](#kepler-orbit) with gravitational parameter $\mu_g$ and [specific angular momentum](#specific-angular-momentum) $h$ has the displayed [velocity](classical-mechanics.md#velocity). The [velocity](classical-mechanics.md#velocity) tip traces a circle of radius $\mu_g/h$ centred at $(0,e\mu_g/h)$. To derive it, differentiate $r=h^2/[\mu_g(1+e\cos f)]$, use $r^2\dot f=h$, and resolve $\dot r\widehat{\boldsymbol r}+r\dot f\widehat{\boldsymbol\theta}$. A rotation of the spatial axes rotates the entire hodograph by the same angle.

### Apsidal speed sum for an attractive inverse-square orbit

↑ **Parent:** [Kepler orbit](#kepler-orbit)

For unit mass with [inverse-square potential](energy.md#inverse-square-potential) $-Q/r$, $Q>0$, and positive conserved [angular momentum](momentum.md#angular-momentum) $h$, a bounded orbit has $-Q^2/(2h^2)\le E<0$. Its [periapsis distance](#pericentre-distance) and [apoapsis distance](#apocentre-distance) are roots of $|E|r^2-Qr+h^2/2=0$, so their sum is $Q/|E|$ and product $h^2/(2|E|)$. Speed is largest at the [periapsis](#periapsis) and smallest at the [apoapsis](#apoapsis), because $v^2=2(E+Q/r)$ decreases with $r$. Radial velocity is zero there, so the two speeds are $h/r_{\min}$ and $h/r_{\max}$. Their sum is $h(r_{\min}+r_{\max})/(r_{\min}r_{\max})=2Q/h$, independent of $E$, including the circular limit.

### Velocity kick on a circular Kepler orbit

↑ **Parent:** [Kepler orbit](#kepler-orbit)

For an instantaneous in-plane change of [velocity](classical-mechanics.md#velocity) of magnitude $\gamma v_K$ on a [circular orbit](classical-mechanics.md#circular-orbit), with angle $\theta$ measured from the forward tangential direction, the new [specific orbital energy](#specific-orbital-energy) gives $a'/a=(1-2\gamma\cos\theta-\gamma^2)^{-1}$. The [specific angular momentum](#specific-angular-momentum) gives $e'^2=1-(1-2\gamma\cos\theta-\gamma^2)(1+\gamma\cos\theta)^2$. The signed [semi-major axis](#semi-major-axis) becomes negative for an unbound [hyperbolic Kepler orbit](#hyperbolic-kepler-orbit).

#### Kick-orbit distribution

↑ **Parent:** [Velocity kick on a circular Kepler orbit](#velocity-kick-on-a-circular-kepler-orbit)

Uniform planar kick angle $\theta$ gives $c=\cos\theta$ with probability density $1/(\pi\sqrt{1-c^2})$. This maps onto a one-dimensional curve in [orbital eccentricity](#orbital-eccentricity)–[semi-major axis](#semi-major-axis) space. The two radial-kick signs share that curve but have opposite tangential components of the [eccentricity vector](#eccentricity-vector). The resulting density is enhanced near tangential-kick endpoints.

### Kepler radial energy equation

↑ **Parent:** [Kepler orbit](#kepler-orbit)

For unit [mass](classical-mechanics.md#mass) in $\Phi=-GM/r$, [conservation of angular momentum](momentum.md#conservation-of-angular-momentum) splits the [velocity](classical-mechanics.md#velocity) norm into $\dot r^2+L^2/r^2$. [Conservation of energy](mathematical-physics.md#conservation-of-energy) then gives $\tfrac12\dot r^2+L^2/(2r^2)=E+GM/r$. It separates radial dynamics from the reconstruction of the orbital angle.

### Two-body orbital energy

↑ **Parent:** [Kepler orbit](#kepler-orbit)

In the centre-of-mass frame of two Newtonian point masses, total orbital energy is reduced mass times [specific orbital energy](#specific-orbital-energy): $E=\mu[|\dot{\mathbf r}|^2/2-GM/r]$. The factor $\mu$ multiplies both kinetic and potential contributions, while $GM$ is the relative gravitational parameter.

### Polar equation of a Kepler orbit

↑ **Parent:** [Kepler orbit](#kepler-orbit)

For an attractive [inverse-square force](classical-mechanics.md#inverse-square-force), $r=p/(1+e\cos f)$, where $f$ is [true anomaly](#true-anomaly), $e$ is [orbital eccentricity](#orbital-eccentricity), and $p=h^2/\mu$ is the semilatus rectum. The [specific angular momentum](#specific-angular-momentum) relation $\dot f=h/r^2$ converts this geometric equation into an angular evolution law.

### Circumplanetary orbit

↑ **Parent:** [Kepler orbit](#kepler-orbit)

An [orbit](dynamical-systems.md#orbit-dynamical-system) about a [planet](planetary-science.md#planet). Stellar tides, [radiation pressure](pressure.md#radiation-pressure) and other perturbations can limit its stability; a sufficiently small [semi-major axis](#semi-major-axis) compared with the [Hill sphere](#hill-sphere) permits a local approximately planet-centred [Kepler orbit](#kepler-orbit).

#### Planet-synchronous orbit

↑ **Parent:** [Circumplanetary orbit](#circumplanetary-orbit)

A [circumplanetary orbit](#circumplanetary-orbit) whose [orbital period](#orbital-period) equals the central planet's spin period. Its [semi-major axis](#semi-major-axis) follows from [Kepler's third law](mathematical-physics.md#kepler-s-third-law). Matching periods alone does not fix the satellite above one ground location; that additionally requires a [planet-stationary orbit](#planet-stationary-orbit).

##### Planet-stationary orbit

↑ **Parent:** [Planet-synchronous orbit](#planet-synchronous-orbit)

A prograde, equatorial [circular orbit](classical-mechanics.md#circular-orbit) with [orbital period](#orbital-period) equal to the planet's spin period. In the ideal model its satellite remains above one equatorial ground location. Nonzero [orbital inclination](#orbital-inclination) or [orbital eccentricity](#orbital-eccentricity) destroys exact stationarity even when the periods agree.

#### Radiation pressure on circumplanetary dust

↑ **Parent:** [Circumplanetary orbit](#circumplanetary-orbit)

The leading uniform stellar [radiation pressure](pressure.md#radiation-pressure) is a differential [acceleration](classical-mechanics.md#acceleration) relative to a [planet](planetary-science.md#planet), of scale $\beta GM_\star/a_p^2$. Relative to planetocentric gravity at dust radius $a$, its magnitude is

$$
\eta_{\rm rad}=\beta\frac{M_\star}{M_p}\left(\frac a{a_p}\right)^2.
$$

Thus lying inside a [Hill sphere](#hill-sphere) alone does not guarantee small radiative perturbations. Approximately circular tightly bound dust requires this ratio sufficiently small, as well as weak tides; the uniform radiative [force](force.md) can otherwise excite [orbital eccentricity](#orbital-eccentricity) or unbind grains.

##### Shadowing of circumplanetary dust

↑ **Parent:** [Radiation pressure on circumplanetary dust](#radiation-pressure-on-circumplanetary-dust)

A [planet](planetary-science.md#planet) can block stellar radiation during part of a [circumplanetary orbit](#circumplanetary-orbit). Then the full-orbit constant-flux averages for [radiation pressure](pressure.md#radiation-pressure) and [Poynting–Robertson drag](planetary-science.md#poynting-robertson-drag) require modification. The detailed shadow duty cycle depends on the [orbital inclination](#orbital-inclination), stellar angular extent and dust radius.

### Circumstellar orbit

↑ **Parent:** [Kepler orbit](#kepler-orbit)

An [orbit](dynamical-systems.md#orbit-dynamical-system) about a [star](stellar-astrophysics.md#star). Dust on such an [orbit](dynamical-systems.md#orbit-dynamical-system) can experience [radiation pressure](pressure.md#radiation-pressure) and [Poynting–Robertson drag](planetary-science.md#poynting-robertson-drag), in addition to gravitational perturbations.

### Binet equation

↑ **Parent:** [Kepler orbit](#kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binet_equation)

Binet’s equation rewrites a central-force orbit using $u(\theta)=1/r$. If $\ell=mr^2\dot\theta$ is angular momentum and the potential is $V(r)$, then

$$
u''+u=\frac{m}{\ell^2u^2}\frac{dV}{dr}\bigg|_{r=1/u}.
$$

#### Circular orbit through an inverse-fifth-power singularity

↑ **Parent:** [Binet equation](#binet-equation)

For an attractive [central force](mathematical-physics.md#central-force) of magnitude $c/r^5$, a circle of radius $R$ through the force center has polar equation $r=2R\cos\theta$. With [specific angular momentum](#specific-angular-momentum) $h$, substitution into the [Binet equation](#binet-equation) gives $c=8mh^2R^2$. Consequently $R$ is inversely proportional to the magnitude of the [angular momentum](momentum.md#angular-momentum), and the angular-time integral gives $T=2\pi R^2/|h|\propto R^3$. This is the finite travel time along the punctured circle from one approach to the singular center to the next; the force law alone does not specify continuation through the collision.

#### Orbit equation for combined inverse-square and inverse-cube attraction

↑ **Parent:** [Binet equation](#binet-equation)

For radial acceleration $-A/r^2-B/r^3$, conserved [specific angular momentum](#specific-angular-momentum) $l$ and $u=1/r$ reduce the [Binet equation](#binet-equation) to the displayed linear equation. If $l^2>B$, its angular oscillation frequency is $\sqrt{1-B/l^2}$; attraction proportional to $r^{-3}$ changes the apsidal angle. A zero of $u$ ends the physical positive-radius branch and corresponds to escape, not passage to a negative radius. A spatial self-intersection need not be a periodic return because [velocity](classical-mechanics.md#velocity) may differ.

##### Apsidal invariant on an unbound central-force branch

↑ **Parent:** [Orbit equation for combined inverse-square and inverse-cube attraction](#orbit-equation-for-combined-inverse-square-and-inverse-cube-attraction)

For $u=u_c[1+e\cos\nu(\psi-\psi_0)]$ with $\nu>0$ and $e\geq1$, the positive-radius scattering branch has $|\nu(\psi-\psi_0)|<\arccos(-1/e)\leq\pi$. Thus the principal complex argument in the displayed expression is continuous throughout that branch, unlike at an apocentre of a bound orbit. Its derivative is $\nu$, so the angle modulo $2\pi$, or the associated unit apsidal vector in the orbital plane, is a stationary [integral of motion](hamiltonian-mechanics.md#integral-of-motion) fixing the periapsis direction. Together with energy and three components of [specific angular momentum](#specific-angular-momentum), it gives five regular scattering labels even for irrational $\nu$. Periodicity is therefore necessary for five orbit labels in recurrent bound motion, not in general for escaping trajectories.

##### Closed orbits with an inverse-cube perturbation

↑ **Parent:** [Orbit equation for combined inverse-square and inverse-cube attraction](#orbit-equation-for-combined-inverse-square-and-inverse-cube-attraction)

In the [gravitational potential](newton-s-law-of-universal-gravitation.md#newtonian-potential-of-a-point-mass) $-\mu(1/r+a/r^2)$, a regular noncircular bound [orbit](dynamical-systems.md#orbit-dynamical-system) requires $L^2>2\mu a$ and has $u=\mu(L^2-2\mu a)^{-1}[1+e\cos\nu(\psi-\psi_0)]$ with $0<e<1$. Each radial period advances the angle by $2\pi/\nu$. The full position and [velocity](classical-mechanics.md#velocity) return after finitely many radial periods precisely when $\nu$ is rational. Irrational $\nu$ gives a dense rosette on the two-frequency [invariant torus](hamiltonian-mechanics.md#invariant-torus). Rationality permits a fifth [orbit](dynamical-systems.md#orbit-dynamical-system) label fixing the apsidal phase on that resonant [angular momentum](momentum.md#angular-momentum) family, but does not give global superintegrability for all nearby angular momenta. When $a=0$, every regular bound [Kepler orbit](#kepler-orbit) is closed and the [Laplace-Runge-Lenz vector](classical-mechanics.md#laplace-runge-lenz-vector) supplies the globally defined additional integral.

##### Inverse-cube perturbation of Kepler apsidal motion

↑ **Parent:** [Orbit equation for combined inverse-square and inverse-cube attraction](#orbit-equation-for-combined-inverse-square-and-inverse-cube-attraction)

For radial acceleration $-\mu/r^2+C/r^3$, the [Binet equation](#binet-equation) gives $u''+(1+C/h^2)u=\mu/h^2$, where $h$ is [specific angular momentum](#specific-angular-momentum). A regular bound orbit has $h^2+C>0$, $a=-\mu/(2\mathcal E)$ and $e^2=1+2\mathcal E(h^2+C)/\mu^2$. Its radius is $a(1-e^2)/[1+e\cos(\alpha\theta)]$, with $\alpha=\sqrt{1+C/h^2}$. The [apsidal precession](planetary-science.md#apsidal-precession) per radial period is $2\pi(\alpha^{-1}-1)$, which reduces to the displayed expression for a small perturbation. Negative $C$ produces prograde precession; positive $C$ produces retrograde precession. The dimensionless coefficient is $C/(\mu a)$, since $C$ has units of length to the fourth power divided by time squared.

###### Inferring an inverse-cube perturbation from apsidal precession

↑ **Parent:** [Inverse-cube perturbation of Kepler apsidal motion](#inverse-cube-perturbation-of-kepler-apsidal-motion)

For radial acceleration $-GM(1+\gamma/r)/r^2$, conserved [specific angular momentum](#specific-angular-momentum) $h$ gives an angular radial frequency $\alpha=\sqrt{1-GM\gamma/h^2}$ through the [Binet equation](#binet-equation). Successive pericentres differ by $2\pi/\alpha$, so a small perturbation produces [apsidal precession](planetary-science.md#apsidal-precession) $\Delta\varpi\simeq\pi GM\gamma/h^2$. Writing the unperturbed semilatus rectum as $p=h^2/(GM)$ gives the displayed inverse relation. For a nearly circular orbit of period $P$, use $p\simeq[GM(P/(2\pi))^2]^{1/3}$. Positive $\gamma$ means prograde precession; $\gamma$ is a length. A measured rate per century must first be converted to an angle per orbit.

#### Inferring an inverse-square force from Kepler laws

↑ **Parent:** [Binet equation](#binet-equation)

Constant [areal velocity](momentum.md#areal-velocity) gives constant specific [angular momentum](momentum.md#angular-momentum) $l=r^2\dot\theta$, hence zero transverse acceleration and a [central force](mathematical-physics.md#central-force). For a focus-based [ellipse](euclidean-geometry.md#ellipse) $u=1/r=(1+\varepsilon\cos\theta)/A$, one has $u_{\theta\theta}+u=1/A$. The [Binet equation](#binet-equation) then gives the displayed radial acceleration, proving an attractive [inverse-square law](physics.md#inverse-square-law). An orbit's shape alone does not specify its acceleration without a time law.

#### Damped Binet equation

↑ **Parent:** [Binet equation](#binet-equation)

An attractive [inverse-square force](classical-mechanics.md#inverse-square-force) together with radial drag $-k\dot r/r^2$ preserves [angular momentum](momentum.md#angular-momentum) $h=r^2\dot\theta$ but modifies the [Binet equation](#binet-equation) for $u=1/r$ by a first derivative. For $k/|h|<2$ and $h\ne0$, the reciprocal radius is a decaying oscillation about $p/h^2$. Forward angular distance $\operatorname{sgn}(h)(\theta-\theta_0)$ makes its damping sign explicit for either orbital orientation.

##### Circularization under radial inverse-square drag

↑ **Parent:** [Damped Binet equation](#damped-binet-equation)

A bounded trajectory in the [damped Binet equation](#damped-binet-equation) with nonzero [angular momentum](momentum.md#angular-momentum) asymptotically becomes circular. Energy loss is nonnegative in magnitude and vanishes only for zero radial velocity. The centrifugal effective [potential energy](energy.md#potential-energy) excludes collision; bounded radius forces indefinitely increasing forward angular distance, so the reciprocal-radius oscillation decays. Escaping trajectories are excluded by the boundedness hypothesis.

#### Shifted inverse-radius potential

↑ **Parent:** [Binet equation](#binet-equation)

For

$$
V(r)=-\frac{km}{r-r_0},
\qquad r>r_0,
$$

Binet’s equation is

$$
u''+u=\frac{K}{(1-r_0u)^2},
\qquad K=\frac{km^2}{\ell^2}.
$$

Its circular orbits solve $K=u(1-r_0u)^2$; the branch $u<1/(3r_0)$ is stable and the branch $u>1/(3r_0)$ is unstable.

### Orbital eccentricity

↑ **Parent:** [Kepler orbit](#kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orbital_eccentricity)

Orbital eccentricity distinguishes circular, elliptic, parabolic, and hyperbolic conics.

#### Eccentricity vector

↑ **Parent:** [Orbital eccentricity](#orbital-eccentricity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eccentricity_vector)

For an attractive [Kepler orbit](#kepler-orbit) with gravitational parameter $GM$, [velocity](classical-mechanics.md#velocity) $\mathbf v$ and [specific angular momentum](#specific-angular-momentum) $\mathbf h=\mathbf r\times\mathbf v$, the eccentricity vector is

$$
\mathbf e=\frac{\mathbf v\times\mathbf h}{GM}-\widehat{\mathbf r}.
$$

Its magnitude is the [orbital eccentricity](#orbital-eccentricity), and it points toward [periapsis](#periapsis) for a noncircular orbit. It is a normalized attractive [Laplace-Runge-Lenz vector](classical-mechanics.md#laplace-runge-lenz-vector); it remains constant under the pure inverse-square force.

##### Perturbed Kepler-orbit conservation laws

↑ **Parent:** [Eccentricity vector](#eccentricity-vector)

If the relative acceleration is $\ddot{\mathbf r}=-GM\mathbf r/r^3+\mathbf f$, with constant masses, then the [specific orbital energy](#specific-orbital-energy) $\varepsilon$, [specific angular momentum](#specific-angular-momentum) $\mathbf h$ and [eccentricity vector](#eccentricity-vector) obey

$$
\dot\varepsilon=\mathbf v\mathbin\cdot\mathbf f,\qquad
\dot{\mathbf h}=\mathbf r\times\mathbf f,\qquad
GM\dot{\mathbf e}=\mathbf f\times\mathbf h+\mathbf v\times(\mathbf r\times\mathbf f).
$$

The inverse-square-force terms cancel in each derivative. These identities express perturbing work and torque, and track the instantaneous change of the ellipse's shape and orientation.

#### Thermal eccentricity distribution

↑ **Parent:** [Orbital eccentricity](#orbital-eccentricity)

An isotropic population of bound Kepler orbits has eccentricity probability density $n(e)=2e$ on $0\leq e<1$. It follows from the fixed-energy angular-momentum measure $n(L)dL\propto LdL$ and $L=L_c\sqrt{1-e^2}$.

##### Delaunay phase-volume proof of the thermal eccentricity distribution

↑ **Parent:** [Thermal eccentricity distribution](#thermal-eccentricity-distribution)

For bound [Kepler orbits](#kepler-orbit), the [Delaunay variables](hamiltonian-mechanics.md#delaunay-variables) obey $0<G<L$, $-G<H<G$, and three periodic angles. A [canonical transformation](hamiltonian-mechanics.md#canonical-transformation) preserves [phase space](hamiltonian-mechanics.md#phase-space) volume. At fixed $L$, integrating $H$ supplies the measure $2G\,dG$. Since $G=L\sqrt{1-e^2}$, the fraction with [orbital eccentricity](#orbital-eccentricity) less than $e$ is $L^{-2}\int_{L\sqrt{1-e^2}}^L2G\,dG=e^2$. Thus the [probability density function](continuous-probability-distribution.md#probability-density-function) is $2e$, independently of any normalizable energy-only [phase-space distribution function](statistical-physics.md#phase-space-distribution-function). A [Boltzmann distribution](thermodynamics.md#boltzmann-distribution) is unnecessary. Even the time-dependent density $F(E(L))[1+\eta\cos(l-n(L)t)]$, $|\eta|<1$, has this same marginal because integrating the [mean anomaly](#mean-anomaly) removes its oscillatory part; an eccentricity marginal alone does not imply equilibrium.

###### Finite normalization of an energy-only Kepler distribution

↑ **Parent:** [Delaunay phase-volume proof of the thermal eccentricity distribution](#delaunay-phase-volume-proof-of-the-thermal-eccentricity-distribution)

For bound [Kepler orbits](#kepler-orbit) with gravitational parameter $\mu$, integrating the [Delaunay variables](hamiltonian-mechanics.md#delaunay-variables) over $0<G<L$, $-G<H<G$ and their three full angle periods gives the displayed population. A globally defined [thermal eccentricity distribution](#thermal-eccentricity-distribution) requires this integral to converge, or an explicit finite action range. Merely having finite $F(E)$ at every energy does not suffice: $F=1$ yields an infinite integral at large $L$. At each fixed energy, or on every finite normalized action band, the cumulative eccentricity fraction remains $e^2$.

### Elliptic orbit

↑ **Parent:** [Kepler orbit](#kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elliptic_orbit)

An elliptic orbit is a bound orbit shaped as an ellipse. A Kepler ellipse has negative [specific orbital energy](#specific-orbital-energy) and eccentricity $0\leq e<1$.

### Hyperbolic Kepler orbit

↑ **Parent:** [Kepler orbit](#kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_Kepler_orbit)

A positive-energy inverse-square orbit is a hyperbola with two scattering asymptotes.

#### Gravitational scattering angle

↑ **Parent:** [Hyperbolic Kepler orbit](#hyperbolic-kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gravitational_scattering_angle)

The gravitational scattering angle is the change between incoming and outgoing asymptotic velocity directions.

##### Non-colliding gravitational velocity-kick bound

↑ **Parent:** [Gravitational scattering angle](#gravitational-scattering-angle)

For a local two-body hyperbolic encounter with central parameter $\mu$ and allowed centre separation $r_{\min}\geq r_0$, [conservation of energy](mathematical-physics.md#conservation-of-energy) gives equal asymptotic speeds. The [gravitational scattering angle](#gravitational-scattering-angle) therefore implies

$$
|\Delta\boldsymbol v|=\frac{2v_\infty}{1+r_{\min}v_\infty^2/\mu}
\leq\sqrt{\frac{\mu}{r_0}}=\frac{v_{\rm esc}(r_0)}{\sqrt2}.
$$

Put $z=v_\infty\sqrt{r_{\min}/\mu}$ and use $2z/(1+z^2)\leq1$. The optimizing grazing [orbit](dynamical-systems.md#orbit-dynamical-system) has $z=1$, [orbital eccentricity](#orbital-eccentricity) two and deflection $\pi/3$. For finite spherical bodies $r_0$ is the sum of their radii; excluding actual contact makes the upper bound a supremum. Without a finite exclusion radius the ideal point-mass problem has no finite bound.

#### Gravitational assist

↑ **Parent:** [Hyperbolic Kepler orbit](#hyperbolic-kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gravitational_assist)

In a gravitational assist, a small body's speed relative to a moving massive body is deflected with nearly unchanged magnitude. Transforming back to the inertial frame can transfer orbital energy between the bodies.

### Parabolic trajectory

↑ **Parent:** [Kepler orbit](#kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parabolic_trajectory)

A zero-energy inverse-square orbit is parabolic and has eccentricity one.

#### Barker equation

↑ **Parent:** [Parabolic trajectory](#parabolic-trajectory)

For a [parabolic trajectory](#parabolic-trajectory) with [periapsis](#periapsis) radius $r_p$, put $D=\tan(f/2)$, where $f$ is [true anomaly](#true-anomaly). The Barker equation is $t-t_p=\sqrt{2r_p^3/(GM)}(D+D^3/3)$. Since $r=r_p(1+D^2)$, it is equivalent to the [radius-time relation for a parabolic Kepler orbit](#radius-time-relation-for-a-parabolic-kepler-orbit). The sign of $D$ distinguishes approach from recession; $t_p$ is the [periapsis](#periapsis) time.

##### Radius-time relation for a parabolic Kepler orbit

↑ **Parent:** [Barker equation](#barker-equation)

On a nonradial zero-[energy](energy.md) [Kepler orbit](#kepler-orbit), conserved [specific angular momentum](#specific-angular-momentum) $h$ gives periapsis $r_p=h^2/(2GM)$ and $\dot r^2=2GM(r-r_p)/r^2$. Integrating with $s=\sqrt{r-r_p}$ yields $t-t_p=\pm\sqrt{2/(GM)}(r+2r_p)\sqrt{r-r_p}/3$. Squaring gives the displayed version of the [Barker equation](#barker-equation), valid on both incoming and outgoing branches. The time origin $t_p$ is passage through [periapsis](#periapsis), not an arbitrary point on the orbit.

##### Pericentre-to-crossover flight time

↑ **Parent:** [Barker equation](#barker-equation)

A [parabolic Kepler orbit](#parabolic-trajectory) obeys $t=\sqrt{2q^3/(GM)}(D+D^3/3)$ with $D=\tan(f/2)$. At the [high-eccentricity angular-speed crossover](#high-eccentricity-angular-speed-crossover), $q\ll r_x$, so $n_pt_x\simeq(\sqrt2/3)(r_x/a_p)^{3/2}=2^{7/8}(q/a_p)^{3/8}/3$. The small time fraction explains why an eccentric orbit turns through almost $\pi$ of [true anomaly](#true-anomaly) while a distant perturber barely moves.

### Periapsis

↑ **Parent:** [Kepler orbit](#kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Periapsis)

The periapsis is the point of an orbit nearest its force centre.

#### Pericentre distance

↑ **Parent:** [Periapsis](#periapsis)

### Apoapsis

↑ **Parent:** [Kepler orbit](#kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Apoapsis)

The apoapsis is the point of an orbit farthest from its force centre.

#### Apocentre distance

↑ **Parent:** [Apoapsis](#apoapsis)

### Semi-major axis

↑ **Parent:** [Kepler orbit](#kepler-orbit)

The semi-major axis is one half of an ellipse's longest diameter. For a Kepler ellipse with apsidal distances $r_1,r_2$, it is $a=(r_1+r_2)/2$.

This is one of the [semi-major and semi-minor axes](euclidean-geometry.md#semi-major-and-semi-minor-axes); the two-axis geometry is the broader concept.

### Semi-minor axis

↑ **Parent:** [Kepler orbit](#kepler-orbit)

For an ellipse of eccentricity $e$, the semi-minor axis is $b=a\sqrt{1-e^2}$.

This is one of the [semi-major and semi-minor axes](euclidean-geometry.md#semi-major-and-semi-minor-axes); the two-axis geometry is the broader concept.

### Orbital element

↑ **Parent:** [Kepler orbit](#kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orbital_element)

An orbital element is one of a set of parameters specifying an orbit at a chosen epoch. For a Kepler orbit, the semi-major axis and eccentricity determine its size and shape, while angular elements determine its orientation and the body's position.

#### Radial-velocity semi-amplitude

↑ **Parent:** [Orbital element](#orbital-element)

Half the full range of an orbit-induced line-of-sight [velocity](classical-mechanics.md#velocity) variation, after accounting for a constant systemic offset.

#### Argument of periapsis

↑ **Parent:** [Orbital element](#orbital-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Argument_of_periapsis)

The [argument of periapsis](#argument-of-periapsis) is the angle in the [orbital plane](#orbital-plane) from the [ascending node](#ascending-node) to [periapsis](#periapsis), measured in the direction of motion. It differs from the [longitude of periapsis](#longitude-of-periapsis) $\varpi=\Omega+\omega$. For an inclined orbit this sum is a conventional longitude, not generally the azimuth of the projected periapsis. The argument is undefined for a circular orbit and the node-based description is singular when the orbit and reference plane coincide.

#### True longitude

↑ **Parent:** [Orbital element](#orbital-element)

True longitude is the conventional orbital angle formed from the [longitude of ascending node](#longitude-of-ascending-node), argument of [periapsis](#periapsis) and [true anomaly](#true-anomaly). For a coplanar [Kepler orbit](#kepler-orbit) it is the actual polar longitude of the position vector. For an inclined [orbital plane](#orbital-plane) the sum of angles is generally not the projected azimuth. The [mean longitude](#mean-longitude) uses [mean anomaly](#mean-anomaly) $M$ in place of $f$, so $\ell_{\rm true}-\lambda=f-M$. For small [orbital eccentricity](#orbital-eccentricity), [Kepler's equation](#kepler-s-equation) gives $E=M+e\sin M+O(e^2)$, while the eccentric-to-true anomaly relation gives $f=E+e\sin E+O(e^2)$; hence $f-M=2e\sin M+O(e^2)$. This periodic difference matters when separating a slow [resonant argument](#resonant-argument) from a rapidly varying geometric angle.

#### Orbital plane

↑ **Parent:** [Orbital element](#orbital-element)

The plane containing a central-force [Kepler orbit](#kepler-orbit), perpendicular to its conserved [specific angular momentum](#specific-angular-momentum). Its orientation can be specified by an [orbital inclination](#orbital-inclination) and an [orbital node](#orbital-node). Perturbing [forces](force.md) can change that orientation.

#### Osculating orbital element

↑ **Parent:** [Orbital element](#orbital-element)

An [orbital element](#orbital-element) of the [Kepler orbit](#kepler-orbit) having the same instantaneous position and [velocity](classical-mechanics.md#velocity) as a perturbed trajectory. Its elements vary as the perturbing [force](force.md) acts. Their interpretation depends on the central [gravitational parameter](newton-s-law-of-universal-gravitation.md#standard-gravitational-parameter) used, for example whether static [radiation pressure](pressure.md#radiation-pressure) is included in the unperturbed attraction.

##### Astrocentric osculating-element oscillations

↑ **Parent:** [Osculating orbital element](#osculating-orbital-element)

A circular distant barycentric [Kepler orbit](#kepler-orbit) around a circular star–planet binary need not have constant star-centred [osculating orbital elements](#osculating-orbital-element). Let $\mu$ be the planet's fraction of the binary [mass](classical-mechanics.md#mass), $\alpha=a_{\rm pl}/a\ll1$, and $\varepsilon=\mu/\sqrt\alpha\ll1$. Subtracting the stellar reflex [velocity](classical-mechanics.md#velocity) produces radial and tangential perturbations $(-v_0\varepsilon\sin\Delta,v_0\varepsilon\cos\Delta)$, where $\Delta$ is the planet's longitude minus the particle's longitude. The [vis-viva equation](#vis-viva-equation) gives the displayed [semi-major axis](#semi-major-axis) variation. The [eccentricity vector](#eccentricity-vector) components follow from $e_r=rv_\theta^2/(GM_\star)-1$ and $e_\theta=-rv_rv_\theta/(GM_\star)$. The errors are $O(\mu+\varepsilon^2)$; the spatial translation itself is only $O(\mu\alpha)$. These are changes of instantaneous orbital description, even when the assumed barycentric trajectory is fixed.

#### True anomaly

↑ **Parent:** [Orbital element](#orbital-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/True_anomaly)

The true anomaly is the angle at the focus from periapsis to the current position of an orbiting body, measured in the direction of motion.

#### Orbital phase

↑ **Parent:** [Orbital element](#orbital-element)

Orbital phase specifies where a body lies within its orbital cycle relative to a chosen reference event.

##### Phase-mixed orbit

↑ **Parent:** [Orbital phase](#orbital-phase)

A phase-mixed orbit has a probability distribution uniform in its canonical angle variable. For a Kepler ellipse, this means uniform mean anomaly and therefore probability proportional to time spent in each orbital segment.

###### Line density on a Kepler orbit

↑ **Parent:** [Phase-mixed orbit](#phase-mixed-orbit)

Uniform [mean anomaly](#mean-anomaly) implies a line probability inversely proportional to the orbital speed. For small [orbital eccentricity](#orbital-eccentricity) and [true anomaly](#true-anomaly) $f$, it is proportional to $1-e\cos f$.

###### Cross-sectional-area current

↑ **Parent:** [Line density on a Kepler orbit](#line-density-on-a-kepler-orbit)

The [geometric cross-section](classical-mechanics.md#geometric-collision-cross-section) passing a fixed point of a steady orbital wire per unit time is $J_\sigma=\lambda_\sigma v$, where $\lambda_\sigma=d\sigma/ds$. Conservation of fragments requires $J_\sigma$ constant and $\lambda_\sigma\propto1/v$. For total area $\sigma_{\rm tot}$ and [orbital period](#orbital-period) $P$,

$$
J_\sigma=\frac{\sigma_{\rm tot}}P.
$$

With the [fractional luminosity of a phase-mixed eccentric wire](planetary-science.md#fractional-luminosity-of-a-phase-mixed-eccentric-wire), this becomes $J_\sigma=2fh$. The current describes transported area, not the swept area enclosed by the [orbit](dynamical-systems.md#orbit-dynamical-system).

###### Phase-mixed radial probability of a Kepler orbit

↑ **Parent:** [Phase-mixed orbit](#phase-mixed-orbit)

For a [Kepler orbit](#kepler-orbit) with [pericentre distance](#pericentre-distance) $q$, [apocentre distance](#apocentre-distance) $Q$, and [semi-major axis](#semi-major-axis) $a=(q+Q)/2$, a uniform [mean anomaly](#mean-anomaly) gives

$$
p_r(r)=\frac{r}{\pi a\sqrt{(r-q)(Q-r)}},\qquad q<r<Q.
$$

The two radial passages per [orbital period](#orbital-period) are included, and $\int_q^Qp_r(r)\,dr=1$.

#### Mean anomaly

↑ **Parent:** [Orbital element](#orbital-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mean_anomaly)

Mean anomaly is the uniformly increasing phase $M=n(t-\tau)$ of a Kepler orbit, measured from periapsis time $\tau$.

<h5 id="kepler-s-equation">Kepler's equation</h5>

↑ **Parent:** [Mean anomaly](#mean-anomaly)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kepler's_equation)

For an elliptic [Kepler orbit](#kepler-orbit), [Kepler's equation](#kepler-s-equation) relates [mean anomaly](#mean-anomaly) $M$ and [eccentric anomaly](#eccentric-anomaly) $E$ by

$$
M=E-e\sin E.
$$

#### Eccentric anomaly

↑ **Parent:** [Orbital element](#orbital-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eccentric_anomaly)

The eccentric anomaly parametrizes a Kepler ellipse through the corresponding point on its auxiliary circle. It gives radius $r=a(1-e\cos E)$.

#### Orbital node

↑ **Parent:** [Orbital element](#orbital-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orbital_node)

An orbital node is an intersection of an orbital plane with its reference plane.

##### Ascending node

↑ **Parent:** [Orbital node](#orbital-node)

The ascending node is the orbital node where a body crosses from the negative to the positive side of the reference plane.

###### Longitude of ascending node

↑ **Parent:** [Ascending node](#ascending-node)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Longitude_of_ascending_node)

The longitude of ascending node is the reference-plane angle from a fixed direction to the ascending node.

#### Orbital inclination

↑ **Parent:** [Orbital element](#orbital-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orbital_inclination)

Orbital inclination is the angle between an orbital plane and a reference plane.

##### Orbital-frame rotation from inclination and node

↑ **Parent:** [Orbital inclination](#orbital-inclination)

In a right-handed reference frame, the [rotation matrix](linear-algebra.md#rotation-matrix) from an [orbital plane](#orbital-plane) frame whose first axis points along the [ascending node](#ascending-node) is $R_z(\Omega)R_x(I)$. Its columns are the orbital frame's [orthonormal basis](inner-product.md#orthonormal-basis) expressed in reference coordinates. The [unit vector](vector-space.md#unit-vector) normal is $(\sin\Omega\sin I,-\cos\Omega\sin I,\cos I)$; its [dot product](inner-product.md#dot-product) with another such normal gives the cosine of their [mutual inclination](#mutual-inclination).

##### Mutual inclination

↑ **Parent:** [Orbital inclination](#orbital-inclination)

The mutual inclination is the angle between two orbital planes, equivalently the angle between consistently oriented orbital normal vectors.

###### Mutual inclination of nearly edge-on orbits

↑ **Parent:** [Mutual inclination](#mutual-inclination)

For two nearly [edge-on orbits](#edge-on-orbit) with small [orbital inclination](#orbital-inclination) difference $\Delta I$ and small [longitude of ascending node](#longitude-of-ascending-node) difference $\Delta\Omega$, expanding the [dot product](inner-product.md#dot-product) of their normals gives $I_m^2=(\Delta I)^2+(\Delta\Omega)^2+O(\delta^4)$, with angles in radians and all offsets from edge-on of order $\delta$. Thus equality of observed sky-plane inclinations alone does not imply aligned [orbital planes](#orbital-plane).

##### Invariable plane

↑ **Parent:** [Orbital inclination](#orbital-inclination)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Invariable_plane)

The invariable plane is perpendicular to a system's total [angular momentum](momentum.md#angular-momentum). For an isolated planetary system, it is fixed while individual orbital planes precess.

###### Inclination to the invariable plane of two orbital planes

↑ **Parent:** [Invariable plane](#invariable-plane)

For two groups carrying [angular momenta](momentum.md#angular-momentum) $L_a,L_b$ with [mutual inclination](#mutual-inclination) $\Delta I$, resolving total [angular momentum](momentum.md#angular-momentum) parallel and perpendicular to the second group's normal gives its [orbital inclination](#orbital-inclination) relative to the [invariable plane](#invariable-plane):

$$
I_b=\operatorname{atan2}(L_a\sin\Delta I,L_b+L_a\cos\Delta I).
$$

For a positive denominator, $\tan I_b=\sin\Delta I/(L_b/L_a+\cos\Delta I)$. The larger-angular-momentum group lies closer to the [invariable plane](#invariable-plane).

##### Edge-on orbit

↑ **Parent:** [Orbital inclination](#orbital-inclination)

An orbit is edge-on to an observer when its orbital plane contains the line of sight, so its inclination to the plane of the sky is $90^\circ$.

##### Orbital-plane orientation degeneracy

↑ **Parent:** [Orbital inclination](#orbital-inclination)

Projected observations that do not identify which node is ascending may determine an orbital plane only up to reversal of its normal or addition of $\pi$ to its nodal longitude.

#### Longitude of periapsis

↑ **Parent:** [Orbital element](#orbital-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Longitude_of_periapsis)

The longitude of periapsis gives the angular direction of periapsis in the reference plane.

#### Mean longitude

↑ **Parent:** [Orbital element](#orbital-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mean_longitude)

Mean longitude is an angle that advances uniformly at the mean motion in an unperturbed Kepler orbit.

#### Mean motion

↑ **Parent:** [Orbital element](#orbital-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mean_motion)

Mean motion is the average orbital angular frequency. A Kepler orbit about gravitational parameter $\mu$ has $n^2a^3=\mu$.

##### Orbital period

↑ **Parent:** [Mean motion](#mean-motion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orbital_period)

The orbital period is the time required to complete one orbit. It is related to [mean motion](#mean-motion) by $T=2\pi/n$.

###### Low circular-orbit period measures mean density

↑ **Parent:** [Orbital period](#orbital-period)

For a spherical body of radius $R$, mass $M$ and [mean density](fluid-mechanics.md#mean-density) $\bar\rho=3M/(4\pi R^3)$, a low [circular orbit](classical-mechanics.md#circular-orbit) has period $P\simeq2\pi\sqrt{R^3/(GM)}$, by equating the gravitational acceleration from [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md) to the [centripetal acceleration](classical-mechanics.md#centripetal-acceleration). Substitution proves the displayed relation. Thus similar low-orbit periods indicate similar mean densities, even for bodies with very different masses and radii. At altitude $h$, the right side is multiplied by $(1+h/R)^3$; the simple density inference requires $h\ll R$ and neglects rotation, nonsphericity and other gravitating bodies.

##### Synodic period

↑ **Parent:** [Mean motion](#mean-motion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Synodic_period)

The synodic period is the interval between successive repetitions of the relative orbital configuration of two bodies. For coplanar prograde mean motions $n_1,n_2$, it is $2\pi/|n_1-n_2|$.

### Specific orbital energy

↑ **Parent:** [Kepler orbit](#kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Specific_orbital_energy)

The specific orbital energy is the mechanical energy per unit mass,

$$
\varepsilon=\frac{v^2}{2}-\frac{\mu}{r}=-\frac{\mu}{2a}.
$$

Its sign distinguishes bound elliptic, marginal parabolic, and unbound hyperbolic Kepler orbits.

#### Orbit-averaged drag work

↑ **Parent:** [Specific orbital energy](#specific-orbital-energy)

A weak perturbing relative acceleration $\mathbf f$ changes [specific orbital energy](#specific-orbital-energy) at rate $\dot\varepsilon=\mathbf v\cdot\mathbf f$. Since $\varepsilon=-\mu/(2a)$ for a [Kepler orbit](#kepler-orbit),

$$
\dot a=\frac{2a^2}{\mu}\mathbf v\cdot\mathbf f.
$$

For a circular [Kepler orbit](#kepler-orbit) under $\mathbf f=-\kappa\mathbf v+\mathbf g$ with constant $\mathbf g$, the constant-force term averages to zero over an unperturbed orbit. Thus $\langle\dot a\rangle=-2\kappa a$. This is a leading-order orbital average; a strong constant force can distort the orbit instead.

#### Vis-viva equation

↑ **Parent:** [Specific orbital energy](#specific-orbital-energy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vis-viva_equation)

For a [Kepler orbit](#kepler-orbit) with [semi-major axis](#semi-major-axis) $a$, the [vis-viva equation](#vis-viva-equation) is

$$
v^2=\mu\left(\frac2r-\frac1a\right).
$$

For the convention that a [hyperbolic Kepler orbit](#hyperbolic-kepler-orbit) has positive semi-major-axis magnitude $a$, its final term instead has a plus sign.

### Specific angular momentum

↑ **Parent:** [Kepler orbit](#kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Specific_angular_momentum)

The specific angular momentum is angular momentum per unit mass, $\mathbf h=\mathbf r\times\mathbf v$. For a planar Kepler orbit its magnitude is $h=r^2\dot\theta=\sqrt{\mu a(1-e^2)}$.

#### High-eccentricity angular-speed crossover

↑ **Parent:** [Specific angular momentum](#specific-angular-momentum)

For a nearly radial [Kepler orbit](#kepler-orbit) with [pericentre](#periapsis) $q$, [specific angular momentum](#specific-angular-momentum) is $h\simeq\sqrt{2GMq}$. Relative to a circular reference orbit of radius $a_p$ and [mean motion](#mean-motion) $n_p$, the instantaneous azimuthal rate changes from faster to slower at $r_x=\sqrt{h/n_p}\simeq a_p(2q/a_p)^{1/4}$. In a [rotating reference frame](mathematical-physics.md#rotating-reference-frame) the polar angle has a turning point at this radius. The [true anomaly](#true-anomaly) there differs from $\pi$ by approximately $2\sqrt{q/r_x}$.

#### Periapsis angular speed

↑ **Parent:** [Specific angular momentum](#specific-angular-momentum)

The [specific angular momentum](#specific-angular-momentum) of an elliptic [Kepler orbit](#kepler-orbit) is $h=\sqrt{\mu a(1-e^2)}$. At [periapsis](#periapsis), $r=a(1-e)$, so

$$
\dot\theta_{\rm peri}=\frac h{r^2}=n\frac{\sqrt{1+e}}{(1-e)^{3/2}}.
$$

The [mean motion](#mean-motion) understates instantaneous angular speed near [periapsis](#periapsis). A particle in an [exterior mean-motion resonance](#exterior-mean-motion-resonance) can briefly overtake the planet in angle despite completing full orbits more slowly.

### Circular Kepler orbit

↑ **Parent:** [Kepler orbit](#kepler-orbit)

A circular Kepler orbit at radius $r$ has speed $v_K=\sqrt{\mu/r}$ and mean motion $n=\sqrt{\mu/r^3}$.

#### Synchronous circular orbit

↑ **Parent:** [Circular Kepler orbit](#circular-kepler-orbit)

A satellite remaining above a fixed point of a uniformly rotating spherical planet must have a prograde equatorial [circular Kepler orbit](#circular-kepler-orbit) with angular speed $2\pi/T$. Balancing gravitational acceleration and centripetal acceleration gives the displayed radius and speed $v=2\pi r/T$. The satellite's own mass cancels. A physically realizable external orbit additionally requires this radius to exceed the planet's radius.

##### Geostationary orbit

↑ **Parent:** [Synchronous circular orbit](#synchronous-circular-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geostationary_orbit)

A [geostationary orbit](#geostationary-orbit) is a prograde equatorial [circular Kepler orbit](#circular-kepler-orbit) whose [orbital period](#orbital-period) equals one [sidereal day](astrophysics.md#sidereal-day), so its satellite remains above a fixed location on [Earth](planetary-science.md#earth)'s equator. It is the terrestrial case of a [planet-stationary orbit](#planet-stationary-orbit). Its radius follows from [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md) and circular [acceleration](classical-mechanics.md#acceleration): $r=(GM_ET^2/(4\pi^2))^{1/3}$, approximately $42164\ \mathrm{km}$ from [Earth](planetary-science.md#earth)'s centre. Its altitude above the surface is smaller by [Earth](planetary-science.md#earth)'s radius.

### Hohmann transfer orbit

↑ **Parent:** [Kepler orbit](#kepler-orbit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hohmann_transfer_orbit)

A Hohmann transfer uses two tangential impulses and one half of an elliptic Kepler orbit to move between two coplanar circular orbits.

#### Reversed circularization burn in a Hohmann transfer

↑ **Parent:** [Hohmann transfer orbit](#hohmann-transfer-orbit)

An outward transfer from radius $R$ to $\alpha R$ arrives with speed $v_a/v_c=\sqrt{2/(1+\alpha)}$, where $v_c$ is the desired outer circular speed. Reversing the same circularization [impulse](classical-mechanics.md#impulse) leaves speed ratio $v_w/v_c=2\sqrt{2/(1+\alpha)}-1$, possibly signed. Its square $q$ determines the new [apocentre](#apoapsis) [orbit](dynamical-systems.md#orbit-dynamical-system): $e=1-q$ and $r_p=\alpha Rq/(2-q)$. The [orbit](dynamical-systems.md#orbit-dynamical-system) intersects a spherical body of radius $R_b$ if $r_p<R_b$. A negative signed speed means retrograde motion, while $q=0$ is the degenerate radial-fall limit.

#### Hohmann transfer impulse fractions

↑ **Parent:** [Hohmann transfer orbit](#hohmann-transfer-orbit)

For a [Hohmann transfer orbit](#hohmann-transfer-orbit) from radius $r_0$ to $\eta r_0$, with $\eta>1$ and initial circular speed $v_0=\sqrt{GM/r_0}$, conservation of [orbital energy](#orbital-energy) and [angular momentum](momentum.md#angular-momentum) gives transfer endpoint speeds $v_p/v_0=\sqrt{2\eta/(1+\eta)}$ and $v_a/v_0=\sqrt{2/[\eta(1+\eta)]}$. The required prograde impulses are

$$
\frac{\Delta v_1}{v_0}=\sqrt{\frac{2\eta}{1+\eta}}-1,\qquad
\frac{\Delta v_2}{v_0}=\frac1{\sqrt\eta}-\sqrt{\frac2{\eta(1+\eta)}}.
$$

If the spacecraft mass is constant and fuel use is proportional to impulse magnitude, these also give the fuel fractions relative to a budget with total speed change $v_0$. Their sum is a sum of magnitudes, even though the burns occur at different positions and directions.

#### Hohmann transfer time

↑ **Parent:** [Hohmann transfer orbit](#hohmann-transfer-orbit)

A [Hohmann transfer orbit](#hohmann-transfer-orbit) between coplanar [circular Kepler orbits](#circular-kepler-orbit) of radii $r_1,r_2$ traverses half an [elliptic orbit](#elliptic-orbit) of [semi-major axis](#semi-major-axis) $a=(r_1+r_2)/2$. [Kepler's third law](mathematical-physics.md#kepler-s-third-law) therefore gives $t=\pi\sqrt{a^3/(GM)}$. Relative to the initial [orbital period](#orbital-period) $T_1$, $t=(T_1/2)[(r_1+r_2)/(2r_1)]^{3/2}$. Radii must be measured from the attracting centre, rather than from its surface.

## Restricted three-body problem

↑ **Parent:** [Celestial mechanics](celestial-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Restricted_three-body_problem)

The restricted three-body problem follows a negligibly massive particle in the gravitational field of two massive bodies whose motion is unaffected by the particle.

### Circular restricted three-body problem

↑ **Parent:** [Restricted three-body problem](#restricted-three-body-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circular_restricted_three-body_problem)

In the circular restricted three-body problem the two massive bodies move on circular orbits about their barycentre. The problem is autonomous in their uniformly rotating frame.

#### Hill equations

↑ **Parent:** [Circular restricted three-body problem](#circular-restricted-three-body-problem)

The unforced planar [equation of motion in a rotating frame](classical-mechanics.md#equation-of-motion-in-a-rotating-frame) near a circular [Kepler orbit](#kepler-orbit) has components $\ddot x-2n\dot y-3n^2x=0$ and $\ddot y+2n\dot x=0$. They describe [epicyclic motion](astrophysical-disk.md#epicyclic-motion) and [Keplerian shear](planetary-science.md#keplerian-shear); mutual gravity adds close-encounter forcing.

##### Free solution of Hill equations

↑ **Parent:** [Hill equations](#hill-equations)

###### Orbital elements from Hill coordinates

↑ **Parent:** [Free solution of Hill equations](#free-solution-of-hill-equations)

The oscillatory integration constants determine the [orbital eccentricity](#orbital-eccentricity) vector, the constant radial offset determines the [semi-major axis](#semi-major-axis), and the constant along-track offset fixes the [mean longitude](#mean-longitude). The radial and tangential epicycle amplitudes have ratio $1:2$.

#### Photogravitational restricted three-body problem

↑ **Parent:** [Circular restricted three-body problem](#circular-restricted-three-body-problem)

The photogravitational restricted three-body problem adds radial [radiation pressure](pressure.md#radiation-pressure) from one or both luminous primaries. If the pressure-to-gravity ratio of primary $i$ is $\beta_i$, its effective attraction on the test particle is multiplied by $1-\beta_i$.

#### Lagrange point

↑ **Parent:** [Circular restricted three-body problem](#circular-restricted-three-body-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lagrange_point)

A Lagrange point is an equilibrium of the [circular restricted three-body problem](#circular-restricted-three-body-problem) in the frame rotating with the two massive bodies.

##### Effective-potential geometry of Lagrange points

↑ **Parent:** [Lagrange point](#lagrange-point)

The [rotating-frame effective potential](mathematical-physics.md#rotating-frame-effective-potential) of the [circular restricted three-body problem](#circular-restricted-three-body-problem) has negative singular wells at both primaries. Its three [Collinear Lagrange points](#collinear-lagrange-point) are planar saddles, and its two [Triangular Lagrange points](#triangular-lagrange-point) are planar local maxima for nonzero primary masses. These geometric labels do not replace a dynamical stability analysis including the [Coriolis force](mathematical-physics.md#coriolis-force).

##### Collinear Lagrange point

↑ **Parent:** [Lagrange point](#lagrange-point)

The three collinear Lagrange points $L_1,L_2,L_3$ lie on the line through the two massive bodies.

###### Small-mass-ratio collinear Lagrange points

↑ **Parent:** [Collinear Lagrange point](#collinear-lagrange-point)

In barycentric coordinates with unit primary separation, a small secondary mass fraction $\alpha$ gives distances $(\alpha/3)^{1/3}$ from that secondary to the two neighboring [Lagrange points](#lagrange-point) at leading order. This is the dimensionless [Hill radius](#hill-radius). The opposite exterior [L3 Lagrange point](#l3-lagrange-point) has coordinate $-1-5\alpha/12+O(\alpha^2)$.

###### Inner Lagrange point

↑ **Parent:** [Collinear Lagrange point](#collinear-lagrange-point)

The [Lagrange point](#lagrange-point) lying between the components of a [circular restricted three-body problem](#circular-restricted-three-body-problem). The critical effective potential through this saddle defines their [Roche lobes](stellar-astrophysics.md#roche-lobe); gas passing through it can initiate [Roche-lobe overflow](stellar-astrophysics.md#roche-lobe-overflow).

###### L2 Lagrange point

↑ **Parent:** [Collinear Lagrange point](#collinear-lagrange-point)

The collinear [Lagrange point](#lagrange-point) beyond the smaller primary, away from the larger one, is $L_2$. For a small mass ratio it lies approximately one [Hill radius](#hill-radius) from the secondary and has a growing linear mode.

###### Linearization at L2

↑ **Parent:** [L2 Lagrange point](#l2-lagrange-point)

In unit binary separation and mean motion, displacements obey $\ddot X-2\dot Y=(1+2B)X$ and $\ddot Y+2\dot X=(1-B)Y$, where $B=\mu_1/r_1^3+\mu_2/r_2^3$ at $L_2$. The characteristic polynomial is $\lambda^4+(2-B)\lambda^2+(1+2B)(1-B)$. The small-secondary limit has $B\to4$.

###### L2 escape e-folding time

↑ **Parent:** [Linearization at L2](#linearization-at-l2)

For a small secondary-to-primary mass ratio, the unstable exponent at the outer collinear equilibrium is $n_{\rm bin}\sqrt{1+2\sqrt7}$. Its inverse is approximately $0.0634$ binary periods. Reaching a finite target distance takes this time multiplied by the logarithm of the ratio of final to initial unstable amplitudes.

###### L3 Lagrange point

↑ **Parent:** [Collinear Lagrange point](#collinear-lagrange-point)

The $L_3$ Lagrange point lies beyond the more massive primary, on the side opposite the secondary.

##### Triangular Lagrange point

↑ **Parent:** [Lagrange point](#lagrange-point)

The triangular Lagrange points $L_4,L_5$ complete equilateral triangles with the two massive bodies.

#### Hill sphere

↑ **Parent:** [Circular restricted three-body problem](#circular-restricted-three-body-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hill_sphere)

The Hill sphere is the neighborhood of a smaller body in which its gravity can dominate tidal perturbations from a larger primary.

##### Hill radius

↑ **Parent:** [Hill sphere](#hill-sphere)

For a body of mass $m$ on a circular orbit of radius $a$ about mass $M\gg m$, the Hill radius is approximately

$$
r_H=a\left(\frac{m}{3M}\right)^{1/3}.
$$

###### Mutual Hill radius

↑ **Parent:** [Hill radius](#hill-radius)

A scale for the combined gravitational influence of two small orbiting bodies relative to their common host [star](stellar-astrophysics.md#star). It is often used to express the separation of neighboring [planetary embryos](planetary-science.md#planetary-embryo). For equal masses and nearly equal orbital radii it exceeds the individual [Hill radius](#hill-radius) by $2^{1/3}$.

#### Jacobi constant

↑ **Parent:** [Circular restricted three-body problem](#circular-restricted-three-body-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi_constant)

The Jacobi constant is the conserved energy-like integral of the circular restricted three-body problem in the rotating frame.

## Orbital resonance

↑ **Parent:** [Celestial mechanics](celestial-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orbital_resonance)

An orbital resonance occurs when orbital frequencies satisfy an approximately integer relation, allowing perturbations to accumulate coherently.

### Mean-motion resonance

↑ **Parent:** [Orbital resonance](#orbital-resonance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mean-motion_resonance)

A mean-motion resonance has $jn_2-kn_1\simeq0$ for small integers $j,k$. Its slow resonant angle combines mean longitudes with apsidal or nodal longitudes.

#### Interior eccentricity-type mean-motion resonance

↑ **Parent:** [Mean-motion resonance](#mean-motion-resonance)

For an eccentric inner body and circular outer perturber near the reduced $(m+n):m$ period ratio, the leading [resonant argument](#resonant-argument) is $\phi=(m+n)\lambda_{\rm out}-m\lambda_{\rm in}-n\varpi_{\rm in}$. Its [disturbing function](planetary-science.md#disturbing-function) amplitude is of order $e_{\rm in}^n$. At a mean [conjunction](planetary-science.md#conjunction-astronomy), $\phi=n(\Lambda-\varpi_{\rm in})$; at actual alignment the exact expression is $(m+n)x-my$ with $x=f_{\rm in}$ and $y=M_{\rm in}(x)$.

#### Inclination-type mean-motion resonance

↑ **Parent:** [Mean-motion resonance](#mean-motion-resonance)

An inclination-type mean-motion resonance has a leading [resonant argument](#resonant-argument) containing a [longitude of ascending node](#longitude-of-ascending-node). Reflection symmetry forces the total nodal coefficient in each disturbing-function harmonic to be even, so the leading resonant strength is an even power of $\sin(I/2)$.

#### Exterior mean-motion resonance

↑ **Parent:** [Mean-motion resonance](#mean-motion-resonance)

In an exterior mean-motion resonance, the resonant small body orbits outside the perturbing planet and therefore has lower mean motion. A $(p+q):p$ exterior resonance has $n/n_p\simeq p/(p+q)$.

##### Resonant semi-major axis

↑ **Parent:** [Exterior mean-motion resonance](#exterior-mean-motion-resonance)

The nominal [semi-major axis](#semi-major-axis) of an exterior $(p+q):p$ [mean-motion resonance](#mean-motion-resonance) follows from $(p+q)n_r=pn_p$ and [Kepler's third law](mathematical-physics.md#kepler-s-third-law). Apsidal precession displaces the actual libration center because stationarity of the [resonant argument](#resonant-argument) requires $(p+q)n-pn_p-q\dot\varpi=0$.

##### Radiation-pressure shift of a mean-motion resonance

↑ **Parent:** [Exterior mean-motion resonance](#exterior-mean-motion-resonance)

A grain with [radiation-pressure coefficient](planetary-science.md#radiation-pressure-coefficient) $\beta<1$ feels effective central [gravitational parameter](newton-s-law-of-universal-gravitation.md#standard-gravitational-parameter) $GM_\star(1-\beta)$. Combining its [mean motion](#mean-motion) with the planet's [mean motion](#mean-motion) at an exterior-type $(j+1):j$ frequency commensurability gives the displayed [semi-major axis](#semi-major-axis). The commensurability lies geometrically exterior only for $j<\sqrt{1-\beta}/(1-\sqrt{1-\beta})$. Radiation changes the grain's attraction, so the same frequency ratio need not imply the usual radial ordering.

#### First-order mean-motion resonance

↑ **Parent:** [Mean-motion resonance](#mean-motion-resonance)

A first-order mean-motion resonance has $|j-k|=1$. For small eccentricity its leading eccentric resonant term is linear in eccentricity.

##### Resonance-overlap encounter estimate

↑ **Parent:** [First-order mean-motion resonance](#first-order-mean-motion-resonance)

A local weak [gravitational assist](#gravitational-assist) estimate for a nonradiating circular grain gives $\delta\epsilon\simeq32\mu^2\epsilon^{-5}$, where $\mu=M_p/M_\star$. [Conjunction-longitude sensitivity to an encounter](#conjunction-longitude-sensitivity-to-an-encounter) then gives $|\delta\Lambda|\simeq128\pi\mu^2/(3\epsilon^7)$. Requiring the change to exceed one full turn and using $\epsilon\simeq2/(3j)$ gives $j_c\simeq(2/729)^{1/7}\mu^{-2/7}$. This motivates loss of coherent resonant conjunctions, rather than proving that every initial phase escapes. The coefficient depends on the encounter convention and the approximations; near-planet [Hill equations](#hill-equations) require a consistent rotating-frame shear instead of mixing local inertial and rotating velocities.

#### Resonant argument

↑ **Parent:** [Mean-motion resonance](#mean-motion-resonance)

A resonant argument is a slow angular combination whose libration diagnoses resonance. For an exterior $j:(j-1)$ eccentric resonance it can be $\phi=j\lambda-(j-1)\lambda_p-\varpi$.

A resonant argument is an integer combination of orbital angles whose slow variation can diagnose [mean-motion resonance](#mean-motion-resonance). Its libration, rather than circulation through every angle, characterizes trapping in the resonance.

##### Resonant conjunction geometry

↑ **Parent:** [Resonant argument](#resonant-argument)

For an eccentric outer body and circular inner perturber, the exterior [resonant argument](#resonant-argument) is $\phi=(p+q)\lambda_{\rm out}-p\lambda_{\rm in}-q\varpi$. At equal [mean longitudes](#mean-longitude) $\Lambda$, [conjunction](planetary-science.md#conjunction-astronomy) phases are

$$
\Lambda_j=\varpi+\frac{\phi+2\pi j}{q},\qquad j=0,\ldots,q-1.
$$

The [synodic period](#synodic-period) and coprime $p,q$ determine the visitation order, with advance $2\pi p/q$. For actual true alignment, write $x=f$ and $y=M(f)$ for the eccentric body's [true anomaly](#true-anomaly) and [mean anomaly](#mean-anomaly). Then $\phi=(p+q)y-px$ instead of $qx$. The evenly spaced directions are a leading-small-eccentricity approximation.

###### Phase protection of interior integer resonances

↑ **Parent:** [Resonant conjunction geometry](#resonant-conjunction-geometry)

In a high-[orbital eccentricity](#orbital-eccentricity) interior $k:1$ [mean-motion resonance](#mean-motion-resonance), the [resonant argument](#resonant-argument) $\phi=k\lambda_p-\lambda-(k-1)\varpi$ places successive rotating-frame [apocentres](#apoapsis) at $\pi-[\phi+(2j+1)\pi]/k$. Avoiding [astronomical conjunction](planetary-science.md#conjunction-astronomy) at these slow outer excursions favors $\phi=0$ for $k=2$ and $\phi=\pi$ for $k=3$. This geometrical phase protection suggests stable [resonant-argument libration](#resonant-argument-libration) centres; actual dynamical stability requires the resonant perturbation problem.

###### Conjunction-pattern precession near a mean-motion resonance

↑ **Parent:** [Resonant conjunction geometry](#resonant-conjunction-geometry)

With constant [mean motions](#mean-motion) and $P_c/P_b=(1+\delta)(p+q)/p$, mean [conjunctions](planetary-science.md#conjunction-astronomy) advance by $\Delta\Lambda=2\pi/(P_c/P_b-1)$ each [synodic period](#synodic-period). Tracking one branch every $q$ [conjunctions](planetary-science.md#conjunction-astronomy) and subtracting $2\pi p$ gives

$$
\dot\Lambda=\frac{q\Delta\Lambda-2\pi p}{qP_{\rm syn}}
=-\frac{2\pi p\delta}{qP_b(1+\delta)}.
$$

The usual formula $-2\pi p\delta/(qP_b)$ keeps only first order in $\delta$. A labelled branch takes $qP_b(1+\delta)/(p|\delta|)$ to turn once, whereas the full set of $q$ interchangeable directions repeats after $P_b(1+\delta)/(p|\delta|)$. Finite [orbital eccentricity](#orbital-eccentricity) introduces true-conjunction corrections.

###### Conjunction-longitude sensitivity to an encounter

↑ **Parent:** [Conjunction-pattern precession near a mean-motion resonance](#conjunction-pattern-precession-near-a-mean-motion-resonance)

For an exterior circular grain with [radiation-pressure coefficient](planetary-science.md#radiation-pressure-coefficient) $\beta$, set $q=\sqrt{1-\beta}$ and $\epsilon=a/a_p-1$. Its next [conjunction](planetary-science.md#conjunction-astronomy) occurs after the [synodic period](#synodic-period), during which the planet's unwrapped [mean longitude](#mean-longitude) advances by $\Lambda=2\pi/[1-q(1+\epsilon)^{-3/2}]$. A weak [planetary scattering](planetary-science.md#planetary-scattering) encounter changes this by $\delta\Lambda\simeq-3\pi q(1+\epsilon)^{-5/2}\delta\epsilon/[1-q(1+\epsilon)^{-3/2}]^2$. Unwrapped longitude counts turns; reducing it modulo $2\pi$ before comparison would erase this measure of timing sensitivity.

##### Resonant-argument libration

↑ **Parent:** [Resonant argument](#resonant-argument)

Resonant-argument libration is bounded oscillation of a resonant argument about a stable equilibrium value instead of circulation through all angles.

###### Pendulum approximation of a mean-motion resonance

↑ **Parent:** [Resonant-argument libration](#resonant-argument-libration)

Keeping one resonant harmonic and treating [orbital eccentricity](#orbital-eccentricity) as fixed reduces [mean-motion resonance](#mean-motion-resonance) dynamics to a [physical pendulum](mathematical-physics.md#physical-pendulum) equation. For the inner first-order term $\mathcal R=(GM_2/a_2)f(\alpha)e\cos\phi$, leading [Lagrange planetary equations](planetary-science.md#lagrange-planetary-equations) give $\ddot\phi\simeq3j^2\mu_2n^2\alpha f e\sin\phi$. Around its stable phase, the small-amplitude libration frequency is $jn\sqrt{3\mu_2\alpha|f|e}$. Evolution of eccentricity, other harmonics, and approach to a [separatrix](dynamical-systems.md#separatrix) change this approximation.

###### Resonant pendulum energy

↑ **Parent:** [Pendulum approximation of a mean-motion resonance](#pendulum-approximation-of-a-mean-motion-resonance)

For $\ddot\phi=\omega_0^2\sin\phi$ with constant $\omega_0$, multiplication by $\dot\phi$ gives the conserved energy $E=\dot\phi^2/2+\omega_0^2(1+\cos\phi)$. The stable center is $\pi$; the [separatrix](dynamical-systems.md#separatrix) has $E=2\omega_0^2$. Below it the [resonant argument](#resonant-argument) librates and above it the angle circulates. This is an invariant of the constant-coefficient [pendulum approximation of a mean-motion resonance](#pendulum-approximation-of-a-mean-motion-resonance), not of arbitrary coupled [orbital element](#orbital-element) evolution.

###### Asymmetric resonant-argument libration

↑ **Parent:** [Resonant-argument libration](#resonant-argument-libration)

Libration about a resonant phase distinct from the symmetric values zero and $\pi$. For example, in a negative-Kepler-curvature reduction with disturbing potential $R=A\cos\phi+B\cos2\phi$, $A>0$, $B>A/4$, stationary points obey $\sin\phi(A+4B\cos\phi)=0$. At $\pi$, $R''=A-4B<0$, so it is unstable, whereas at $\cos\phi=-A/(4B)$ one has $R''=4B-A^2/(4B)>0$, giving two stable asymmetric centres. Actual branch thresholds depend on the resonance coefficients and evolving [orbital elements](#orbital-element).

###### Symmetric libration centres of an eccentricity resonance

↑ **Parent:** [Resonant-argument libration](#resonant-argument-libration)

In the weak, non-crossing, leading-eccentricity planar model, exterior orders one to three have positive resonant [disturbing function](planetary-science.md#disturbing-function) coefficients $B_q$. Interior eccentricity-type coefficients of these orders have sign $(-1)^q$. A local resonant [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) $H=-AJ^2/2-Be^q\cos\phi$, with $A>0$, gives $\ddot\phi=ABe^q\sin\phi$. [Linear stability analysis](dynamical-systems.md#linear-stability) therefore selects $\phi=\pi$ for $B>0$ and $\phi=0$ for $B<0$. Exterior symmetric centres are $\pi$; interior centres are $0,\pi,0$ for orders one, two and three. These are conditional leading-harmonic predictions, not universal centres at arbitrary [orbital eccentricity](#orbital-eccentricity); [asymmetric resonant-argument libration](#asymmetric-resonant-argument-libration) changes the picture.

###### Low-eccentricity correction to a first-order resonance center

↑ **Parent:** [Symmetric libration centres of an eccentricity resonance](#symmetric-libration-centres-of-an-eccentricity-resonance)

In the planar exterior first-order constant-coefficient model, differentiating the apsidal-precession term retains a contribution proportional to $C_r^2/e^2$. At the zero-phase fixed point its linear angular curvature is $3(p+1)^2nC_re-C_r^2/e^2$. Hence zero is a saddle for $3(p+1)^2ne^3>C_r$, but is a center when this inequality reverses. The usual constant-eccentricity [pendulum approximation of a mean-motion resonance](#pendulum-approximation-of-a-mean-motion-resonance) omits this term and requires $C_r/(ne^3)\ll1$.

###### Libration amplitude of a resonant argument

↑ **Parent:** [Resonant-argument libration](#resonant-argument-libration)

The libration amplitude is the maximum angular displacement of a librating resonant argument from its equilibrium value.

###### Resonance protection

↑ **Parent:** [Resonant-argument libration](#resonant-argument-libration)

Resonance protection confines conjunctions to orbital phases that avoid close encounters even when the osculating orbits geometrically cross.

#### Resonance capture

↑ **Parent:** [Mean-motion resonance](#mean-motion-resonance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Resonance_capture)

Resonance capture occurs when slow orbital migration carries a body into a resonance and the resonant argument begins to librate, so resonant torque can balance the migration torque.

## ↑ Ancestors (4)

1. [Classical mechanics](classical-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)
