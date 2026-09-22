# Schwarzschild spacetime

↑ **Parent:** [General relativity](general-relativity.md)

In units $G=c=1$, the Schwarzschild exterior metric is

$$
ds^2=-\left(1-\frac{2M}{r}\right)dt^2
+\left(1-\frac{2M}{r}\right)^{-1}dr^2+r^2d\Omega^2.
$$

**Table of contents**

- [Coordinate invariance of the Schwarzschild photon radial potential](#coordinate-invariance-of-the-schwarzschild-photon-radial-potential)
- [Schwarzschild static observer](#schwarzschild-static-observer)
  - [Local radial speed of a Schwarzschild geodesic](#local-radial-speed-of-a-schwarzschild-geodesic)
    - [Radial Schwarzschild escape with asymptotic speed](#radial-schwarzschild-escape-with-asymptotic-speed)
    - [Marginal escape geodesic in Schwarzschild spacetime](#marginal-escape-geodesic-in-schwarzschild-spacetime)
- [Timelike circular Schwarzschild geodesic](#timelike-circular-schwarzschild-geodesic)
  - [Marginally bound circular Schwarzschild orbit](#marginally-bound-circular-schwarzschild-orbit)
  - [Schwarzschild circular-orbit local speed](#schwarzschild-circular-orbit-local-speed)
  - [Face-on frequency shift of a circular Schwarzschild source](#face-on-frequency-shift-of-a-circular-schwarzschild-source)
  - [Comparison of circular-orbit and static Schwarzschild clocks](#comparison-of-circular-orbit-and-static-schwarzschild-clocks)
    - [Schwarzschild circular-ring energy shift](#schwarzschild-circular-ring-energy-shift)
      - [Edge-on Schwarzschild ISCO redshift envelope](#edge-on-schwarzschild-isco-redshift-envelope)
- [Schwarzschild radial fall from rest at a finite radius](#schwarzschild-radial-fall-from-rest-at-a-finite-radius)
  - [Finite pulse count for a falling Schwarzschild beacon](#finite-pulse-count-for-a-falling-schwarzschild-beacon)
- [Proper-time bound inside a Schwarzschild black hole](#proper-time-bound-inside-a-schwarzschild-black-hole)
- [Horizon redshift of a Schwarzschild infaller](#horizon-redshift-of-a-schwarzschild-infaller)
- [Schwarzschild time](#schwarzschild-time)
- [Kruskal spacetime](#kruskal-spacetime)
  - [Non-traversability of the Schwarzschild bridge](#non-traversability-of-the-schwarzschild-bridge)
  - [Kruskal diagram](#kruskal-diagram)
  - [Radial timelike incompleteness in Kruskal spacetime](#radial-timelike-incompleteness-in-kruskal-spacetime)
- [Negative heat capacity of a Schwarzschild black hole](#negative-heat-capacity-of-a-schwarzschild-black-hole)
- [Ultrarelativistic limit of the boosted Schwarzschild metric away from the null plane](#ultrarelativistic-limit-of-the-boosted-schwarzschild-metric-away-from-the-null-plane)
- [Schwarzschild-de Sitter spacetime](#schwarzschild-de-sitter-spacetime)
  - [Radial geodesic acceleration in Schwarzschild-de Sitter spacetime](#radial-geodesic-acceleration-in-schwarzschild-de-sitter-spacetime)
- [Geodetic effect](#geodetic-effect)
- [Painlevé–Gullstrand coordinates](#painleve-gullstrand-coordinates)
  - [Domain of the ingoing Painleve-Gullstrand chart](#domain-of-the-ingoing-painleve-gullstrand-chart)
  - [Free-fall proper time in Schwarzschild spacetime](#free-fall-proper-time-in-schwarzschild-spacetime)
    - [Schwarzschild horizon-to-singularity proper time for fall from infinity](#schwarzschild-horizon-to-singularity-proper-time-for-fall-from-infinity)
  - [Orthonormal coframe in Painlevé–Gullstrand coordinates](#orthonormal-coframe-in-painleve-gullstrand-coordinates)
- [Radial Weyl curvature of Schwarzschild spacetime](#radial-weyl-curvature-of-schwarzschild-spacetime)
  - [Schwarzschild tidal force](#schwarzschild-tidal-force)
  - [Tidal gravity and the equivalence principle](#tidal-gravity-and-the-equivalence-principle)
- [Equatorial null orbit in Schwarzschild spacetime](#equatorial-null-orbit-in-schwarzschild-spacetime)
  - [Finite-azimuth Schwarzschild photon plunge](#finite-azimuth-schwarzschild-photon-plunge)
    - [Affine-time scaling of a nonradial Schwarzschild photon plunge](#affine-time-scaling-of-a-nonradial-schwarzschild-photon-plunge)
  - [Null effective potential in Schwarzschild spacetime](#null-effective-potential-in-schwarzschild-spacetime)
  - [Critical photon orbits of Schwarzschild spacetime](#critical-photon-orbits-of-schwarzschild-spacetime)
  - [Circular null geodesic](#circular-null-geodesic)
    - [Photon sphere](#photon-sphere)
      - [Schwarzschild photon escape cone](#schwarzschild-photon-escape-cone)
      - [Photon capture cross-section of a Reissner-Nordstrom black hole](#photon-capture-cross-section-of-a-reissner-nordstrom-black-hole)
- [Schwarzschild radius](#schwarzschild-radius)
- [Schwarzschild tortoise coordinate](#schwarzschild-tortoise-coordinate)
  - [Outgoing Eddington-Finkelstein coordinates](#outgoing-eddington-finkelstein-coordinates)
  - [Ingoing Eddington-Finkelstein coordinates](#ingoing-eddington-finkelstein-coordinates)
    - [Finkelstein diagram](#finkelstein-diagram)
    - [Radial null trajectories in ingoing Eddington-Finkelstein coordinates](#radial-null-trajectories-in-ingoing-eddington-finkelstein-coordinates)
- [Schwarzschild event horizon](#schwarzschild-event-horizon)
  - [Schwarzschild horizon collision energy](#schwarzschild-horizon-collision-energy)
- [Schwarzschild singularity](#schwarzschild-singularity)
- [Kruskal–Szekeres coordinates](#kruskal-szekeres-coordinates)
  - [Kruskal extension across a simple static horizon](#kruskal-extension-across-a-simple-static-horizon)
  - [Schwarzschild geodesic from the bifurcation sphere to the singularity](#schwarzschild-geodesic-from-the-bifurcation-sphere-to-the-singularity)
- [Gravitational redshift between static Schwarzschild observers](#gravitational-redshift-between-static-schwarzschild-observers)
- [Proper acceleration of a static Schwarzschild observer](#proper-acceleration-of-a-static-schwarzschild-observer)
- [Birkhoff's theorem](#birkhoff-s-theorem)
  - [Redshifted gravitational mass of a static thin shell](#redshifted-gravitational-mass-of-a-static-thin-shell)
- [Schwarzschild light deflection](#schwarzschild-light-deflection)
  - [Eddington experiment](#eddington-experiment)
  - [Perturbative derivation of Schwarzschild light deflection](#perturbative-derivation-of-schwarzschild-light-deflection)

## Coordinate invariance of the Schwarzschild photon radial potential

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

A stationary time-coordinate change $t'=t+F(r)$ leaves both the [areal radius](general-relativity.md#areal-radius) and the time-translation [Killing vector field](killing-vector-field.md) unchanged. The conserved [Killing energy](killing-vector-field.md#killing-energy) and [angular momentum](momentum.md#angular-momentum) of a [null geodesic](special-relativity.md#null-geodesic) therefore yield the same radial equation in either chart, $\dot r^2+h^2(1-2\mu/r)/r^2=c^2k^2$. The [effective potential](mathematical-physics.md#effective-potential) and radial [turning points](energy.md#turning-point) agree, even when the coordinate time velocities and horizon regularity differ.

## Schwarzschild static observer

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

An observer at fixed exterior Schwarzschild spatial coordinates. Its [proper time](special-relativity.md#proper-time) is $dT=\sqrt f\,dt$, with $f=1-2GM/(rc^2)>0$. It is accelerated, not freely falling; no such static timelike [worldline](special-relativity.md#world-line) exists on or inside the [event horizon](black-hole.md#event-horizon).

### Local radial speed of a Schwarzschild geodesic

↑ **Parent:** [Schwarzschild static observer](#schwarzschild-static-observer)

For a radial [timelike geodesic](general-relativity.md#timelike-geodesic) of specific [Killing energy](killing-vector-field.md#killing-energy) $k=f\,dt/d\tau$, the static observer measures $v_{\rm loc}=(dr/dt)/f=\dot r/k$. Its relative [Lorentz factor](special-relativity.md#lorentz-factor) is $k/\sqrt f$, giving $v_{\rm loc}^2=c^2(1-f/k^2)$.

#### Radial Schwarzschild escape with asymptotic speed

↑ **Parent:** [Local radial speed of a Schwarzschild geodesic](#local-radial-speed-of-a-schwarzschild-geodesic)

For asymptotic [speed](classical-mechanics.md#speed) $0\le u<c$, $k=(1-u^2/c^2)^{-1/2}$ and the local outward [speed](classical-mechanics.md#speed) obeys $v_{\rm loc}^2=u^2+(2GM/r)(1-u^2/c^2)$. It tends to $c$ as the horizon is approached from outside, though a static observer cannot actually remain on the horizon.

#### Marginal escape geodesic in Schwarzschild spacetime

↑ **Parent:** [Local radial speed of a Schwarzschild geodesic](#local-radial-speed-of-a-schwarzschild-geodesic)

The outgoing radial [timelike geodesic](general-relativity.md#timelike-geodesic) with zero [speed](classical-mechanics.md#speed) at infinity has $k=1$ and $dr/d\tau=\sqrt{2GM/r}$. Thus $r(\tau)=[r_0^{3/2}+(3/2)\sqrt{2GM}\tau]^{2/3}$ and the local static-observer [speed](classical-mechanics.md#speed) is $\sqrt{2GM/r}$.

## Timelike circular Schwarzschild geodesic

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

For the [Schwarzschild metric](schwarzschild-spacetime.md) with $\mu=GM/c^2$, let $k=(1-2\mu/r)\dot t$ and $h=r^2\dot\phi$ on an equatorial [timelike geodesic](general-relativity.md#timelike-geodesic). The normalization of the [four-velocity](special-relativity.md#four-velocity) gives $\dot r^2+V(r)=c^2(k^2-1)$, where $V(r)=(1-2\mu/r)h^2/r^2-2\mu c^2/r$. A circular [geodesic](riemannian-geometry.md#geodesic) obeys $V'(R)=0$, giving the displayed constants and requiring $R>3\mu$. Its coordinate [angular velocity](rigid-body-dynamics.md#angular-velocity) is $\Omega^2=GM/R^3$, and its proper clock rate is $d\tau/dt=\sqrt{1-3\mu/R}$. Differentiating $V$ twice at the circular solution gives stability for $R>6\mu$.

### Marginally bound circular Schwarzschild orbit

↑ **Parent:** [Timelike circular Schwarzschild geodesic](#timelike-circular-schwarzschild-geodesic)

The circular timelike orbit with conserved [energy](energy.md) equal to [rest energy](special-relativity.md#rest-energy) at infinity. Substituting $E/(mc^2)=(1-2\mu/r)/\sqrt{1-3\mu/r}$ and solving $E=mc^2$ gives $r=4\mu$, with $\mu=GM/c^2$. It is unstable. Strictly bound circular orbits have $r>4\mu$ and $E<mc^2$; radial stability requires $r>6\mu$. This limiting orbit is not the smallest radius ever reached by a bound-energy plunging trajectory.

### Schwarzschild circular-orbit local speed

↑ **Parent:** [Timelike circular Schwarzschild geodesic](#timelike-circular-schwarzschild-geodesic)

A [Schwarzschild static observer](#schwarzschild-static-observer) at a circular orbit measures speed $v_{\rm loc}=r(d\phi/dt)/\sqrt{1-2\mu/r}$. Combining the circular [geodesic](riemannian-geometry.md#geodesic) [frequency](wave.md#frequency) with this clock rate gives the displayed formula. The observer-relative [Lorentz factor](special-relativity.md#lorentz-factor) is $\gamma=\sqrt{(r-2\mu)/(r-3\mu)}$, and $r\,d\phi/d\tau=\gamma v_{\rm loc}$. Thus the local speed is $c/2$ at the Schwarzschild [innermost stable circular orbit](astrophysical-black-hole.md#innermost-stable-circular-orbit). Coordinate and locally measured speeds are distinct.

### Face-on frequency shift of a circular Schwarzschild source

↑ **Parent:** [Timelike circular Schwarzschild geodesic](#timelike-circular-schwarzschild-geodesic)

A source on a [timelike circular Schwarzschild geodesic](#timelike-circular-schwarzschild-geodesic) at radius $r>3GM/c^2$ emits light to a static observer at infinity on the orbital symmetry axis. Such a ray has zero conserved axial [angular momentum](momentum.md#angular-momentum). The locally measured photon [energy](energy.md) is the contraction of its [four-momentum](special-relativity.md#four-momentum) with the observer's [four-velocity](special-relativity.md#four-velocity). Comparing the emitter with the observer at infinity therefore gives $\nu_{\rm em}=U^t\nu_\infty$, where $U^t=[1-3GM/(c^2r)]^{-1/2}$, proving the formula.

Equivalently the [gravitational redshift](general-relativity.md#gravitational-redshift) factor $\sqrt{1-2GM/(c^2r)}$ multiplies the transverse [Doppler effect](wave.md#doppler-effect) factor $1/\gamma$ measured by a local static observer. For $R_S=2GM/c^2\ll r$,

$$
\nu_{\rm em}=\nu_\infty\left[1+\frac{3R_S}{4r}+O\!\left(\frac{R_S^2}{r^2}\right)\right].
$$

The coefficient contains both gravitational and orbital time dilation. It assumes an observer at infinity on the symmetry axis; other viewing directions generally introduce a first-order longitudinal [Doppler effect](wave.md#doppler-effect).

### Comparison of circular-orbit and static Schwarzschild clocks

↑ **Parent:** [Timelike circular Schwarzschild geodesic](#timelike-circular-schwarzschild-geodesic)

A clock following a [timelike circular Schwarzschild geodesic](#timelike-circular-schwarzschild-geodesic) of [radius](topology.md#radius) $R_s$ advances at $\sqrt{1-3\mu/R_s}$ per unit Schwarzschild coordinate time. A static clock at [radius](topology.md#radius) $R_E>2\mu$ advances at $\sqrt{1-2\mu/R_E}$. Their ratio over the same coordinate-time interval gives the displayed result. For periodic signal comparisons, successive corresponding signals must also have the same propagation delay, as happens for repeated overhead passages in a fixed circular orbit observed from a static pole. To first order in $\mu/R$, the ratio is $1+\mu/R_E-3\mu/(2R_s)$.

#### Schwarzschild circular-ring energy shift

↑ **Parent:** [Comparison of circular-orbit and static Schwarzschild clocks](#comparison-of-circular-orbit-and-static-schwarzschild-clocks)

For the receding edge of a circular emitter ring, the direct-projection model gives $1+z=(1-3r_g/r)^{-1/2}[1+\sqrt{r_g/(r-2r_g)}\sin i]$, with $r_g=GM/c^2$. Gravitational and transverse shifts combine with the line-of-sight [Doppler factor](special-relativity.md#doppler-factor). Mapping the distant inclination directly to a local [photon](quantum-mechanics.md#photon) direction neglects gravitational ray bending.

##### Edge-on Schwarzschild ISCO redshift envelope

↑ **Parent:** [Schwarzschild circular-ring energy shift](#schwarzschild-circular-ring-energy-shift)

At $r=6r_g$, the local circular speed is $c/2$, so the receding direct-projection shift is $\sqrt2(1+\sin i/2)$. The upper envelope over inclinations is $3/\sqrt2$. It is not the shift for a face-on or arbitrary azimuthal emitter, and it excludes plunging-region emission and ray-tracing corrections.

## Schwarzschild radial fall from rest at a finite radius

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

For radial timelike [geodesic](riemannian-geometry.md#geodesic) fall released from rest at $r_0>2M$, the [Killing energy](killing-vector-field.md#killing-energy) is $E=\sqrt{1-2M/r_0}$ and the [proper time](special-relativity.md#proper-time) radial equation is $(dr/ds)^2=2M/r-2M/r_0$. The displayed parameterization integrates its inward branch, with $s=0$ at release. The [Schwarzschild event horizon](#schwarzschild-event-horizon) is reached at $\eta_H=\arccos(4M/r_0-1)$ in finite proper time, even though [Schwarzschild time](#schwarzschild-time) diverges.

// Target: general-relativity.bigb

### Finite pulse count for a falling Schwarzschild beacon

↑ **Parent:** [Schwarzschild radial fall from rest at a finite radius](#schwarzschild-radial-fall-from-rest-at-a-finite-radius)

A freely falling source emits [optical pulses](optics.md#optical-pulse) at proper times $\delta+nP$, for integers $n\ge0$. If its horizon-crossing [proper time](special-relativity.md#proper-time) is finite, only pulses beginning before $s_H$ can escape. Their number is the displayed ceiling, for $0\le\delta<P<s_H$. Infinite [Schwarzschild time](#schwarzschild-time) at crossing does not give infinitely many emitted pulses. The pulse phase $\delta$ fixes both the count and the redshift of the last pulse. If a finite pulse straddles the horizon, its exterior portion has an arbitrarily late, increasingly redshifted received tail.

## Proper-time bound inside a Schwarzschild black hole

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

Inside the future black-hole region, the radius decreases along every future-directed timelike path. Its unit tangent obeys $|dr/ds|\geq\sqrt{2M/r-1}$ from the metric normalization, independently of radial acceleration or angular motion. Integrating from $r_0<2M$ to zero gives the displayed finite upper bound. The statement concerns future continuation within the black-hole region; reversing time in the white-hole region reverses the radial direction.

## Horizon redshift of a Schwarzschild infaller

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

For smooth radial infall through a future [Schwarzschild event horizon](#schwarzschild-event-horizon), outgoing retarded time obeys $u\sim-4M\log(\tau_H-\tau)$. A distant observer sees the [redshift](optics.md#redshift) grow as $e^{t_{\rm rec}/(4M)}$. Its exponent in emission [Schwarzschild time](#schwarzschild-time) is instead $1/(2M)$, because $t_{\rm rec}\sim2t_{\rm em}$. At finite fixed observer radius the wavelength ratio includes $\sqrt{1-2M/r_B}$.

## Schwarzschild time

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

[Schwarzschild time](#schwarzschild-time) $t$ is the exterior time coordinate normalized to the [proper time](special-relativity.md#proper-time) of static observers at infinity. At fixed exterior radius, $d\tau=\sqrt{1-2M/r}\,dt$. A received signal and its emission occur at different values of this coordinate.

## Kruskal spacetime

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

The [Kruskal spacetime](#kruskal-spacetime) is the maximal analytic extension of the positive-mass vacuum [Schwarzschild spacetime](schwarzschild-spacetime.md). It contains two exterior regions, a [black hole](black-hole.md), and a [white hole](black-hole.md#white-hole). [Kruskal–Szekeres coordinates](#kruskal-szekeres-coordinates) remove both horizon coordinate singularities, while $r=0$ remains a [curvature singularity](general-relativity.md#curvature-singularity).

### Non-traversability of the Schwarzschild bridge

↑ **Parent:** [Kruskal spacetime](#kruskal-spacetime)

In [Kruskal–Szekeres coordinates](#kruskal-szekeres-coordinates), every future-directed radial causal curve has nondecreasing $U$ and $V$. The right exterior has $U<0,V>0$, while the left has $U>0,V<0$. No future-directed causal curve can travel between the exteriors because it would have to decrease one null coordinate. The spatial bridge on a time-symmetric slice is therefore not a traversable passage.

### Kruskal diagram

↑ **Parent:** [Kruskal spacetime](#kruskal-spacetime)

This radial spacetime diagram uses [Kruskal–Szekeres coordinates](#kruskal-szekeres-coordinates) to display both exteriors, the black hole and the white hole of maximally extended [Schwarzschild spacetime](schwarzschild-spacetime.md). Each point represents a symmetry two-sphere. Radial [null geodesics](special-relativity.md#null-geodesic) have slopes $\pm1$ in the displayed coordinates; the horizons are $T_K=\pm X_K$ and the singularities satisfy $T_K^2-X_K^2=1$ in the usual normalization. A further compactification gives the corresponding [Penrose diagram](black-hole.md#penrose-diagram).

### Radial timelike incompleteness in Kruskal spacetime

↑ **Parent:** [Kruskal spacetime](#kruskal-spacetime)

Every maximal radial [timelike geodesic](general-relativity.md#timelike-geodesic) in positive-mass [Kruskal spacetime](#kruskal-spacetime) is incomplete in at least one direction. Its equations are $\dot r^2=E^2-1+2M/r$ and $\ddot r=-M/r^2$. A finite turning point is a maximum, and each trajectory reaches $r=0$ at one or both ends. The remaining [proper time](special-relativity.md#proper-time) is finite because $d\tau\sim\sqrt{r/(2M)}\,dr$. Complete circular timelike geodesics exist, but they have nonzero [angular momentum](momentum.md#angular-momentum).

## Negative heat capacity of a Schwarzschild black hole

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

In units $G=\hbar=c=k_B=1$, a [Schwarzschild black hole](schwarzschild-spacetime.md) has [Hawking temperature](black-hole.md#hawking-temperature) $T=1/(8\pi M)$, so its [heat capacity](heat.md#heat-capacity) is $dM/dT=-8\pi M^2$. It heats up as it loses [mass](classical-mechanics.md#mass), preventing stable canonical equilibrium with an unlimited thermal reservoir.

## Ultrarelativistic limit of the boosted Schwarzschild metric away from the null plane

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

Boost a Schwarzschild mass with speed $v$ and hold $p=m\gamma$ fixed as $v\to1$. Away from the null plane $x=t$, the isotropic-coordinate expression tends to

$$
ds^2=ds_{\rm Minkowski}^2+\frac{4p}{|x-t|}(dt-dx)^2.
$$

The complete distributional limit on the null plane requires the additional coordinate treatment that produces the Aichelburg-Sexl shock wave.

## Schwarzschild-de Sitter spacetime

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schwarzschild-de_Sitter_spacetime)

The Schwarzschild-de Sitter spacetime is the spherically symmetric vacuum solution with positive [cosmological constant](cosmology.md#cosmological-constant). In static coordinates its metric function is $f(r)=1-2m/r-H^2r^2$, with a black-hole horizon and a cosmological horizon when $mH<1/\sqrt{27}$.

### Radial geodesic acceleration in Schwarzschild-de Sitter spacetime

↑ **Parent:** [Schwarzschild-de Sitter spacetime](#schwarzschild-de-sitter-spacetime)

For $ds^2=A\,dt^2-dr^2/A-r^2d\Omega^2$, $A=1-2GM/r-\Lambda r^2/3$, and $c=1$, a radial timelike [geodesic](riemannian-geometry.md#geodesic) has $\dot r^2=k^2-A$. The radial [geodesic equation](riemannian-geometry.md#geodesic-equation) gives $\ddot r=-A'/2=-GM/r^2+\Lambda r/3$, including at a [turning point](energy.md#turning-point). This is a second [derivative](calculus.md#derivative) of the [areal radius](general-relativity.md#areal-radius) with respect to [proper time](special-relativity.md#proper-time); the [geodesic](riemannian-geometry.md#geodesic)'s [four-acceleration](special-relativity.md#four-acceleration) still vanishes. In the slow-motion weak-field limit, restoring units gives $d^2r/dt^2=-GM/r^2+\Lambda c^2r/3$.

## Geodetic effect

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geodetic_effect)

Geodetic precession is the rotation of a parallel-transported gyroscope relative to the orbital radial direction in curved spacetime. For a circular Schwarzschild orbit its exact precession per revolution is $2\pi[1-\sqrt{1-3M/R}]$.

<h2 id="painleve-gullstrand-coordinates">Painlevé–Gullstrand coordinates</h2>

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Painlevé–Gullstrand_coordinates)

Painlevé–Gullstrand coordinates write the Schwarzschild metric as

$$
ds^2=-dt^2+\left(dr+\sqrt{\frac{2M}{r}}\,dt\right)^2+r^2d\Omega^2.
$$

The constant-$t$ spatial slices are flat, and the coordinates remain regular at the [Schwarzschild radius](#schwarzschild-radius).

### Domain of the ingoing Painleve-Gullstrand chart

↑ **Parent:** [Painlevé–Gullstrand coordinates](#painleve-gullstrand-coordinates)

Choose [Kruskal–Szekeres coordinates](#kruskal-szekeres-coordinates) with the right exterior at $U<0,V>0$ and $UV=(1-r/(2M))e^{r/(2M)}$. The ingoing [Painlevé–Gullstrand coordinates](#painleve-gullstrand-coordinates) cover that exterior and the future black-hole region $U>0,V>0$, together with their common future horizon. They exclude the other exterior, the white hole, the bifurcation sphere and the singularity. Indeed $\tau=v+F(r)-r_*(r)$, with $v=4M\log V$ and $F'=\sqrt{2M/r}/f$; the difference $F-r_*$ is finite at $r=2M$, whereas $V=0$ requires infinite coordinate time.

### Free-fall proper time in Schwarzschild spacetime

↑ **Parent:** [Painlevé–Gullstrand coordinates](#painleve-gullstrand-coordinates)

The inward radial [geodesic congruence](geodesic-congruence.md) with unit [Killing energy](killing-vector-field.md#killing-energy) has $U=f^{-1}\partial_t-\sqrt{2M/r}\,\partial_r$, where $f=1-2M/r$. Its metric dual is $U^\flat=-d\tau$, so $\tau$ is a synchronized [proper time](special-relativity.md#proper-time) for the congruence. Locally $\tau=t+2\sqrt{2Mr}+2M\log| (\sqrt r-\sqrt{2M})/(\sqrt r+\sqrt{2M}) |$. This yields [Painlevé–Gullstrand coordinates](#painleve-gullstrand-coordinates) with flat spatial slices and a regular future horizon.

#### Schwarzschild horizon-to-singularity proper time for fall from infinity

↑ **Parent:** [Free-fall proper time in Schwarzschild spacetime](#free-fall-proper-time-in-schwarzschild-spacetime)

A radial observer released from rest at infinity has $dr/d\tau=-\sqrt{2M/r}$. Integration from $r=2M$ to $r=0$ gives $\Delta\tau=\int_0^{2M}\sqrt{r/(2M)}dr=4M/3$ in geometric units. In ordinary units it is $4GM/(3c^3)$. The endpoint is the curvature singularity, not a regular spacetime centre; this value belongs to that specified energy, not every possible infalling worldline.

<h3 id="orthonormal-coframe-in-painleve-gullstrand-coordinates">Orthonormal coframe in Painlevé–Gullstrand coordinates</h3>

↑ **Parent:** [Painlevé–Gullstrand coordinates](#painleve-gullstrand-coordinates)

An orthonormal coframe is

$$
e^0=dt,
\qquad e^1=dr+\sqrt{\frac{2M}{r}}\,dt,
\qquad e^2=r\,d\theta,
\qquad e^3=r\sin\theta\,d\phi.
$$

## Radial Weyl curvature of Schwarzschild spacetime

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

With the curvature convention

$$
R^\alpha{}_{\beta\gamma\delta}
=\partial_\gamma\Gamma^\alpha_{\beta\delta}
-\partial_\delta\Gamma^\alpha_{\beta\gamma}+\cdots,
$$

the vacuum Schwarzschild metric satisfies

$$
C_{trtr}=R_{trtr}=-\frac{2M}{r^3}.
$$

The opposite Riemann-sign convention reverses this sign.

### Schwarzschild tidal force

↑ **Parent:** [Radial Weyl curvature of Schwarzschild spacetime](#radial-weyl-curvature-of-schwarzschild-spacetime)

The orthonormal-frame components of Schwarzschild curvature scale as $M/r^3$. The [geodesic deviation](riemann-curvature-tensor.md#geodesic-deviation) equation therefore gives radial stretching and transverse compression whose magnitude diverges as $r\to0$.

### Tidal gravity and the equivalence principle

↑ **Parent:** [Radial Weyl curvature of Schwarzschild spacetime](#radial-weyl-curvature-of-schwarzschild-spacetime)

Weyl curvature produces relative acceleration between neighbouring freely falling trajectories and therefore tidal deformation. A freely falling frame removes gravity at one event, as required by the equivalence principle, but cannot remove curvature over an extended region.

## Equatorial null orbit in Schwarzschild spacetime

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

For inverse radius $y=1/r$ and azimuth $\phi$, a Schwarzschild null geodesic obeys

$$
(y')^2+y^2-2My^3=\frac1{b^2},
\qquad
y''+y=3My^2,
$$

where $b=L/E$ is the [impact parameter](classical-mechanics.md#impact-parameter).

### Finite-azimuth Schwarzschild photon plunge

↑ **Parent:** [Equatorial null orbit in Schwarzschild spacetime](#equatorial-null-orbit-in-schwarzschild-spacetime)

For a captured nonradial [null geodesic](special-relativity.md#null-geodesic) with $u=1/r$, the large-$u$ orbit equation is $(du/d\phi)^2\sim2\mu u^3$. Integration on the inward branch gives

$$
\phi_*-\phi\sim\sqrt{2/(\mu u)},\qquad
r\sim\frac\mu2(\phi_*-\phi)^2.
$$

The [curvature singularity](general-relativity.md#curvature-singularity) is reached at finite azimuth. This does not prevent a near-critical ray from winding repeatedly near the [photon sphere](#photon-sphere) before its final plunge. A radial ray has constant azimuth, so this asymptotic coordinate parametrization is inapplicable to it.

#### Affine-time scaling of a nonradial Schwarzschild photon plunge

↑ **Parent:** [Finite-azimuth Schwarzschild photon plunge](#finite-azimuth-schwarzschild-photon-plunge)

For nonzero angular constant $h$, the interior null radial equation gives $\dot r^2\sim2\mu h^2/r^3$. Its inward branch integrates to $r^{5/2}\sim\tfrac52\sqrt{2\mu}|h|(\lambda_*-\lambda)$. Thus the singularity is at finite [affine parameter](riemannian-geometry.md#affine-parameter) and $r\propto(\lambda_*-\lambda)^{2/5}$. The zero-angular-momentum case has a different affine scaling.

### Null effective potential in Schwarzschild spacetime

↑ **Parent:** [Equatorial null orbit in Schwarzschild spacetime](#equatorial-null-orbit-in-schwarzschild-spacetime)

For an equatorial [null geodesic](special-relativity.md#null-geodesic) in [Schwarzschild spacetime](schwarzschild-spacetime.md), let $k=(1-2\mu/r)\,dt/d\lambda$ and $h=r^2d\phi/d\lambda$ be the conserved quantities for an [affine parameter](riemannian-geometry.md#affine-parameter) $\lambda$. The null [metric](topological-analysis.md#metric) condition gives $\dot r^2/2+V_{\rm eff}=c^2k^2/2$. For $h\ne0$, the [effective potential](mathematical-physics.md#effective-potential) is zero at the [Schwarzschild event horizon](#schwarzschild-event-horizon), positive outside, and tends to zero at infinity. Its unique exterior maximum is at $r=3\mu$, with value $h^2/(54\mu^2)$ and second [derivative](calculus.md#derivative) $-h^2/(81\mu^4)$. This maximum gives the unstable [photon sphere](#photon-sphere).

The [impact parameter](classical-mechanics.md#impact-parameter) of an incoming ray is $b=|h|/(ck)$ for $k>0$. Capture requires its radial energy to exceed the maximum, namely $b<3\sqrt3\mu$. At equality the incoming ray approaches the circular orbit asymptotically; it does not cross the horizon. For $h=0$, the potential is identically zero and the ingoing radial ray is captured.

### Critical photon orbits of Schwarzschild spacetime

↑ **Parent:** [Equatorial null orbit in Schwarzschild spacetime](#equatorial-null-orbit-in-schwarzschild-spacetime)

At the critical [impact parameter](classical-mechanics.md#impact-parameter) $b=3\sqrt3M$, the null orbit equation factors as $(u')^2=(u-1/3)^2(2u+1/3)$ for $u=M/r$. One oriented family has the displayed solution. As $\phi\to-\infty$, positive $A$ approaches the [photon sphere](#photon-sphere) from larger radii and negative $A$ from smaller radii; $A=0$ is the circular orbit. The physical domain must retain $r>0$ and the positive square root in its implicit parametrization.

### Circular null geodesic

↑ **Parent:** [Equatorial null orbit in Schwarzschild spacetime](#equatorial-null-orbit-in-schwarzschild-spacetime)

A circular null geodesic remains at constant areal radius. It lies at a stationary point of the null radial effective potential and may be stable or unstable according to the sign of the second derivative there.

#### Photon sphere

↑ **Parent:** [Circular null geodesic](#circular-null-geodesic)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Photon_sphere)

A photon sphere is a spherical set of circular [null geodesics](special-relativity.md#null-geodesic). In [Schwarzschild spacetime](schwarzschild-spacetime.md) it occurs at $r=3M$ and is unstable.

##### Schwarzschild photon escape cone

↑ **Parent:** [Photon sphere](#photon-sphere)

At $2\mu<r\le3\mu$, measure the emission [angle](geometry-and-topology.md#angle) $\alpha$ from the outward radial direction in a static observer's [orthonormal tetrad](general-relativity.md#orthonormal-frame-in-spacetime). Local [photon](quantum-mechanics.md#photon) energy is $E_{\rm loc}=E_\infty/\sqrt{1-2\mu/r}$, and its tangential [momentum](momentum.md) is $E_{\rm loc}\sin\alpha/c$. Thus its [impact parameter](classical-mechanics.md#impact-parameter) is $b=r\sin\alpha/\sqrt{1-2\mu/r}$. Combining this with the [null effective potential in Schwarzschild spacetime](#null-effective-potential-in-schwarzschild-spacetime) gives escape precisely for outward directions $0\le\alpha<\alpha_{\rm crit}$; the limiting ray approaches the [photon sphere](#photon-sphere) and does not escape.

As $r\downarrow2\mu$ the cone shrinks to zero opening. A static observer does not exist on the horizon itself, and no future-directed ray starting on the [Schwarzschild event horizon](#schwarzschild-event-horizon) reaches exterior infinity. At $r=3\mu$, the critical half-angle is $\pi/2$; the exactly tangential critical ray stays on the unstable circular orbit. Escape cones for a moving observer are changed by [relativistic aberration](mathematical-physics.md#relativistic-aberration).

##### Photon capture cross-section of a Reissner-Nordstrom black hole

↑ **Parent:** [Photon sphere](#photon-sphere)

For a [Reissner-Nordstrom black hole](black-hole.md#reissner-nordstrom-spacetime) with $|Q|\le M$, the outer unstable [circular null geodesic](#circular-null-geodesic) has radius $r_{\mathrm{ph}}=(3M+\sqrt{9M^2-8Q^2})/2$. Maximizing $f/r^2$ for $f=1-2M/r+Q^2/r^2$ gives the critical [impact parameter](classical-mechanics.md#impact-parameter) $b_c^2=r_{\mathrm{ph}}^2/f(r_{\mathrm{ph}})=2r_{\mathrm{ph}}^3/(r_{\mathrm{ph}}-M)$. The [geometrical optics](geometrical-optics.md) capture cross-section is $\pi b_c^2$, reducing to $27\pi M^2$ in [Schwarzschild spacetime](schwarzschild-spacetime.md) and $16\pi M^2$ in the extremal charged case. Finite-wavelength absorption need not equal this geometric limit.

// Target: general-relativity.bigb

## Schwarzschild radius

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schwarzschild_radius)

The Schwarzschild radius is $r_s=2GM/c^2$, or $2M$ in geometrized units.

## Schwarzschild tortoise coordinate

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

The tortoise coordinate satisfies

$$
\frac{dr_*}{dr}=\left(1-\frac{2M}{r}\right)^{-1},
\qquad
r_*=r+2M\log\left|\frac{r}{2M}-1\right|.
$$

### Outgoing Eddington-Finkelstein coordinates

↑ **Parent:** [Schwarzschild tortoise coordinate](#schwarzschild-tortoise-coordinate)

The retarded coordinate $u=t-r_*$ puts the radial [Schwarzschild metric](schwarzschild-spacetime.md) into $ds^2=-f\,du^2-2\,du\,dr+r^2d\Omega^2$, with $f=1-2M/r$. Outgoing radial [null geodesics](special-relativity.md#null-geodesic) have constant $u$. These coordinates are regular at the past horizon; an infaller crossing the future horizon has $u\to+\infty$.

### Ingoing Eddington-Finkelstein coordinates

↑ **Parent:** [Schwarzschild tortoise coordinate](#schwarzschild-tortoise-coordinate)

The advanced coordinate $v=t+r_*$ puts the radial Schwarzschild metric into the form

$$
ds^2=-\left(1-\frac{2M}{r}\right)dv^2+2\,dv\,dr+r^2d\Omega^2,
$$

which is regular at the future horizon.

These are the advanced, ingoing member of the [Eddington-Finkelstein coordinates](general-relativity.md#eddington-finkelstein-coordinates).

#### Finkelstein diagram

↑ **Parent:** [Ingoing Eddington-Finkelstein coordinates](#ingoing-eddington-finkelstein-coordinates)

A [Finkelstein diagram](#finkelstein-diagram) plots [areal radius](general-relativity.md#areal-radius) $r$ against $T=v-r$ in [ingoing Eddington-Finkelstein coordinates](#ingoing-eddington-finkelstein-coordinates). Its radial [null directions](special-relativity.md#null-directions) show explicitly that both future light-ray families decrease $r$ inside a [Schwarzschild black hole](schwarzschild-spacetime.md). It is not a compactified [Penrose diagram](black-hole.md#penrose-diagram).

#### Radial null trajectories in ingoing Eddington-Finkelstein coordinates

↑ **Parent:** [Ingoing Eddington-Finkelstein coordinates](#ingoing-eddington-finkelstein-coordinates)

Radial null curves comprise the ingoing family $v=\text{constant}$ and the outgoing family

$$
\frac{dr}{dv}=\frac12\left(1-\frac{2M}{r}\right).
$$

Outside the horizon the outgoing family moves to larger $r$; inside it both future-directed families move to smaller $r$.

## Schwarzschild event horizon

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

The surface $r=2M$ is the future event horizon of Schwarzschild spacetime. Its singularity in Schwarzschild coordinates is removable, whereas $r=0$ is a curvature singularity.

### Schwarzschild horizon collision energy

↑ **Parent:** [Schwarzschild event horizon](#schwarzschild-event-horizon)

For two equal-mass inward [timelike geodesics](general-relativity.md#timelike-geodesic) of unit specific [Killing energy](killing-vector-field.md#killing-energy), their invariant [center-of-mass energy](special-relativity.md#center-of-mass-energy) has this finite horizon limit. If both are captured from infinity, [Schwarzschild marginally bound capture](general-relativity.md#schwarzschild-marginally-bound-capture) gives $E_{\rm com}<m\sqrt{20}$, with $m\sqrt{20}$ a supremum. No such universal bound follows for particles prepared inside the angular-momentum barrier.

## Schwarzschild singularity

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

The Schwarzschild singularity is the spacelike curvature singularity at $r=0$. Curvature invariants and orthonormal tidal components diverge there.

<h2 id="kruskal-szekeres-coordinates">Kruskal–Szekeres coordinates</h2>

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kruskal–Szekeres_coordinates)

Kruskal–Szekeres coordinates extend the Schwarzschild solution smoothly through its future and past horizons. Constant Schwarzschild radius curves are hyperbolae, while the horizons are null lines through the bifurcation sphere.

### Kruskal extension across a simple static horizon

↑ **Parent:** [Kruskal–Szekeres coordinates](#kruskal-szekeres-coordinates)

For $ds^2=-fdt^2+dr^2/f+R^2d\Omega^2$, suppose $f$ and $R$ are analytic at $r_H$, $f(r_H)=0$, $f'(r_H)=2\kappa>0$ and $R(r_H)>0$. The [tortoise coordinate](black-hole.md#tortoise-coordinate) obeys the displayed expansion with analytic $h$. For $U=-e^{-\kappa(t-r_*)}$ and $V=e^{\kappa(t+r_*)}$ in the right exterior, $-UV=(r-r_H)e^{2\kappa h(r)}$ after fixing an additive constant. The inverse function theorem makes $r$ analytic in $UV$ through zero, while $ds^2=f\,dU\,dV/(\kappa^2UV)+R^2d\Omega^2$ has a finite nonzero radial coefficient there. This supplies the local analytic extension and its [bifurcate Killing horizon](general-relativity.md#bifurcate-killing-horizon).

### Schwarzschild geodesic from the bifurcation sphere to the singularity

↑ **Parent:** [Kruskal–Szekeres coordinates](#kruskal-szekeres-coordinates)

A radial geodesic orthogonal to the time-symmetric Kruskal slice starts at $r=2M$ with zero Schwarzschild energy and reaches $r=0$ after proper time $\pi M$.

## Gravitational redshift between static Schwarzschild observers

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

For static observers at radii $r_A$ and $r_B$, equal Schwarzschild-coordinate time intervals correspond to proper times $d\tau=\sqrt{1-2M/r}\,dt$. Hence

$$
\frac{\Delta\tau_B}{\Delta\tau_A}
=\sqrt{\frac{1-2M/r_B}{1-2M/r_A}}.
$$

This static-observer relation is a special case of [gravitational redshift](general-relativity.md#gravitational-redshift), not a definition of every gravitational frequency shift.

## Proper acceleration of a static Schwarzschild observer

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

A static observer at Schwarzschild radius $r>2M$ must maintain the outward [proper acceleration](special-relativity.md#proper-acceleration)

$$
a=\frac{M}{r^2\sqrt{1-2M/r}}.
$$

It approaches the Newtonian value $M/r^2$ at large radius and diverges at the horizon.

<h2 id="birkhoff-s-theorem">Birkhoff's theorem</h2>

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Birkhoff's_theorem_(relativity))

Every spherically symmetric vacuum solution of the Einstein field equation is locally a portion of Schwarzschild spacetime. In particular, a spherically symmetric body's exterior field depends only on its total mass.

### Redshifted gravitational mass of a static thin shell

↑ **Parent:** [Birkhoff's theorem](#birkhoff-s-theorem)

A thin spherical shell of proper surface mass density $\rho$ held at Schwarzschild radius $r_{\rm st}$ around mass $M$ contributes, to first order in its mass,

$$
\Delta M_\infty
=4\pi r_{\rm st}^2\rho\sqrt{1-\frac{2M}{r_{\rm st}}}
$$

to the exterior Schwarzschild mass parameter.

## Schwarzschild light deflection

↑ **Parent:** [Schwarzschild spacetime](schwarzschild-spacetime.md)

A null Schwarzschild geodesic with $b\gg r_s$ is deflected through $2r_s/b=4GM/(bc^2)$ to first order.

This is the leading spherical-mass deflection underlying a [gravitational lens](gravitational-lensing.md#gravitational-lens).

### Eddington experiment

↑ **Parent:** [Schwarzschild light deflection](#schwarzschild-light-deflection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eddington_experiment)

The 1919 [solar eclipse](astronomy.md#solar-eclipse) expeditions organized by [Frank Watson Dyson](astronomy.md#frank-watson-dyson) and [Arthur Eddington](astronomy.md#arthur-eddington) compared background-star positions near the obscured [Sun](stellar-astrophysics.md#sun) with reference photographs. The optical train used a slowly rotating flat mirror to send the light into a horizontal photographic telescope. A smaller telescope at Sobral provided a separate set of plates. Focus and plate-scale changes had to be distinguished from the radial pattern predicted by [Schwarzschild light deflection](#schwarzschild-light-deflection). The experiment therefore tested a spatial pattern and its amplitude, not merely whether a star image had moved.[1920 report of the 1919 observations](physics-bibliography.md#a-determination-of-the-deflection-of-light-by-the-sun-s-gravitational-field-by-frank-watson-dyson-and-others) [Equipment taken and the Sobral expedition: horizontal telescopes, tracking mirrors and reference plates](https://www.royalobservatorygreenwich.org/articles.php?article=1283)

### Perturbative derivation of Schwarzschild light deflection

↑ **Parent:** [Schwarzschild light deflection](#schwarzschild-light-deflection)

Writing $y=b^{-1}\sin\phi+\Delta y$ in $y''+y=3My^2$ and retaining first order in $M$ gives

$$
\Delta y''+\Delta y=\frac{3M}{2b^2}(1-\cos2\phi).
$$

The displacement of the outgoing zero is $4M/b$.

## ↑ Ancestors (4)

1. [General relativity](general-relativity.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (40)

- [Affine rescaling of a null geodesic tangent](riemannian-geometry.md#affine-rescaling-of-a-null-geodesic-tangent)
- [Causal structure of the magnetic dilaton black hole](einstein-field-equations.md#causal-structure-of-the-magnetic-dilaton-black-hole)
- [Einstein field equations](einstein-field-equations.md)
- [Gravitational time dilation](general-relativity.md#gravitational-time-dilation)
- [Kretschmann scalar](riemann-curvature-tensor.md#kretschmann-scalar)
- [Kruskal diagram](#kruskal-diagram)
- [Kruskal spacetime](#kruskal-spacetime)
- [Maximal analytic extension](special-relativity.md#maximal-analytic-extension)
- [Null effective potential in Schwarzschild spacetime](#null-effective-potential-in-schwarzschild-spacetime)
- [Outgoing pulse redshift from a radial Schwarzschild infaller](general-relativity.md#outgoing-pulse-redshift-from-a-radial-schwarzschild-infaller)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-40.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-72.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-62.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-62.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-62.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-66.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56.md#1/g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-51.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-52.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-311.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-347.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#37d/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3.md#37c/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3.md#37c/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3.md#37d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#37b/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-309.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-3.md#37e/a/solution)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2012/paper-1.md#1/solution)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2016/paper-1.md#1/solution)
- [Photon capture cross-section of a Reissner-Nordstrom black hole](#photon-capture-cross-section-of-a-reissner-nordstrom-black-hole)
- [Photon sphere](#photon-sphere)
- [Relativistic spherical accretion](astrophysical-black-hole.md#relativistic-spherical-accretion)
- [Riemannian Penrose inequality](black-hole.md#riemannian-penrose-inequality)
- [Schwarzschild conformal compactification](black-hole.md#schwarzschild-conformal-compactification)
- [Schwarzschild retarded null coordinate](general-relativity.md#schwarzschild-retarded-null-coordinate)
- [Weak-field photon-orbit validity](linearized-gravity.md#weak-field-photon-orbit-validity)
- [White hole](black-hole.md#white-hole)
