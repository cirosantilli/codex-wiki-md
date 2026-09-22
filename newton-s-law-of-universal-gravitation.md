# Newton's law of universal gravitation

↑ **Parent:** [Classical mechanics](classical-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Newton's_law_of_universal_gravitation)

[Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md) gives the attractive [force](force.md) between two [point masses](classical-mechanics.md#point-mass). With source [mass](classical-mechanics.md#mass) $M$ at the origin and relative [position](classical-mechanics.md#position) $\mathbf r$ of [mass](classical-mechanics.md#mass) $m$, write $r=|\mathbf r|>0$:

$$
\mathbf F_{M\to m}=-\frac{GMm}{r^3}\mathbf r,\qquad |\mathbf F_{M\to m}|=\frac{GMm}{r^2}.
$$

Here $G$ is the [gravitational constant](#gravitational-constant). The minus sign points toward $M$; the magnitude follows an [inverse-square law](physics.md#inverse-square-law), so doubling the separation quarters the [force](force.md). The opposite [force](force.md) on $M$ satisfies [Newton's third law](force.md#newton-s-third-law). [OpenStax: mutual gravitational forces](https://openstax.org/books/university-physics-volume-1/pages/13-1-newtons-law-of-universal-gravitation)

Both [masses](classical-mechanics.md#mass) accelerate. Applying [Newton's second law](force.md#newton-s-second-law) to each in the isolated [two-body problem](celestial-mechanics.md#two-body-problem) gives

$$
\ddot{\mathbf r}=-\frac{\mu}{r^3}\mathbf r,\qquad \mu=G(M+m).
$$

The relative [standard gravitational parameter](#standard-gravitational-parameter) includes both [masses](classical-mechanics.md#mass); replacing it by $GM$ requires the [test particle](classical-mechanics.md#test-particle) approximation $m\ll M$.

Historically, Newton's Book III, Proposition VII argues that gravitational attraction applies to all bodies and scales with their [masses](classical-mechanics.md#mass); its second corollary states the [inverse-square law](physics.md#inverse-square-law) for individual particles. [Newton, Principia, Book III, Proposition VII, Motte's 1729 translation](https://en.wikisource.org/wiki/The_Mathematical_Principles_of_Natural_Philosophy_(1729)/Proposition_7:_Gravity_tending_to_all_Bodies)

**Table of contents**

- [Axial and transverse gravity of a uniform rod](#axial-and-transverse-gravity-of-a-uniform-rod)
  - [Circular orbit perpendicular to a uniform rod](#circular-orbit-perpendicular-to-a-uniform-rod)
- [Gravitational-electrostatic balance of equal charged spheres](#gravitational-electrostatic-balance-of-equal-charged-spheres)
- [Free fall](#free-fall)
  - [Free fall in a constant gravitational field](#free-fall-in-a-constant-gravitational-field)
  - [Radial free fall from rest](#radial-free-fall-from-rest)
  - [Rotational deflection of a falling body](#rotational-deflection-of-a-falling-body)
    - [Equatorial Coriolis deflection in free fall](#equatorial-coriolis-deflection-in-free-fall)
- [Newtonian gravitational field](#newtonian-gravitational-field)
  - [Gravitational field of an infinite plane sheet](#gravitational-field-of-an-infinite-plane-sheet)
    - [Tidal water loading of a spring balance](#tidal-water-loading-of-a-spring-balance)
  - [Axial gravitational field of a uniform ring](#axial-gravitational-field-of-a-uniform-ring)
  - [Gravitational field of a finite uniform line segment](#gravitational-field-of-a-finite-uniform-line-segment)
  - [Gravitational field of an infinite uniform cylinder](#gravitational-field-of-an-infinite-uniform-cylinder)
    - [Plumb-line deflection from cylindrical gravity](#plumb-line-deflection-from-cylindrical-gravity)
    - [Diameter-rod oscillation in cylindrical gravity](#diameter-rod-oscillation-in-cylindrical-gravity)
  - [Gauss's law for gravity](#gauss-s-law-for-gravity)
  - [Uniform gravitational field in an off-center spherical cavity](#uniform-gravitational-field-in-an-off-center-spherical-cavity)
    - [Cavity equilibrium destabilized by a second void](#cavity-equilibrium-destabilized-by-a-second-void)
  - [Newtonian gravitational stress tensor](#newtonian-gravitational-stress-tensor)
    - [Gravitational stress contribution to angular-momentum transport](#gravitational-stress-contribution-to-angular-momentum-transport)
  - [Self-gravity](#self-gravity)
  - [Standard gravitational parameter](#standard-gravitational-parameter)
  - [Tidal tensor](#tidal-tensor)
    - [Newtonian tidal eigenvalues outside a point mass](#newtonian-tidal-eigenvalues-outside-a-point-mass)
    - [Corotating point-mass tidal field](#corotating-point-mass-tidal-field)
    - [Point-mass tidal stretching and squeezing](#point-mass-tidal-stretching-and-squeezing)
    - [Quadrupolar point-mass tidal potential](#quadrupolar-point-mass-tidal-potential)
    - [Tidal disruption](#tidal-disruption)
    - [Tidal force](#tidal-force)
      - [Corotating tidal-disruption estimate for a uniform sphere](#corotating-tidal-disruption-estimate-for-a-uniform-sphere)
      - [Tide](#tide)
        - [Bay of Fundy](#bay-of-fundy)
        - [Semidiurnal tide](#semidiurnal-tide)
        - [Spring tide](#spring-tide)
        - [Neap tide](#neap-tide)
      - [Exact tidal acceleration between separated masses](#exact-tidal-acceleration-between-separated-masses)
      - [Gravity magnitude versus tidal gradient](#gravity-magnitude-versus-tidal-gradient)
      - [Love number](#love-number)
    - [Gravity gradiometry](#gravity-gradiometry)
      - [Atom-cloud gravity-gradient measurement](#atom-cloud-gravity-gradient-measurement)
    - [Quadrupolar tidal forcing](#quadrupolar-tidal-forcing)
  - [Gravitational acceleration](#gravitational-acceleration)
    - [Newtonian central configuration](#newtonian-central-configuration)
      - [Homothetic gravitational motion](#homothetic-gravitational-motion)
  - [Gravitational constant](#gravitational-constant)
    - [Gravitational mass degeneracy](#gravitational-mass-degeneracy)
    - [Gravitational constant measurement sensitivity](#gravitational-constant-measurement-sensitivity)
    - [Cold-atom measurement of the gravitational constant](#cold-atom-measurement-of-the-gravitational-constant)
  - [Poisson equation for Newtonian gravity](#poisson-equation-for-newtonian-gravity)
    - [Dyadic spherical shells with inverse-radius density scaling](#dyadic-spherical-shells-with-inverse-radius-density-scaling)
  - [Newtonian gravitational potential](#newtonian-gravitational-potential)
    - [Gravitational potential of a sinusoidal sheet](#gravitational-potential-of-a-sinusoidal-sheet)
    - [Newtonian gravitational potential of a uniform solid sphere](#newtonian-gravitational-potential-of-a-uniform-solid-sphere)
    - [Planetary quadrupole coefficient](#planetary-quadrupole-coefficient)
      - [Oblate-quadrupole epicyclic precession](#oblate-quadrupole-epicyclic-precession)
    - [Axisymmetric logarithmic gravitational potential](#axisymmetric-logarithmic-gravitational-potential)
      - [Density positivity for an axisymmetric logarithmic potential](#density-positivity-for-an-axisymmetric-logarithmic-potential)
    - [Power-law gravitational potential](#power-law-gravitational-potential)
    - [Gravitational quadrupole potential of a point-mass binary](#gravitational-quadrupole-potential-of-a-point-mass-binary)
    - [Flattened power-law gravitational potential](#flattened-power-law-gravitational-potential)
      - [Density positivity for a flattened power-law potential](#density-positivity-for-a-flattened-power-law-potential)
    - [Newtonian potential of a point mass](#newtonian-potential-of-a-point-mass)
      - [Self-gravity in a thin spherical shell expansion](#self-gravity-in-a-thin-spherical-shell-expansion)
      - [Gravitational potential of a truncated inverse-radius sphere](#gravitational-potential-of-a-truncated-inverse-radius-sphere)
      - [Axisymmetric gravitational potential of a displaced cylindrical interface](#axisymmetric-gravitational-potential-of-a-displaced-cylindrical-interface)
    - [Spherically symmetric potential](#spherically-symmetric-potential)
  - [Newtonian gravitational potential energy](#newtonian-gravitational-potential-energy)
    - [Spherical binding-energy mass integral](#spherical-binding-energy-mass-integral)
    - [Minimum-separation binding-energy bounds](#minimum-separation-binding-energy-bounds)
      - [Negative-energy minimum-separation upper bound](#negative-energy-minimum-separation-upper-bound)
  - [Cavendish experiment](#cavendish-experiment)
    - [Cavendish torsion balance](#cavendish-torsion-balance)

## Axial and transverse gravity of a uniform rod

↑ **Parent:** [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md)

Integrate Newtonian point-force elements along a uniform thin rod of total [mass](classical-mechanics.md#mass) $M$ and half-length $a$. The first title formula applies on the axis outside the endpoint, $b>a$; the second applies on its perpendicular bisector. Both approach the point-mass result at large distance, but at equal distance their ratio is $1+3a^2/(2b^2)+O(a^4/b^4)$. A nonuniform linear [mass](classical-mechanics.md#mass) profile cannot be replaced by these formulas using only total [mass](classical-mechanics.md#mass) and [length](physics.md#length).

### Circular orbit perpendicular to a uniform rod

↑ **Parent:** [Axial and transverse gravity of a uniform rod](#axial-and-transverse-gravity-of-a-uniform-rod)

For a light test [mass](classical-mechanics.md#mass) in the rod's perpendicular-bisector plane, axial [symmetry](physics.md#symmetry-physics) makes the attraction radial. Equating $mv^2/r$ to the transverse [force](force.md) gives the title [speed](classical-mechanics.md#speed). Far outside the rod it is Keplerian, proportional to $r^{-1/2}$. Well inside the half-length but outside its physical thickness, the rod approximates an infinite line and the circular [speed](classical-mechanics.md#speed) is nearly constant, $\sqrt{GM/a}$. Extrapolation to an orbit inside the material or a zero-radius orbit is outside this thin-rod model.

## Gravitational-electrostatic balance of equal charged spheres

↑ **Parent:** [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md)

For two identical spheres sufficiently far apart, [Coulomb's law](electrostatics.md#coulomb-s-law) and [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md) both give inverse-square forces. Equal-sign charges therefore balance attraction when the displayed charge-to-mass relation holds. For uniform mass density $\rho$, substituting $M=4\pi\rho a^3/3$ fixes the radius. Changing the separation does not restore balance if the charge-to-mass ratio is wrong. Spherically symmetric charge makes the monopole result exact outside each sphere; polarization can require a far-field approximation.

## Free fall

↑ **Parent:** [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_fall)

Free fall is motion under [gravity](physics.md#gravity) alone: there is no supporting [normal force](force.md#normal-force), engine thrust or appreciable [drag force](fluid-mechanics.md#drag-physics). In the [Newtonian mechanics](newtonian-mechanics.md) model, a [test particle](classical-mechanics.md#test-particle) of [mass](classical-mechanics.md#mass) $m$ obeys $m\ddot{\mathbf r}=m\mathbf g(\mathbf r)$, hence $\ddot{\mathbf r}=\mathbf g(\mathbf r)$. The [mass](classical-mechanics.md#mass) cancels. Bodies released at the same [position](classical-mechanics.md#position) with the same [velocity](classical-mechanics.md#velocity) follow the same path in this model, even if their [gravitational weights](force.md#weight-physics) differ. [NASA Glenn: free-falling objects and the cancellation of mass](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/free-falling-objects/)

A dropped stone is one example; a coasting satellite is another. Free fall does not require motion straight down or decreasing distance to the attracting body. An ideal [circular orbit](classical-mechanics.md#circular-orbit) has constant radius while its [velocity](classical-mechanics.md#velocity) continually turns under [centripetal acceleration](classical-mechanics.md#centripetal-acceleration). The [circular orbit as continuous free fall](classical-mechanics.md#circular-orbit-as-continuous-free-fall) connects the familiar drop with orbital motion.

Near a surface, treating the [gravitational acceleration](#gravitational-acceleration) as constant gives a useful first prediction. Over larger heights, the [inverse-square law](physics.md#inverse-square-law) changes the acceleration during the fall. [Radial free fall from rest](#radial-free-fall-from-rest) uses [conservation of mechanical energy](energy.md#conservation-of-mechanical-energy) to account for that change exactly, within the specified [Newtonian gravitational field](#newtonian-gravitational-field). The contrast matters: the simplest formula is an approximation to a physical model, rather than a law with the same numerical $g$ everywhere.

History also makes the idealization tangible. Galileo's _Two New Sciences_ (1638), Third Day, Theorem II, derives distance proportional to the square of time for uniformly accelerated motion from rest; its first corollary gives successive distances in the ratios $1,3,5,7,\ldots$ over equal time intervals. This is a kinematic statement, predating the gravitational [inverse-square law](physics.md#inverse-square-law). [Galileo, Two New Sciences, Third Day, Theorem II and Corollary I; Crew and de Salvio's 1914 translation, pp. 174–176](https://galileoandeinstein.phys.virginia.edu/tns_draft/tns_160to243.html)

On Apollo 15's final lunar surface excursion, David Scott released a hammer and a feather together. The near-[vacuum](physics.md#vacuum) removed the large difference in [drag force](fluid-mechanics.md#drag-physics) familiar on Earth. NASA's report describes their arrival together within the accuracy of the release; this demonstration illustrates the [free fall](#free-fall) prediction without establishing infinite experimental precision. [NASA's original footage and Joe Allen's account in the Apollo 15 Preliminary Science Report, p. 2-11](https://science.nasa.gov/resource/the-apollo-15-hammer-feather-drop/)

<a id="video-nasa-footage-of-david-scott-s-apollo-15-hammer-and-feather-free-fall-demonstration"></a>
**[Video 1](#video-nasa-footage-of-david-scott-s-apollo-15-hammer-and-feather-free-fall-demonstration). NASA footage of David Scott's Apollo 15 hammer-and-feather free-fall demonstration.** [Source](https://www.youtube.com/watch?v=oYEgdZ3iEKA).

### Free fall in a constant gravitational field

↑ **Parent:** [Free fall](#free-fall)

Take downward [displacement](classical-mechanics.md#displacement) $s$ as positive, assume a constant [gravitational acceleration](#gravitational-acceleration) $g>0$, and release a [point mass](classical-mechanics.md#point-mass) from rest at $s=0$. Integrating $\ddot s=g$ twice gives

$$
v(t)=gt,\qquad s(t)=\frac12gt^2.
$$

For a downward distance $h>0$, the arrival time and [speed](classical-mechanics.md#speed) are

$$
t_{\mathrm{fall}}=\sqrt{\frac{2h}{g}},\qquad v_{\mathrm{arrival}}=\sqrt{2gh}.
$$

For the model values $h=20\,\mathrm m$ and $g=9.81\,\mathrm{m\,s^{-2}}$, these are approximately $2.0193\,\mathrm s$ and $19.8091\,\mathrm{m\,s^{-1}}$. Doubling the height multiplies both quantities by $\sqrt2$; it does not double them. The same [speed](classical-mechanics.md#speed) follows from the [work-energy theorem](energy.md#work-energy-theorem), $mgh=mv^2/2$.

For intervals of length $\Delta t$, the successive downward [displacements](classical-mechanics.md#displacement) are

$$
s((j+1)\Delta t)-s(j\Delta t)=\frac12g(\Delta t)^2(2j+1),\qquad j=0,1,2,\ldots.
$$

Thus equal spacing in time produces increasingly separated positions. This is the odd-number pattern in Galileo's result. It assumes constant [acceleration](classical-mechanics.md#acceleration) and release from rest; a nonzero initial [velocity](classical-mechanics.md#velocity) adds a linear term to $s(t)$.

The approximation can be estimated for a spherical source of radius $R$ and [standard gravitational parameter](#standard-gravitational-parameter) $\mu$. Writing $g_0=\mu/R^2$, the gravitational magnitude at height $h$ is

$$
\frac{g(R+h)}{g_0}=\left(1+\frac hR\right)^{-2}.
$$

For $h/R\ll1$, a [Taylor expansion](calculus.md#taylor-expansion) gives $g(R+h)/g_0=1-2h/R+O((h/R)^2)$. Small height relative to the source's radius makes nearly constant gravity plausible; negligible [drag force](fluid-mechanics.md#drag-physics) remains a separate requirement.

### Radial free fall from rest

↑ **Parent:** [Free fall](#free-fall)

Let a [test particle](classical-mechanics.md#test-particle) start at rest at radius $r_0$ outside a fixed spherically symmetric source. The [spherical shell theorem](mathematical-physics.md#spherical-shell-theorem) gives the exterior [Newtonian gravitational potential](#newtonian-gravitational-potential) $\Phi(r)=-\mu/r$, where $\mu=GM$ is the source's [standard gravitational parameter](#standard-gravitational-parameter). Zero initial transverse [velocity](classical-mechanics.md#velocity) makes the motion radial. [Conservation of mechanical energy](energy.md#conservation-of-mechanical-energy) per unit [mass](classical-mechanics.md#mass) gives

$$
\frac{\dot r^2}{2}-\frac{\mu}{r}=-\frac{\mu}{r_0},\qquad
\dot r=-\sqrt{2\mu\left(\frac1r-\frac1{r_0}\right)}.
$$

The minus sign selects inward motion; the positive square root is its [speed](classical-mechanics.md#speed). For a fall from $r_0=2R$ to the surface $r=R$, that [speed](classical-mechanics.md#speed) is $\sqrt{\mu/R}$. In the limit of release from rest infinitely far away, the familiar [free-fall speed](astrophysical-black-hole.md#free-fall-speed) is $\sqrt{2\mu/r}$, equal in magnitude to the local [escape velocity](energy.md#escape-velocity). A finite starting radius gives a smaller speed.

The arrival time follows from the same first integral. Set $r=r_0\cos^2\eta$. Then

$$
t(\eta)=\sqrt{\frac{r_0^3}{2\mu}}\left(\eta+\sin\eta\cos\eta\right),\qquad
\eta=\arccos\sqrt{\frac r{r_0}},\qquad 0\leq\eta<\frac\pi2.
$$

For arrival at $R>0$ this is finite, and the field formula is used only outside the source. For $r_0=2R$, $\eta=\pi/4$ gives

$$
t_{\mathrm{arrival}}=\left(1+\frac\pi2\right)\sqrt{\frac{R^3}{\mu}}\approx2.570796\sqrt{\frac{R^3}{\mu}}.
$$

Keeping the smaller initial gravitational magnitude $g(r_0)=\mu/(4R^2)$ constant would predict $\sqrt8\,\sqrt{R^3/\mu}$, about $10.0\%$ longer. The actual [acceleration](classical-mechanics.md#acceleration) increases during the fall.

<a id="image-radial-free-fall-height-and-arrival-time-compared-with-constant-gravity-at-the-release-point"></a>
![](radial-free-fall-gravity-variation.png)

**[Figure 1](#image-radial-free-fall-height-and-arrival-time-compared-with-constant-gravity-at-the-release-point). Radial free-fall height and arrival time compared with constant gravity at the release point**.

The curves compare a shallow fall, $h/R=0.02$, with a fall from $r_0=2R$, so $h/R=1$. Each comparison holds the release height and initial gravitational magnitude fixed. The constant-gravity model is close for the shallow fall and increasingly inaccurate for the larger one. This is also a practical use of [nondimensionalization](mathematical-physics.md#nondimensionalization): the normalized trajectories depend on $h/R$, while $\sqrt{R^3/\mu}$ supplies the dimensional time scale.

### Rotational deflection of a falling body

↑ **Parent:** [Free fall](#free-fall)

In an Earth-fixed [rotating reference frame](mathematical-physics.md#rotating-reference-frame), the horizontal displacement of a freely falling body receives contributions from [Coriolis acceleration](mathematical-physics.md#coriolis-acceleration) and [centrifugal acceleration](mathematical-physics.md#centrifugal-acceleration). A short-fall approximation substitutes the unperturbed downward [velocity](classical-mechanics.md#velocity) into the Coriolis term and the Earth's surface [position](classical-mechanics.md#position) into the centrifugal term. If [gravitational acceleration](#gravitational-acceleration) excludes centrifugal acceleration, both contributions must be included explicitly.

#### Equatorial Coriolis deflection in free fall

↑ **Parent:** [Rotational deflection of a falling body](#rotational-deflection-of-a-falling-body)

A body released from rest relative to [Earth](planetary-science.md#earth) at the equator has unperturbed downward [velocity](classical-mechanics.md#velocity) $v_U=-gt$. The [Coriolis acceleration in local Earth coordinates](mathematical-physics.md#coriolis-acceleration-in-local-earth-coordinates) gives eastward acceleration $a_E=-2\Omega_Ev_U=2\Omega_Egt$. Integration gives $x_E=\Omega_Egt^3/3$ and impact time $t_f=\sqrt{2h/g}$, proving the title formula. This is first order in [Earth's rotation](planetary-science.md#earth-s-rotation), neglecting air resistance and the height dependence of the effective local [gravitational acceleration](#gravitational-acceleration). For a short fall at latitude $\varphi$, its leading eastward term is multiplied by $\cos\varphi$.

## Newtonian gravitational field

↑ **Parent:** [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md)

The [Newtonian gravitational field](#newtonian-gravitational-field) is the gravitational [force](force.md) per unit [mass](classical-mechanics.md#mass) of a [test particle](classical-mechanics.md#test-particle). For a [point mass](classical-mechanics.md#point-mass) $M$ at the origin,

$$
\mathbf g(\mathbf r)=\frac{\mathbf F}{m}=-\frac{GM}{r^3}\mathbf r,\qquad g(r)=|\mathbf g|=\frac{GM}{r^2}.
$$

The [test particle](classical-mechanics.md#test-particle)'s [mass](classical-mechanics.md#mass) cancels: different small [masses](classical-mechanics.md#mass) have the same [gravitational acceleration](#gravitational-acceleration) at the same [position](classical-mechanics.md#position). In [SI](physics.md#international-system-of-units), the [Newtonian gravitational field](#newtonian-gravitational-field) has units $\mathrm{N\,kg^{-1}}=\mathrm{m\,s^{-2}}$. The same exterior expression holds for a spherically symmetric source, by the [spherical shell theorem](mathematical-physics.md#spherical-shell-theorem).

Choose a reference radius $r_0>0$, set $g_0=GM/r_0^2$, and use [nondimensionalization](mathematical-physics.md#nondimensionalization) with $z=r/r_0$. Then $g/g_0=z^{-2}$: at $z=1,2,4$, the magnitudes are $1,1/4,1/16$. This makes the spatial variation visible without specifying a planet. [OpenStax: inverse-square attraction and spherical sources](https://openstax.org/books/university-physics-volume-1/pages/13-1-newtons-law-of-universal-gravitation)

<a id="image-normalized-newtonian-gravitational-field-and-point-mass-potential"></a>
![](gravity-force-and-potential.png)

**[Figure 2](#image-normalized-newtonian-gravitational-field-and-point-mass-potential). Normalized Newtonian gravitational field and point-mass potential**. Doubling the radius quarters the magnitude of the [Newtonian gravitational field](#newtonian-gravitational-field), but halves the magnitude of the negative [Newtonian gravitational potential](#newtonian-gravitational-potential). Both curves approach zero as radius increases; the inward [gravitational acceleration](#gravitational-acceleration) is minus the [gradient](multivariable-calculus.md#gradient) of the [Newtonian gravitational potential](#newtonian-gravitational-potential).

### Gravitational field of an infinite plane sheet

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

An infinite plane sheet of surface [mass density](fluid-mechanics.md#density) $\Sigma$ has constant gravitational-field magnitude $2\pi G\Sigma$ on either side, directed toward the sheet. A Gaussian pillbox has equal inward [flux](mathematical-physics.md#flux) on its two caps and enclosed [mass](classical-mechanics.md#mass) $\Sigma A$, so $-2gA=-4\pi G\Sigma A$. A uniform infinite slab has the same exterior formula with $\Sigma=\rho h$. Translating an infinite sheet does not change its exterior field, whereas adding a slab changes its surface [mass density](fluid-mechanics.md#density).

#### Tidal water loading of a spring balance

↑ **Parent:** [Gravitational field of an infinite plane sheet](#gravitational-field-of-an-infinite-plane-sheet)

A [mass](classical-mechanics.md#mass) above a sufficiently wide estuary experiences additional downward [gravity](physics.md#gravity) when extra water is present. Approximating the tide as a plane slab of [density](fluid-mechanics.md#density) $\rho$ and added thickness $h$ gives $\Delta g=2\pi G\rho h$. A linear [spring](elasticity-physics.md#spring) with initial extension $x_0=mg/k$ changes by $\Delta x=(m/k)\Delta g=x_0\Delta g/g$. This isolates direct water attraction; it omits finite shoreline geometry, buoyancy, structural motion and terrestrial tides.

### Axial gravitational field of a uniform ring

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

A uniform thin ring of radius $a$ and [mass](classical-mechanics.md#mass) $M$ has axial [gravitational field](physics.md#gravitational-field) $g_z=-GMz/(a^2+z^2)^{3/2}$. Every ring element is the same distance from the axial point; transverse contributions cancel and axial projection supplies the factor $z/\sqrt{a^2+z^2}$. This also follows by differentiating the axial potential $\Phi=-GM/\sqrt{a^2+z^2}$. Near the centre $g_z\simeq-GMz/a^3$, whereas far away it approaches the point-mass field.

### Gravitational field of a finite uniform line segment

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

Spread [mass](classical-mechanics.md#mass) $M$ uniformly along $-a<z<a$ on an axis, with [linear mass density](fluid-mechanics.md#linear-mass-density) $\lambda=M/(2a)$. In its perpendicular bisector plane, axial field components cancel, and the radial component is

$$
g_r=-G\lambda r\int_{-a}^a\frac{dz}{(r^2+z^2)^{3/2}}=-\frac{GM}{r\sqrt{r^2+a^2}}.
$$

This is an exact [line mass](astrophysical-fluid-dynamics.md#line-mass) model and a thin-rod approximation for a physical cylinder. A centred [circular orbit](classical-mechanics.md#circular-orbit) in this symmetry plane has $v^2=GM/\sqrt{R^2+a^2}$. Thus $v\to\sqrt{GM/a}=\sqrt{2G\lambda}$ for $R/a\to0$, and $v\sim\sqrt{GM/R}$ for $R/a\to\infty$. For a finite-width rod, the first limit is useful only while its transverse size remains much smaller than $R$.

### Gravitational field of an infinite uniform cylinder

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

A circular infinite cylinder of radius $b$ and uniform [mass density](fluid-mechanics.md#density) $\rho$ has [linear mass density](fluid-mechanics.md#linear-mass-density) $\lambda=\pi b^2\rho$. A coaxial [Gaussian surface](maxwell-equations.md#gaussian-surface) of length $L$ has inward radial [gravitational field](physics.md#gravitational-field) and no end-cap [flux](mathematical-physics.md#flux). [Gauss's law for gravity](#gauss-s-law-for-gravity) gives $2\pi rL g_r=-4\pi G\lambda L$ outside, hence the displayed result. Inside, enclosed [linear mass density](fluid-mechanics.md#linear-mass-density) is $\pi r^2\rho$, so $g_r=-2\pi G\rho r$. An exterior [circular orbit](classical-mechanics.md#circular-orbit) has [speed](classical-mechanics.md#speed) $\sqrt{2G\lambda}$ independent of radius. The exterior formula presupposes circular axial symmetry; area alone would not specify the near field of a noncircular rod.

#### Plumb-line deflection from cylindrical gravity

↑ **Parent:** [Gravitational field of an infinite uniform cylinder](#gravitational-field-of-an-infinite-uniform-cylinder)

A pendulum of length $L$ in vertical [gravity](physics.md#gravity) $g$ is weakly attracted horizontally by an added long circular cylinder of line [density](fluid-mechanics.md#density) $\lambda$. Outside it, $g_h=2G\lambda/r$ at axis distance $r$. Small-angle equilibrium gives horizontal deflection $d\simeq Lg_h/g=2GL\lambda/(rg)$. Removing the cylinder's [mass](classical-mechanics.md#mass) reverses the change. It is a before/after differential estimate; finite length, a nonhorizontal radial direction and mechanical motion require corrections.

#### Diameter-rod oscillation in cylindrical gravity

↑ **Parent:** [Gravitational field of an infinite uniform cylinder](#gravitational-field-of-an-infinite-uniform-cylinder)

A thin rod of length $2R$ and [linear mass density](fluid-mechanics.md#linear-mass-density) $\lambda$ slides along a diameter of an infinite uniform source cylinder of radius $R$. Neglect the narrow hole's perturbation of the source field. If the rod centre is displaced by $x$, $F(x)=\lambda\int_{x-R}^{x+R}g_y(y)\,dy$. The endpoint derivative gives $F'(0)=\lambda[g_y(R)-g_y(-R)]=-4\pi G\rho\lambda R$. Dividing the restoring coefficient by rod [mass](classical-mechanics.md#mass) $2R\lambda$ gives the displayed small-oscillation [frequency](wave.md#frequency).

<h3 id="gauss-s-law-for-gravity">Gauss's law for gravity</h3>

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

The outward [flux](mathematical-physics.md#flux) of the [Newtonian gravitational field](#newtonian-gravitational-field) through a closed surface is $-4\pi G$ times the enclosed [mass](classical-mechanics.md#mass). A sphere around a [point mass](classical-mechanics.md#point-mass) establishes the coefficient; [superposition](vector-space.md#superposition-principle) extends the integral law to general [mass distributions](classical-mechanics.md#mass-distribution). The minus sign expresses attractive gravity. A symmetric [Gaussian surface](maxwell-equations.md#gaussian-surface) can turn the flux relation into a local field calculation, but the integral law alone does not imply that the field is uniform on an arbitrary surface.

### Uniform gravitational field in an off-center spherical cavity

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

Remove a spherical void centered at $c$ from a uniform sphere centered at the origin. At points inside the void, [superposition](vector-space.md#superposition-principle) combines the sphere's interior field $-4\pi G\rho x/3$ with the removed sphere's field $+4\pi G\rho(x-c)/3$. Their sum is the displayed constant [Newtonian gravitational field](#newtonian-gravitational-field). A second removed mass outside this void adds a nonuniform contribution.

#### Cavity equilibrium destabilized by a second void

↑ **Parent:** [Uniform gravitational field in an off-center spherical cavity](#uniform-gravitational-field-in-an-off-center-spherical-cavity)

A uniform [Newtonian gravitational field](#newtonian-gravitational-field) inside one spherical void can be cancelled at a point by the repulsive field representing another removed sphere. The latter field has a [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) proportional to $I-3\hat r\hat r^T$: its axial eigenvalue is negative and both transverse eigenvalues positive. The equilibrium is restoring along the axis but unstable transversely. A zero force is thus not enough for stable rest.

### Newtonian gravitational stress tensor

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

For a [Newtonian gravitational potential](#newtonian-gravitational-potential) obeying the [Poisson equation for Newtonian gravity](#poisson-equation-for-newtonian-gravity), define $T_{ij}=[\partial_i\Phi\partial_j\Phi-\delta_{ij}|\nabla\Phi|^2/2]/(4\pi G)$. Commutation of mixed [partial derivatives](multivariable-calculus.md#partial-derivative) gives $\partial_jT_{ij}=\rho\partial_i\Phi$. Thus the gravitational force density can be put in conservative form as $-\partial_jT_{ij}$. The sign is chosen so that $T_{ij}$ is added to the momentum flux; reversing the stress convention reverses the divergence sign.

#### Gravitational stress contribution to angular-momentum transport

↑ **Parent:** [Newtonian gravitational stress tensor](#newtonian-gravitational-stress-tensor)

In cylindrical coordinates, the [Newtonian gravitational stress tensor](#newtonian-gravitational-stress-tensor) gives radial [angular-momentum flux](momentum.md#angular-momentum-flux) $rT_{r\phi}=r(\partial_r\Phi)(r^{-1}\partial_\phi\Phi)/(4\pi G)$. Nonaxisymmetric structure can correlate the field components and transport [angular momentum](momentum.md#angular-momentum). The isotropic negative-pressure part has zero off-diagonal component, so it gives no direct radial transport. This separates a shear flux from a contribution to normal force balance.

### Self-gravity

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

Self-gravity is the [gravitational acceleration](#gravitational-acceleration) produced by a system's own [mass density](fluid-mechanics.md#density). It is obtained by solving the [Poisson equation for Newtonian gravity](#poisson-equation-for-newtonian-gravity) for that density, rather than treating the [Newtonian gravitational potential](#newtonian-gravitational-potential) as an externally fixed field. It competes with [pressure](pressure.md) and rotational support in [gravitational instability of an astrophysical disk](gravitational-instability-of-an-astrophysical-disk.md).

### Standard gravitational parameter

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Standard_gravitational_parameter)

The product $\mu=GM$ of the [gravitational constant](#gravitational-constant) and a central [mass](classical-mechanics.md#mass) sets the strength of the exterior [Newtonian gravitational field](#newtonian-gravitational-field). Its dimensions are length cubed divided by time squared. In the exact relative [two-body problem](celestial-mechanics.md#two-body-problem), the parameter is $G(M_1+M_2)$; using $GM$ for one source assumes the [test particle](classical-mechanics.md#test-particle) approximation.

The combination is useful because orbital and falling-body observations constrain $\mu$ directly. A gravitational [circular orbit](classical-mechanics.md#circular-orbit) of radius $a$ has [oscillation period](classical-mechanics.md#period-of-an-oscillation) $T=2\pi\sqrt{a^3/\mu}$, so measuring $a$ and $T$ gives $\mu=4\pi^2a^3/T^2$. That measurement alone does not separately determine $G$ and $M$. Similarly, [radial free fall from rest](#radial-free-fall-from-rest) has a natural time scale $\sqrt{r_0^3/\mu}$.

Other interactions require a different model. Inverse-square [radiation pressure](pressure.md#radiation-pressure) can reduce the effective attraction for a dust [Kepler orbit](celestial-mechanics.md#kepler-orbit); calling that effective coefficient a gravitational parameter must not hide the added [force](force.md).

### Tidal tensor

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

The acceleration tidal tensor is $T_{jk}=\partial_k g_j=-\partial_j\partial_k\Phi$ for [gravitational acceleration](#gravitational-acceleration) $\mathbf g=-\nabla\Phi$. It describes differential acceleration $\Delta\mathbf g\simeq T\Delta\mathbf r$. Some authors instead call the positive [Hessian matrix](multivariable-calculus.md#hessian-matrix) $\partial_j\partial_k\Phi$ the tidal tensor, reversing this sign convention. For a point mass and the positive potential convention $\mathbf g=\nabla\psi$, the tensor is $Gm(3\mathbf R\mathbf R^{\mathsf T}/R^5-\mathbf1/R^3)$.

The [tidal tensor](#tidal-tensor) is the [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) of the [Newtonian gravitational field](#newtonian-gravitational-field), rather than the [gravitational acceleration](#gravitational-acceleration) itself. Its entries have units $\mathrm{s^{-2}}$: multiplying by a [displacement](classical-mechanics.md#displacement) produces an [acceleration](classical-mechanics.md#acceleration). For a smooth [Newtonian gravitational potential](#newtonian-gravitational-potential), the [tidal tensor](#tidal-tensor) is a [symmetric matrix](linear-algebra.md#symmetric-matrix), since mixed [partial derivatives](multivariable-calculus.md#partial-derivative) commute. A spatially uniform [gravitational acceleration](#gravitational-acceleration) has zero [tidal tensor](#tidal-tensor), however large that [acceleration](classical-mechanics.md#acceleration) is.

#### Newtonian tidal eigenvalues outside a point mass

↑ **Parent:** [Tidal tensor](#tidal-tensor)

For $\Phi=-GM/r$, the acceleration [tidal tensor](#tidal-tensor) is

$$
T_{ij}=-\partial_i\partial_j\Phi=
\frac{GM}{r^3}(3n_i n_j-\delta_{ij}).
$$

Its radial eigenvalue is $2GM/r^3$ and its two transverse eigenvalues are $-GM/r^3$. This stretches a small freely falling cloud radially and compresses it transversely. The zero trace expresses the vacuum [Poisson equation](partial-differential-equation.md#poisson-s-equation) outside the source; within matter the trace is $-4\pi G\rho$.

#### Corotating point-mass tidal field

↑ **Parent:** [Tidal tensor](#tidal-tensor)

Use local axes radial, tangential in the orbital plane, and perpendicular to that plane around a [circular Kepler orbit](celestial-mechanics.md#circular-kepler-orbit) with $\Omega^2=GM/R^3$. The gravitational [tidal tensor](#tidal-tensor) is $\Omega^2\operatorname{diag}(2,-1,-1)$. A uniformly corotating frame adds the gradient of [centrifugal acceleration](mathematical-physics.md#centrifugal-acceleration), $\Omega^2\operatorname{diag}(1,1,0)$, giving the displayed effective tensor for stationary offsets. Thus the radial differential acceleration is $3GMa/R^3$. These are accelerations, or forces per unit test mass; an actual differential force includes that mass. Moving offsets also experience [Coriolis acceleration](mathematical-physics.md#coriolis-acceleration).

#### Point-mass tidal stretching and squeezing

↑ **Parent:** [Tidal tensor](#tidal-tensor)

For a source [point mass](classical-mechanics.md#point-mass) $M$ at the origin, let $\mathbf R=R\mathbf n$, where $\mathbf n$ is an outward [unit vector](vector-space.md#unit-vector), and let $\mu=GM$ be the source's [standard gravitational parameter](#standard-gravitational-parameter). Differentiating $g_i=-\mu R_i/R^3$ gives the [tidal tensor](#tidal-tensor)

$$
T_{ij}=\frac{\mu}{R^3}(3n_i n_j-\delta_{ij}),\qquad T=\frac{\mu}{R^3}(3\mathbf n\mathbf n^{\mathsf T}-I),
$$

where $\delta_{ij}$ is the [Kronecker delta](multilinear-algebra.md#kronecker-delta) and $I$ is the [identity matrix](vector-space.md#identity-matrix). In an [orthonormal basis](inner-product.md#orthonormal-basis) with first axis radial, the [tidal tensor](#tidal-tensor) is

$$
T=\frac{\mu}{R^3}\begin{pmatrix}2&0&0\\0&-1&0\\0&0&-1\end{pmatrix}.
$$

The radial [eigenvalue](linear-operator-theory.md#eigenvalue) $2\mu/R^3$ separates nearby freely falling [test particles](classical-mechanics.md#test-particle); the two transverse [eigenvalues](linear-operator-theory.md#eigenvalue) $-\mu/R^3$ bring them together. The farther radial [test particle](classical-mechanics.md#test-particle) falls inward less rapidly, so its [acceleration](classical-mechanics.md#acceleration) relative to the nearer one points outward. Transverse [gravitational accelerations](#gravitational-acceleration) converge toward the source. Thus an initially resting small cloud stretches radially and squeezes in both transverse directions. These are instantaneous relative [accelerations](classical-mechanics.md#acceleration); the subsequent shape also depends on initial [velocities](classical-mechanics.md#velocity) and the changing [tidal tensor](#tidal-tensor) along the cloud's [free fall](#free-fall).

Outside the source, the [matrix trace](linear-algebra.md#matrix-trace) is $2\mu/R^3-\mu/R^3-\mu/R^3=0$. This matches $\operatorname{tr}T=-\nabla^2\Phi=0$ in a region with zero [mass density](fluid-mechanics.md#density), by the [Poisson equation for Newtonian gravity](#poisson-equation-for-newtonian-gravity). Zero [matrix trace](linear-algebra.md#matrix-trace) means no leading change of a small initially resting cloud's [volume](geometry-and-topology.md#volume) at order $t^2$, not that each separation stays fixed. Inside matter, the same sign convention gives $\operatorname{tr}T=-4\pi G\rho$ instead.

#### Quadrupolar point-mass tidal potential

↑ **Parent:** [Tidal tensor](#tidal-tensor)

Subtracting the constant and uniform-acceleration terms from the point-mass [relative potential](galaxy.md#relative-potential) gives $\psi_{\mathrm{tid}}=Gm_p[3(\mathbf r\cdot\widehat{\mathbf r}_p)^2-r^2]/(2r_p^3)$, with force convention $\nabla\psi$. Its [tidal tensor](#tidal-tensor) is $Gm_p(3\widehat{\mathbf r}_p\widehat{\mathbf r}_p^T-I)/r_p^3$. This is the leading term for target size small compared with separation.

#### Tidal disruption

↑ **Parent:** [Tidal tensor](#tidal-tensor)

Disruption of a self-gravitating body when differential gravitational [acceleration](classical-mechanics.md#acceleration) across it exceeds its binding [acceleration](classical-mechanics.md#acceleration). For a body of radius $R$, [mass](classical-mechanics.md#mass) $m$ at distance $r$ from a much more massive body $M$, the competing scales are $GMR/r^3$ and $Gm/R^2$; their equality gives $r\sim R(M/m)^{1/3}$, up to geometry and internal-structure factors. The [tidal tensor](#tidal-tensor) gives the directional differential [acceleration](classical-mechanics.md#acceleration). A [tidal disruption event](astrophysical-black-hole.md#tidal-disruption-event) near a black hole is a specific astronomical application.

#### Tidal force

↑ **Parent:** [Tidal tensor](#tidal-tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tidal_force)

Differential gravitational [acceleration](classical-mechanics.md#acceleration), multiplied by the affected [mass](classical-mechanics.md#mass), across a spatially extended body. In the linear approximation the [acceleration](classical-mechanics.md#acceleration) difference is $T\Delta\boldsymbol r$, where $T$ is the [tidal tensor](#tidal-tensor). Stellar [tidal forces](#tidal-force) limit the domain of a [circumplanetary orbit](celestial-mechanics.md#circumplanetary-orbit); sufficiently strong ones can produce [tidal disruption](#tidal-disruption).

To isolate a [tidal force](#tidal-force), subtract the [gravitational acceleration](#gravitational-acceleration) shared by the body as a whole. Let a reference [test particle](classical-mechanics.md#test-particle) follow $\ddot{\mathbf R}=\mathbf g(\mathbf R)$, and let another have [position](classical-mechanics.md#position) $\mathbf R+\mathbf x$. In a [translating accelerated reference frame](mathematical-physics.md#translating-accelerated-reference-frame) with parallel, nonrotating axes,

$$
\ddot{\mathbf x}=\mathbf g(\mathbf R+\mathbf x)-\mathbf g(\mathbf R)=T(\mathbf R)\mathbf x+O\!\left(\frac{\mu|\mathbf x|^2}{R^4}\right)
$$

for a source [point mass](classical-mechanics.md#point-mass), when $|\mathbf x|/R\ll1$. Here $\mu=GM$ is its [standard gravitational parameter](#standard-gravitational-parameter) and the last term uses [Big O notation](real-analysis.md#big-o-notation). This [Taylor expansion](calculus.md#taylor-expansion) removes the common inward pull and keeps the spatial variation. The near side has an excess pull toward the source; the far side has a deficit of inward pull, which is an outward relative [acceleration](classical-mechanics.md#acceleration). Both sides can stretch apart while both still accelerate toward the source.[§7–4, discussion of stronger near-side and weaker far-side attraction](physics-bibliography.md#the-feynman-lectures-on-physics-volume-i-by-richard-feynman-and-others/chapter-7-the-theory-of-gravitation)

<a id="image-subtracting-common-gravitational-acceleration-reveals-radial-stretching-and-transverse-squeezing"></a>
![](tidal-field-difference-and-stretching.png)

**[Figure 3](#image-subtracting-common-gravitational-acceleration-reveals-radial-stretching-and-transverse-squeezing). Subtracting common gravitational acceleration reveals radial stretching and transverse squeezing**. Blue arrows show the exact [Newtonian gravitational field](#newtonian-gravitational-field) at several [positions](classical-mechanics.md#position) near a reference point. Orange arrows show its linear residual, calculated with the [tidal tensor](#tidal-tensor). Arrow lengths use separate scales in the two panels; this is a comparison of direction and spatial variation, not two equal-magnitude fields.

For a material element of [mass](classical-mechanics.md#mass) $m$, the residual external [force](force.md) in this [translating accelerated reference frame](mathematical-physics.md#translating-accelerated-reference-frame) is $m[\mathbf g(\mathbf R+\mathbf x)-\mathbf g(\mathbf R)]$. Actual deformation also depends on [elasticity](elasticity-physics.md), [pressure](pressure.md) and [self-gravity](#self-gravity). A [rigid body](rigid-body-dynamics.md) approximation suppresses deformation but can still have internal [forces](force.md) that resist the [tidal force](#tidal-force). The [point-mass tidal stretching and squeezing](#point-mass-tidal-stretching-and-squeezing) pattern describes freely falling, noninteracting [test particles](classical-mechanics.md#test-particle), rather than promising the same shape for every solid, star or ocean. A [rotating reference frame](mathematical-physics.md#rotating-reference-frame) introduces [centrifugal acceleration](mathematical-physics.md#centrifugal-acceleration) and [Coriolis acceleration](mathematical-physics.md#coriolis-acceleration), which must be included separately.

##### Corotating tidal-disruption estimate for a uniform sphere

↑ **Parent:** [Tidal force](#tidal-force)

A small cohesionless spherical body of radius $s$ and density $\rho$ has surface self-gravitational acceleration $4\pi G\rho s/3$. The radial stretching of the [corotating point-mass tidal field](#corotating-point-mass-tidal-field) is $3GMs/R^3$. Equating them gives the displayed survival-distance estimate. The size $s$ cancels because both accelerations are linear in $s$ at fixed density. This is a local spherical force-balance estimate, not the exact fluid Roche figure: shape deformation, material strength and nonsynchronous spin can change its numerical coefficient.

##### Tide

↑ **Parent:** [Tidal force](#tidal-force)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tide)

A [tide](#tide) is a periodic change in ocean level driven mainly by the differential gravitational [forces](force.md) of the [Moon](planetary-science.md#moon) and [Sun](stellar-astrophysics.md#sun), together with the [Earth](planetary-science.md#earth)'s rotation. Their [tidal forces](#tidal-force) act across the extended planet; a uniform acceleration shared by the whole Earth does not by itself generate a tide. Ocean-basin [resonance](dynamical-systems.md#resonance) and coastal geometry modify the local response.

###### Bay of Fundy

↑ **Parent:** [Tide](#tide)

###### Semidiurnal tide

↑ **Parent:** [Tide](#tide)

A [semidiurnal tide](#semidiurnal-tide) has two principal oscillations per day. The dominant lunar constituent has a period of approximately 12 hours 25 minutes; the solar semidiurnal constituent has a period of 12 hours.[Examples M2 and S2](physics-bibliography.md#about-harmonic-constituents-by-national-oceanic-and-atmospheric-administration)

###### Spring tide

↑ **Parent:** [Tide](#tide)

A [spring tide](#spring-tide) has an enhanced high-to-low tidal range because the [Moon](planetary-science.md#moon) and [Sun](stellar-astrophysics.md#sun) are approximately aligned as seen from the [Earth](planetary-science.md#earth), so their principal tidal contributions reinforce. Such alignments occur twice in a lunar phase cycle.

###### Neap tide

↑ **Parent:** [Tide](#tide)

A [neap tide](#neap-tide) has a reduced high-to-low tidal range when the directions to the [Moon](planetary-science.md#moon) and [Sun](stellar-astrophysics.md#sun) make approximately a right [angle](geometry-and-topology.md#angle) at the [Earth](planetary-science.md#earth). Their principal tidal contributions then partly oppose one another. The solar and lunar contributions are not equal, so this does not mean that tides disappear.

##### Exact tidal acceleration between separated masses

↑ **Parent:** [Tidal force](#tidal-force)

Stipulate a fixed source [point mass](classical-mechanics.md#point-mass) $M=10^{12}\,\mathrm{kg}$, two equal [test particles](classical-mechanics.md#test-particle) of [mass](classical-mechanics.md#mass) $m=1\,\mathrm{kg}$, and $G=6.67430\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$. This is a chosen model, not a measurement of a particular object. Place the [test particles](classical-mechanics.md#test-particle) on the outward radial axis at $R-L/2$ and $R+L/2$, with midpoint distance $R=100\,\mathrm m$ and separation $L=2\,\mathrm m$. Neglect their mutual attraction, other sources and all supporting [forces](force.md).

Each signed radial [gravitational acceleration](#gravitational-acceleration) is inward:

$$
a_-=-\frac{\mu}{(R-L/2)^2}\approx-0.0068098153\,\mathrm{m\,s^{-2}},\qquad a_+=-\frac{\mu}{(R+L/2)^2}\approx-0.0065427899\,\mathrm{m\,s^{-2}}.
$$

Their separation has outward relative [acceleration](classical-mechanics.md#acceleration)

$$
\ddot L=a_+-a_-=\mu\left[\frac{1}{(R-L/2)^2}-\frac{1}{(R+L/2)^2}\right]=\frac{2\mu L}{R^3}\left(1-\frac{L^2}{4R^2}\right)^{-2}.
$$

The exact value is $2.6702540\times10^{-4}\,\mathrm{m\,s^{-2}}$. The midpoint [tidal tensor](#tidal-tensor) predicts $2\mu L/R^3=2.6697200\times10^{-4}\,\mathrm{m\,s^{-2}}$, an underestimate of $0.019999\%$ relative to the exact value. For these equal $1\,\mathrm{kg}$ [masses](classical-mechanics.md#mass), the difference of external [forces](force.md) has the same numerical value in the [SI](physics.md#international-system-of-units) unit of [force](force.md), the [newton](physics.md#newton-unit). It is not an additional mutual [force](force.md) between the [test particles](classical-mechanics.md#test-particle).

The exact formula requires $L<2R$ and describes the instantaneous relative [acceleration](classical-mechanics.md#acceleration). Because the two sample [positions](classical-mechanics.md#position) are symmetric about the midpoint, the [Taylor expansion](calculus.md#taylor-expansion) error relative to the linear result starts at order $(L/R)^2$; a one-sided comparison with a reference point generally has relative error of order $L/R$. If either [test particle](classical-mechanics.md#test-particle) enters an extended source, use that source's interior [Newtonian gravitational field](#newtonian-gravitational-field) instead of extrapolating the singular [point mass](classical-mechanics.md#point-mass) model.

##### Gravity magnitude versus tidal gradient

↑ **Parent:** [Tidal force](#tidal-force)

For a fixed source [point mass](classical-mechanics.md#point-mass), the magnitude $g=\mu/R^2$ of the [gravitational acceleration](#gravitational-acceleration) measures the local pull; the radial [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda_r=2\mu/R^3$ of the [tidal tensor](#tidal-tensor) measures how that pull changes across space. Doubling $R$ divides $g$ by four but $\lambda_r$ by eight. For a fixed small radial separation $L$, the linear relative [acceleration](classical-mechanics.md#acceleration) is $\Delta a\simeq\lambda_r L$, so

$$
\frac{\Delta a}{g}\simeq\frac{2L}{R}.
$$

A small body can therefore experience strong common [gravitational acceleration](#gravitational-acceleration) with a comparatively small [tidal force](#tidal-force). A measurement of $g$ alone does not determine the [tidal tensor](#tidal-tensor): sources at different distances can have the same $g$ but different spatial variation.

<a id="image-gravity-falls-as-inverse-distance-squared-while-point-mass-tidal-stretching-falls-as-inverse-distance-cubed"></a>
![](tidal-gravity-distance-scaling.png)

**[Figure 4](#image-gravity-falls-as-inverse-distance-squared-while-point-mass-tidal-stretching-falls-as-inverse-distance-cubed). Gravity falls as inverse distance squared, while point-mass tidal stretching falls as inverse distance cubed**. The left panel compares independently normalized [gravitational acceleration](#gravitational-acceleration) and radial [tidal tensor](#tidal-tensor) [eigenvalue](linear-operator-theory.md#eigenvalue) for a fixed source. The right panel compares exact and linear relative [accelerations](classical-mechanics.md#acceleration) for two radially separated [test particles](classical-mechanics.md#test-particle) at a fixed midpoint, showing the finite-separation correction as their separation grows.

The local stretching time scale is $\lambda_r^{-1/2}=\sqrt{R^3/(2\mu)}$: it marks when an initially resting separation could change by order itself if the [tidal tensor](#tidal-tensor) stayed fixed. During [free fall](#free-fall), $R$ changes, so this scale is not a complete trajectory or a universal disruption time. [Tidal disruption](#tidal-disruption) additionally compares the [tidal force](#tidal-force) with binding by [self-gravity](#self-gravity) and material [forces](force.md); $g$ by itself supplies no such comparison.

##### Love number

↑ **Parent:** [Tidal force](#tidal-force)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Love_number)

A Love number measures a body's tidal response to an applied potential. The degree-two potential response $k_2$ is sensitive to radial density structure and central concentration, and can complement mass and radius constraints on an [exoplanet interior](exoplanet.md#exoplanet-interior). Inferring it from orbital precession requires separating other contributions and assumptions about rotation and the tidal response.

#### Gravity gradiometry

↑ **Parent:** [Tidal tensor](#tidal-tensor)

[Gravity gradiometry](#gravity-gradiometry) measures spatial differences of [gravitational acceleration](#gravitational-acceleration). Two simultaneous measurements along a [unit vector](vector-space.md#unit-vector) $\mathbf e$, separated by $L\mathbf e$, give

$$
\frac{\mathbf e\cdot[\mathbf g(\mathbf R+L\mathbf e)-\mathbf g(\mathbf R)]}{L}\simeq\mathbf e^{\mathsf T}T\mathbf e.
$$

This measures one directional component of the [tidal tensor](#tidal-tensor), not its whole [matrix](vector-space.md#matrix). Any identical platform [acceleration](classical-mechanics.md#acceleration) cancels in the difference. Unequal instrument responses, changing geometry and [rotating reference frames](mathematical-physics.md#rotating-reference-frame) can spoil that cancellation. For a large baseline, the quotient is an average of the directional [tidal tensor](#tidal-tensor) along the baseline, rather than its exact value at one point.

##### Atom-cloud gravity-gradient measurement

↑ **Parent:** [Gravity gradiometry](#gravity-gradiometry)

A laboratory [gravity gradiometry](#gravity-gradiometry) experiment used two vertically separated clouds of [chemical atoms](physics.md#atom-physics) in [vacuum](physics.md#vacuum), launched into [free fall](#free-fall). Shared [laser](laser.md) beams applied three pulses ($\pi/2,\pi,\pi/2$), splitting and recombining [matter waves](wave-function.md#matter-wave). Balanced [photodiodes](optical-instrument.md#photodiode) measured probe-light absorption to infer internal-state populations; scanning the last pulse's [wave phase](wave.md#phase-waves) produced an [interference](physical-optics.md#interference-wave-propagation) fringe.[§I, pp. 033608-1–2; §II E 1, p. 033608-6; §II F 1, p. 033608-7](physics-bibliography.md#sensitive-absolute-gravity-gradiometry-using-atom-interferometry-by-j-m-mcguirk-and-others)

The difference of fringe [wave phases](wave.md#phase-waves) obeys $\delta\phi=\mathbf k_{\mathrm{eff}}\cdot\Delta\mathbf g\,\tau^2$, with effective [wave vector](elasticity-physics.md#wavevector) $\mathbf k_{\mathrm{eff}}$ and pulse spacing $\tau$: shared reference motion cancels, leaving differential [gravitational acceleration](#gravitational-acceleration). Eight lead bricks, each approximately $12.5\,\mathrm{kg}$, were placed symmetrically around the lower chamber, about $0.2\,\mathrm m$ from the fountain apex. The measured signal was $(8.1\pm2.1)\times10^{-9}g$, versus a calculated $8.2\times10^{-9}g$, where $g$ denotes terrestrial [gravitational acceleration](#gravitational-acceleration).[§I, p. 033608-2; §III A 2, p. 033608-10, mass detection](physics-bibliography.md#sensitive-absolute-gravity-gradiometry-using-atom-interferometry-by-j-m-mcguirk-and-others)

Controls deliberately shook the shared reference reflector and compared actively isolated and unisolated operation. Tilting tests exposed sensitivity to [Coriolis acceleration](mathematical-physics.md#coriolis-acceleration) and [centrifugal acceleration](mathematical-physics.md#centrifugal-acceleration). Thus shared translation is rejectable, while rotation and finite measurement uncertainty remain limitations. The brick signal detects spatially varying [gravity](physics.md#gravity); it does not establish a precision value of the [gravitational constant](#gravitational-constant).[§III A, p. 033608-9; §III B, pp. 033608-10–11](physics-bibliography.md#sensitive-absolute-gravity-gradiometry-using-atom-interferometry-by-j-m-mcguirk-and-others)

#### Quadrupolar tidal forcing

↑ **Parent:** [Tidal tensor](#tidal-tensor)

For a point-mass companion at separation $a$, subtract the constant and linear terms of its [Newtonian gravitational potential](#newtonian-gravitational-potential) in a frame accelerating with the target's center. The leading residual is

$$
\Phi_{\mathrm{tide}}=-\frac{GM_2}{2a^3}\left[3(\mathbf n\cdot\mathbf r)^2-r^2\right].
$$

It is degree two in [spherical harmonics](analysis.md#spherical-harmonic). In a circular orbit with angular frequency $\omega_o$, its time-dependent $m=\pm2$ components force at $2\omega_o$ in a frame with no spin; there is also a static $m=0$ component. This is the leading approximation in $r/a$, and the tidal amplitude may be absorbed into a harmonic-dependent constant.

### Gravitational acceleration

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gravitational_acceleration)

Gravitational acceleration is the [acceleration](classical-mechanics.md#acceleration) of a [test particle](classical-mechanics.md#test-particle) in [free fall](#free-fall) in a [Newtonian gravitational field](#newtonian-gravitational-field). It is a vector pointing along that field; $g$ commonly denotes its positive magnitude. Near Earth's surface, the magnitude is approximately constant over shallow vertical scales. For a fixed spherical source it instead varies as $g(r)=\mu/r^2$, where $\mu$ is the [standard gravitational parameter](#standard-gravitational-parameter).

This is distinct from [gravitational weight](force.md#weight-physics), the [force](force.md) $m\mathbf g$, and from [apparent weight](force.md#apparent-weight), the support force a scale measures. An orbiting body can have substantial [gravitational acceleration](#gravitational-acceleration) while its [apparent weight](force.md#apparent-weight) is zero.

#### Newtonian central configuration

↑ **Parent:** [Gravitational acceleration](#gravitational-acceleration)

A collision-free positive-mass configuration satisfies the displayed equation when every gravitational acceleration points proportionally toward a common centre. With $W=-\sum_{i<j}Gm_im_j/|\mathbf a_i-\mathbf a_j|$, homogeneity gives $\Lambda I=-W>0$, $I=\sum_i m_i|\mathbf a_i|^2$. Pairwise force cancellation implies $\sum_i m_i\mathbf a_i=0$. Such a configuration generates a nonrotating [homothetic gravitational motion](#homothetic-gravitational-motion) by multiplying all position vectors by one positive scale factor.

##### Homothetic gravitational motion

↑ **Parent:** [Newtonian central configuration](#newtonian-central-configuration)

For a [Newtonian central configuration](#newtonian-central-configuration), set $\mathbf x_i(t)=a(t)\mathbf a_i$ with $a>0$. The gravitational force scales as $a^{-2}$, reducing all equations to the displayed scalar [ordinary differential equation](differential-equation.md#ordinary-differential-equation). Its first integral is $\dot a^2/2-\Lambda/a=k/2$. The total [energy](energy.md) is $kI/2$, so the scalar energy constant exactly tracks the many-body energy for the fixed shape.

### Gravitational constant

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gravitational_constant)

The [gravitational constant](#gravitational-constant) $G$ sets the strength of [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md). Two [point masses](classical-mechanics.md#point-mass) $M$ and $m$ a center-to-center distance $r$ apart attract with [force](force.md) magnitude

$$
F=\frac{GMm}{r^2}.
$$

For fixed [masses](classical-mechanics.md#mass) and separation, doubling $G$ would double the [force](force.md). For bodies with [spherical symmetry](geometry-and-topology.md#spherical-symmetry), the same exterior formula follows from the [spherical shell theorem](mathematical-physics.md#spherical-shell-theorem); for arbitrary extended bodies, add the attractions of their [mass density](fluid-mechanics.md#density) elements instead. The [gravitational constant](#gravitational-constant) connects a laboratory attraction to the [Newtonian gravitational field](#newtonian-gravitational-field) controlling a [Kepler orbit](celestial-mechanics.md#kepler-orbit).

The [gravitational constant](#gravitational-constant) $G$ and local [gravitational acceleration](#gravitational-acceleration) $g$ are different quantities. Applying [Newton's second law](force.md#newton-s-second-law) to a [test particle](classical-mechanics.md#test-particle) gives $g=F/m=GM/r^2$ for one spherical source. The source's [mass](classical-mechanics.md#mass) and the observer's [position](classical-mechanics.md#position) change $g$; $G$ remains the same parameter of the law. A local falling-body experiment therefore measures a field, not $G$ alone. On rotating [Earth](planetary-science.md#earth), an instrument fixed to the surface also responds to [centrifugal acceleration](mathematical-physics.md#centrifugal-acceleration), while surrounding [mass density](fluid-mechanics.md#density) and altitude change the gravitational contribution.

[Dimensional analysis](mathematical-physics.md#dimensional-analysis) explains the units. Denote the base [physical dimensions](mathematical-physics.md#physical-dimension) of [length](physics.md#length), [mass](classical-mechanics.md#mass) and [time](classical-mechanics.md#time-in-physics) by $\mathsf L,\mathsf M,\mathsf T$. Since [force](force.md) has dimension $\mathsf M\mathsf L\mathsf T^{-2}$,

$$
[G]=\frac{[F][r]^2}{[M][m]}=\mathsf L^3\mathsf M^{-1}\mathsf T^{-2},\qquad G\text{ has SI unit }\mathrm{m^3\,kg^{-1}\,s^{-2}}.
$$

By contrast, $[g]=\mathsf L\mathsf T^{-2}$ and the [standard gravitational parameter](#standard-gravitational-parameter) $\mu=GM$ has dimension $\mathsf L^3\mathsf T^{-2}$. A small numerical value of a dimensional constant depends on the units chosen: it is the resulting [force](force.md) for specified physical [masses](classical-mechanics.md#mass) and separation that conveys the laboratory scale.

NIST's current complete listing gives

$$
G=6.67430(15)\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}
$$

for the _2022 CODATA adjustment_, the latest adjustment listed when checked on 14 October 2026. Parentheses indicate a [standard uncertainty](physics.md#standard-uncertainty) $u(G)=0.00015\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$, approximately $22$ parts per million relative to $G$. The adjustment year is 2022; NIST's May 2024 data update is a different date.[2022 CODATA adjustment, Newtonian constant of gravitation row: value, uncertainty and units](chemistry-bibliography.md#fundamental-physical-constants-complete-listing-by-national-institute-of-standards-and-technology-and-others) [Current adjustment heading, next-adjustment notice and data-content update](chemistry-bibliography.md#fundamental-physical-constants-complete-listing-by-national-institute-of-standards-and-technology-and-others)

For an original scale calculation, stipulate two $1\,\mathrm{kg}$ [point masses](classical-mechanics.md#point-mass) separated by $1\,\mathrm m$ and insert this recommended $G$: $F=6.67430\times10^{-11}\,\mathrm N$. The corresponding [acceleration](classical-mechanics.md#acceleration) of either [mass](classical-mechanics.md#mass) is $6.67430\times10^{-11}\,\mathrm{m\,s^{-2}}$ at that instant. Reducing the separation to $0.10\,\mathrm m$ multiplies both by $100$. These are ideal model predictions, not observations; their tiny scale explains why stray [forces](force.md) matter.

Being a constant of a physical law does not make the numerical value exact. The [SI](physics.md#international-system-of-units) fixes the numerical values of seven defining constants, including the [speed of light](special-relativity.md#speed-of-light) and [Planck constant](quantum-mechanics.md#planck-constant); $G$ is determined experimentally. Exact unit definitions still require physical realizations with [measurement uncertainty](physics.md#measurement-uncertainty): calibrating a [length](physics.md#length) or a [mass](classical-mechanics.md#mass) does not become error-free.[English §§1.3 and 2.2–2.2.1, printed pp. 122–124: realization, seven defining constants and exact numerical values](physics-bibliography.md#the-international-system-of-units-si-ninth-edition-si-brochure)

#### Gravitational mass degeneracy

↑ **Parent:** [Gravitational constant](#gravitational-constant)

An [orbit](dynamical-systems.md#orbit-dynamical-system) around an isolated source constrains its [standard gravitational parameter](#standard-gravitational-parameter) $\mu=GM$ rather than independently measuring the source's [mass](classical-mechanics.md#mass) and the [gravitational constant](#gravitational-constant). In the [test particle](classical-mechanics.md#test-particle) approximation, a [circular orbit](classical-mechanics.md#circular-orbit) of radius $a$ and [orbital period](celestial-mechanics.md#orbital-period) $T$ satisfies

$$
\frac{4\pi^2a}{T^2}=\frac{GM}{a^2},\qquad \mu=\frac{4\pi^2a^3}{T^2}.
$$

The left equation equates the required [centripetal acceleration](classical-mechanics.md#centripetal-acceleration) to the [gravitational acceleration](#gravitational-acceleration). More generally, a [Kepler orbit](celestial-mechanics.md#kepler-orbit) depends on the same $\mu$. In the exact relative [two-body problem](celestial-mechanics.md#two-body-problem), replace $GM$ by $G(M+m)$.

For any positive dimensionless number $q$, replacing $G$ by $qG$ and $M$ by $M/q$ leaves $GM$ and every predicted [test particle](classical-mechanics.md#test-particle) [trajectory](classical-mechanics.md#trajectory) unchanged. This is the [gravitational mass degeneracy](#gravitational-mass-degeneracy): more observations of the same [orbit](dynamical-systems.md#orbit-dynamical-system) can refine $GM$ without separating its factors. A laboratory source whose [mass](classical-mechanics.md#mass) is calibrated independently supplies the missing information.

Consequently an astronomical [mass](classical-mechanics.md#mass) expressed in kilograms as $M=\mu/G$ inherits [measurement uncertainty](physics.md#measurement-uncertainty) from $G$, even if $\mu$ is known much more precisely. To first order,

$$
\frac{\delta M}{M}=\frac{\delta\mu}{\mu}-\frac{\delta G}{G}.
$$

When the relative [standard uncertainty](physics.md#standard-uncertainty) of $\mu$ is negligible, that of $M$ is approximately $u(G)/G$. Conversely, the ratio of two source [masses](classical-mechanics.md#mass) inferred using the same $G$ is $M_1/M_2=\mu_1/\mu_2$, so this common factor cancels. That distinction explains how excellent [orbit determination](energy.md#orbit-determination) can coexist with less precise absolute astronomical [masses](classical-mechanics.md#mass).

#### Gravitational constant measurement sensitivity

↑ **Parent:** [Gravitational constant](#gravitational-constant)

A laboratory determination of the [gravitational constant](#gravitational-constant) must connect a sensor's reading to a gravitational signal from independently characterized [masses](classical-mechanics.md#mass). For an ideal two-[point mass](classical-mechanics.md#point-mass) [force](force.md) measurement, invert the model:

$$
G_{\mathrm{inferred}}=\frac{Fr^2}{Mm},\qquad \frac{\delta G}{G}\simeq\frac{\delta F}{F}+2\frac{\delta r}{r}-\frac{\delta M}{M}-\frac{\delta m}{m}.
$$

These are signed small changes obtained by taking the [logarithmic derivative](analytic-number-theory.md#logarithmic-derivative), not an instruction to add [standard uncertainties](physics.md#standard-uncertainty) with signs. For independent small input uncertainties, linear [propagation of uncertainty](wave-equation.md#propagation-of-uncertainty) instead gives

$$
\left(\frac{u(G)}G\right)^2\simeq\left(\frac{u(F)}F\right)^2+4\left(\frac{u(r)}r\right)^2+\left(\frac{u(M)}M\right)^2+\left(\frac{u(m)}m\right)^2.
$$

Correlated inputs require their [covariances](variance.md#covariance) too. In particular, common geometric calibration errors must not be treated as independent simply because several distances were recorded.

For a concrete model check, hold the actual [force](force.md) and [masses](classical-mechanics.md#mass) fixed but overestimate a true $r=0.100\,\mathrm m$ by $1\,\mathrm{\mu m}$. The exact inferred ratio is

$$
\frac{G_{\mathrm{inferred}}}{G_{\mathrm{true}}}=(1+10^{-5})^2=1.0000200001.
$$

The resulting bias is $20.0001$ parts per million, already comparable with the relative [standard uncertainty](physics.md#standard-uncertainty) of the recommended [gravitational constant](#gravitational-constant). A sensor can resolve very small changes while its inferred answer remains limited by source geometry. The example concerns one idealized separation; it is not an uncertainty estimate for any actual experiment.

<a id="image-weak-laboratory-attraction-and-the-geometric-sensitivity-of-an-inferred-gravitational-constant"></a>
![](gravitational-constant-scale-and-sensitivity.png)

**[Figure 5](#image-weak-laboratory-attraction-and-the-geometric-sensitivity-of-an-inferred-gravitational-constant). Weak laboratory attraction and the geometric sensitivity of an inferred gravitational constant**. Left: ideal [force](force.md) between two stipulated $1\,\mathrm{kg}$ [point masses](classical-mechanics.md#point-mass) using the 2022 recommended [gravitational constant](#gravitational-constant). Right: exact model bias when only the separation entered in the inference changes. These curves are calculations, not measurement data.

Making the source [mass](classical-mechanics.md#mass) larger or bringing it closer strengthens the signal, but also makes detailed [mass density](fluid-mechanics.md#density) and geometry important. Nearby apparatus supplies its own [Newtonian gravitational field](#newtonian-gravitational-field); electromagnetic shielding does not remove that attraction. Sensor offsets, changing [temperature](temperature.md), vibration and source motion can imitate or alter a signal. The [Cavendish experiment](#cavendish-experiment) illustrates calibration of a [torsion constant](classical-mechanics.md#torsion-constant); a different sensor requires its own calibrated response and a full source model.

Repeating readings can reduce independent [measurement noise](probability-and-statistics.md#measurement-noise), but a fixed scale error survives averaging. A useful experiment deliberately changes the source configuration, checks whether the signal follows the predicted change, and characterizes what moves with the source. A [systematic error](physics.md#systematic-error) that changes with that configuration also survives background subtraction. Comparing methods with different sensors and different dominant errors is therefore valuable.

#### Cold-atom measurement of the gravitational constant

↑ **Parent:** [Gravitational constant](#gravitational-constant)

In 2014, [Gabriele Rosi](physicist.md#gabriele-rosi) and colleagues used [atom interferometry](atomic-physics.md#atom-interferometry): two [rubidium](chemical-substance.md#rubidium)-87 clouds prepared by [laser cooling](atomic-physics.md#laser-cooling) in [vacuum](physics.md#vacuum), $328\,\mathrm{mm}$ apart, received shared three-pulse [Raman transitions](atomic-physics.md#raman-transition) spaced by $160\,\mathrm{ms}$. [Fluorescence](fluorescence.md) readout and paired-fringe [ellipse](euclidean-geometry.md#ellipse) fitting yielded differential [wave phase](wave.md#phase-waves). Twenty-four [tungsten](chemical-substance.md#tungsten) alloy cylinders, about $516\,\mathrm{kg}$ total, moved between C and F. Cloud subtraction rejected shared vibration; configuration subtraction isolated the source change.[Main text pp. 3–5; Methods pp. 13–14; Fig. 1 caption p. 21](physics-bibliography.md#precision-measurement-of-the-newtonian-gravitational-constant-using-cold-atoms-by-gabriele-rosi-and-others)

<a id="image-cold-atom-measurement-two-clouds-and-two-source-configurations"></a>
![](gravitational-constant-atom-interferometer.png)

**[Figure 6](#image-cold-atom-measurement-two-clouds-and-two-source-configurations). Cold-atom measurement: two clouds and two source configurations**. Original conceptual scheme; selected cylinders represent surrounding arrays. Geometry is schematic.[Main text pp. 3–5 and Fig. 1 caption p. 21](physics-bibliography.md#precision-measurement-of-the-newtonian-gravitational-constant-using-cold-atoms-by-gabriele-rosi-and-others)

Calibration used timed flight and light-sheet crossings; mirror tilt compensated [Earth](planetary-science.md#earth) rotation. [Wave vector](elasticity-physics.md#wavevector) reversal rejected unwanted shifts. Modeling included source [Newtonian gravitational potential](#newtonian-gravitational-potential), atom [trajectories](classical-mechanics.md#trajectory), cloud distributions and moving supports. Source positioning, [mass density](fluid-mechanics.md#density) variation and cloud geometry limited the reported combined relative [standard uncertainty](physics.md#standard-uncertainty) to $150$ parts per million.[Main text pp. 5–6; Methods pp. 14–18; Table 1, p. 27](physics-bibliography.md#precision-measurement-of-the-newtonian-gravitational-constant-using-cold-atoms-by-gabriele-rosi-and-others)

To understand the subtraction without reproducing that full analysis, consider an ideal [atom interferometer](atomic-physics.md#atom-interferometer) in uniform vertical [acceleration](classical-mechanics.md#acceleration) during each pulse sequence. Let $k_{\mathrm{eff}}$ be its signed effective vertical [wave vector](elasticity-physics.md#wavevector) component and $T$ the pulse spacing. Its acceleration-dependent [wave phase](wave.md#phase-waves) is $\phi\simeq k_{\mathrm{eff}}gT^2$; labels U and L denote upper and lower clouds. The double difference is then

$$
S=(\phi_U-\phi_L)_C-(\phi_U-\phi_L)_F\simeq k_{\mathrm{eff}}T^2[(g_U-g_L)_C-(g_U-g_L)_F].
$$

A background field identical in C and F cancels even if it differs between the two clouds. In a fixed-geometry, linear-response model, write $S=G\mathcal K$, where $\mathcal K$ is calculated from the source [mass density](fluid-mechanics.md#density), calibrated pulse sequence and atom [trajectories](classical-mechanics.md#trajectory). Thus $G_{\mathrm{inferred}}=S/\mathcal K$. Measuring [wave phase](wave.md#phase-waves) accurately is one part of the task; calculating $\mathcal K$ accurately is another. The real nonuniform field and finite clouds require the trajectory-dependent analysis described above rather than this uniform-field approximation.

### Poisson equation for Newtonian gravity

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

For [mass density](fluid-mechanics.md#density) $\rho$, the [Newtonian gravitational potential](#newtonian-gravitational-potential) satisfies the [Poisson equation](partial-differential-equation.md#poisson-s-equation) $\nabla^2\Phi=4\pi G\rho$. The gravitational acceleration is $-\nabla\Phi$. An isolated system also requires the exterior vacuum solution and decay at infinity; solving the interior equation alone does not fix a globally physical field.

#### Dyadic spherical shells with inverse-radius density scaling

↑ **Parent:** [Poisson equation for Newtonian gravity](#poisson-equation-for-newtonian-gravity)

Suppose the shell $2^{-n}<r<2^{1-n}$ has [mass density](fluid-mechanics.md#density) $2^{n-1}\rho_0$. Its mass is $(14\pi\rho_0/3)4^{-n}$, by integrating $4\pi r^2\rho\,dr$. Summing the [geometric series](sequence-and-series.md#geometric-series) gives total mass $14\pi\rho_0/9$. At $r=2^{-N}$ the enclosed shells have indices $n\geq N+1$, so the enclosed mass is the total mass times $r^2$. The magnitude of the [Newtonian gravitational field](#newtonian-gravitational-field) at every such boundary is therefore the same, $14\pi G\rho_0/9$. This does not assert that the field is constant throughout each shell.

### Newtonian gravitational potential

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

The [Newtonian gravitational potential](#newtonian-gravitational-potential) $\Phi$ is [potential energy](energy.md#potential-energy) per unit [mass](classical-mechanics.md#mass) of a [test particle](classical-mechanics.md#test-particle). Its [gradient](multivariable-calculus.md#gradient) determines the [Newtonian gravitational field](#newtonian-gravitational-field):

$$
U=m\Phi,\qquad \mathbf g=-\nabla\Phi,\qquad \mathbf F=-\nabla U=-m\nabla\Phi.
$$

In [SI](physics.md#international-system-of-units), $U$ has units $\mathrm J$, while $\Phi$ has units $\mathrm{J\,kg^{-1}}=\mathrm{m^2\,s^{-2}}$; its [gradient](multivariable-calculus.md#gradient) has units of [acceleration](classical-mechanics.md#acceleration), not [force](force.md). Adding a constant to $\Phi$ leaves the [Newtonian gravitational field](#newtonian-gravitational-field) unchanged. For an isolated [point mass](classical-mechanics.md#point-mass), the convenient reference is $\Phi(\infty)=0$. [Peraire and Widnall, MIT Dynamics, Lecture 16: potential per unit mass](https://ocw.mit.edu/courses/16-07-dynamics-fall-2009/0bb19205a6316ba88f88284bf7257ec6_MIT16_07F09_Lec16.pdf)

Increasing the radius from $r_0$ to $r_1>r_0$ raises the [Newtonian gravitational potential energy](#newtonian-gravitational-potential-energy):

$$
\Delta U=GMm\left(\frac1{r_0}-\frac1{r_1}\right)>0.
$$

An external agent supplies this positive [work](energy.md#work) if the initial and final [kinetic energies](energy.md#kinetic-energy) agree; gravity does [work](energy.md#work) $-\Delta U$. For $r_1=2r_0$, the required [work](energy.md#work) is $GMm/(2r_0)$. [13.3 Gravitational Potential Energy and Total Energy](physics-bibliography.md#university-physics-volume-1-by-william-moebs-and-others/13-3-gravitational-potential-energy-and-total-energy)

#### Gravitational potential of a sinusoidal sheet

↑ **Parent:** [Newtonian gravitational potential](#newtonian-gravitational-potential)

A sinusoidal surface-density component $\Sigma_k\cos(kx)$ on $y=0$, with $k>0$ and translational invariance in the remaining direction, produces the displayed [gravitational potential](#newtonian-potential-of-a-point-mass). [Laplace's equation](partial-differential-equation.md#laplace-equation) away from the sheet separates into a cosine in $x$ and a decaying exponential in $|y|$. Continuity across the sheet excludes a potential jump, while integrating [Poisson equation for Newtonian gravity](#poisson-equation-for-newtonian-gravity) across it gives $[\Phi_y]_{0^-}^{0^+}=4\pi G\Sigma_k\cos(kx)$. For a potential $C\cos(kx)e^{-k|y|}$ that derivative jump is $-2kC\cos(kx)$, giving $C=-2\pi G\Sigma_k/k$.

More generally a specified jump $J\cos(kx)$ gives potential $-J\cos(kx)e^{-k|y|}/(2k)$. Each spatial [Fourier mode](fourier-analysis.md#fourier-mode) decays on the length scale $1/k$, so fine density structure has a shorter-range field. The sinusoid changes sign and is naturally interpreted as a density perturbation component. General sheet distributions are built by superposing their [Fourier modes](fourier-analysis.md#fourier-mode); decay alone does not restrict a harmonic potential to a single mode.

#### Newtonian gravitational potential of a uniform solid sphere

↑ **Parent:** [Newtonian gravitational potential](#newtonian-gravitational-potential)

For radius $R$, constant [mass density](fluid-mechanics.md#density) $\rho$ and $M=4\pi\rho R^3/3$, normalize the [Newtonian gravitational potential](#newtonian-gravitational-potential) to zero at infinity. Then

$$
\boxed{\Phi(r)=\begin{cases}-\dfrac{GM}{2R^3}(3R^2-r^2),&0\leq r\leq R,\\-GM/r,&r\geq R.\end{cases}}
$$

By the [spherical shell theorem](mathematical-physics.md#spherical-shell-theorem), each spherical shell contributes the potential of a point mass outside it and a constant inside it. Summing inner and outer shells gives $\Phi(r)=-4\pi G\rho[r^2/3+(R^2-r^2)/2]$ inside. Equivalently, angular integration of the free-space [Green function of the Laplacian](partial-differential-equation.md#green-function-of-the-laplacian) gives $\int_{-1}^1(r^2+r'^2-2rr'\mu)^{-1/2}d\mu=[r+r'-|r-r'|]/(rr')$. The resulting radial integral has the same value.

The potential and its first radial derivative are continuous at $R$. The interior [gravitational acceleration](#gravitational-acceleration) is $-\nabla\Phi=-(GM/R^3)\mathbf r$, and $\nabla^2\Phi=4\pi G\rho$. At the centre $\Phi(0)=-3GM/(2R)$ while its gradient vanishes.

#### Planetary quadrupole coefficient

↑ **Parent:** [Newtonian gravitational potential](#newtonian-gravitational-potential)

The dimensionless coefficient $J_2$ describes the leading axisymmetric departure of a planet's external [Newtonian gravitational potential](#newtonian-gravitational-potential) from a monopole: $\Phi=-GM_p/r+[GM_pJ_2R_p^2/r^3]P_2(\cos\vartheta)$, where $\vartheta$ is colatitude from the spin axis. An oblate mass distribution has positive $J_2$. The [disturbing function](planetary-science.md#disturbing-function) is minus the nonspherical potential term. On a circular inclined [Kepler orbit](celestial-mechanics.md#kepler-orbit), $\cos\vartheta=\sin I\sin M$, so [orbit averaging](planetary-science.md#orbit-averaging) gives $\overline{\mathcal R}_{J_2}=GM_pJ_2R_p^2a^{-3}(1/2-3\sin^2I/4)$. The exact circular nodal rate is $-3nJ_2(R_p/a)^2\cos I/2$; its small-tilt limit is $-3nJ_2(R_p/a)^2/2$.

##### Oblate-quadrupole epicyclic precession

↑ **Parent:** [Planetary quadrupole coefficient](#planetary-quadrupole-coefficient)

For $\Phi=-\mu/r+\alpha^2\mu(3z^2-r^2)/r^5$, a nearly circular equatorial orbit has $n^2=\mu/R^3$ and azimuthal frequency $\Omega_c^2=n^2(1+3\alpha^2/R^2)$. The [radial epicyclic frequency](astrophysical-disk.md#radial-epicyclic-frequency) is $\kappa^2=R\,d\Omega_c^2/dR+4\Omega_c^2$, and the [vertical epicyclic frequency](astrophysical-disk.md#vertical-epicyclic-frequency) is $\nu^2=\partial_z^2\Phi|_{z=0}$. Radial stability requires $R^2>3\alpha^2$. The [nodal precession](planetary-science.md#nodal-precession) rate $\Omega_c-\nu$ is negative and the [apsidal precession](planetary-science.md#apsidal-precession) rate $\Omega_c-\kappa$ positive. These sign statements concern small eccentricity and inclination. For an arbitrary inclined orbit, the averaged [argument of periapsis](celestial-mechanics.md#argument-of-periapsis) instead evolves as $(3/2)n\alpha^2[5\cos^2i-1]/[a^2(1-e^2)^2]$ and can regress.

#### Axisymmetric logarithmic gravitational potential

↑ **Parent:** [Newtonian gravitational potential](#newtonian-gravitational-potential)

An axisymmetric logarithmic [Newtonian gravitational potential](#newtonian-gravitational-potential) has spheroidal equipotential surfaces and a [flat galaxy rotation curve](galaxy.md#flat-galaxy-rotation-curve): $R\Phi_R(R,0)=V^2$. The singular model is defined away from the origin; a fixed reference length makes the logarithm dimensionless. Its central $r^{-2}$ [mass density](fluid-mechanics.md#density) cusp is locally integrable, but its total [mass](classical-mechanics.md#mass) diverges at large radius.

##### Density positivity for an axisymmetric logarithmic potential

↑ **Parent:** [Axisymmetric logarithmic gravitational potential](#axisymmetric-logarithmic-gravitational-potential)

The [Poisson equation for Newtonian gravity](#poisson-equation-for-newtonian-gravity) gives

$$
\rho=\frac{V^2}{4\pi Gq^2}\frac{R^2+(2-q^{-2})z^2}{(R^2+q^{-2}z^2)^2}.
$$

For $V>0$, nonnegative [mass density](fluid-mechanics.md#density) away from the origin is equivalent to $q^2\geq1/2$. Strict positivity requires $q^2>1/2$. This condition does not by itself guarantee a nonnegative [galactic distribution function](galaxy.md#galactic-distribution-function).

#### Power-law gravitational potential

↑ **Parent:** [Newtonian gravitational potential](#newtonian-gravitational-potential)

A radial [Newtonian gravitational potential](#newtonian-gravitational-potential) $\Phi=-Ar^{-\beta}$ produces inward acceleration $A\beta r^{-\beta-1}$. The point-mass case has $\beta=1$ and $A=GM$. Treating the [power-law gravitational potential](#power-law-gravitational-potential) as prescribed does not require it to be sourced by the flowing gas.

#### Gravitational quadrupole potential of a point-mass binary

↑ **Parent:** [Newtonian gravitational potential](#newtonian-gravitational-potential)

For a [binary star](stellar-astrophysics.md#binary-star) viewed far from its [centre of mass](classical-mechanics.md#center-of-mass), let $\mathbf r$ be the separation and $\mu$ the [reduced mass](classical-mechanics.md#reduced-mass), $M=M_1+M_2$ the total [mass](classical-mechanics.md#mass), $r=|\mathbf r|$ and $x=|\mathbf x|$. The [Taylor expansion](calculus.md#taylor-expansion) of the point-mass [Newtonian gravitational potential](#newtonian-gravitational-potential) has zero dipole because $\sum_A M_A\mathbf x_A=0$. Its second moment is $\sum_A M_Ax_{Ai}x_{Aj}=\mu r_i r_j$, so

$$
\Phi=-\frac{GM}{x}-\frac{G\mu}{2x^5}\left[3(\mathbf x\cdot\mathbf r)^2-x^2r^2\right]+O(GMr^3/x^4).
$$

This holds for an instantaneous separation in any orbit, not only a [circular orbit](classical-mechanics.md#circular-orbit). The [mass quadrupole moment](gravitational-wave.md#mass-quadrupole-moment) convention $Q_{ij}=\mu(r_ir_j-r^2\delta_{ij}/3)$ gives $\Phi_2=-3GQ_{ij}x_ix_j/(2x^5)$.

#### Flattened power-law gravitational potential

↑ **Parent:** [Newtonian gravitational potential](#newtonian-gravitational-potential)

A flattened power-law [Newtonian gravitational potential](#newtonian-gravitational-potential) has equipotential spheroids $R^2+\lambda^2z^2=\text{constant}$. For $\Phi_0<0$ and $0<\beta<1$, its midplane [circular orbit](classical-mechanics.md#circular-orbit) angular frequency satisfies $\Omega^2=-\beta\Phi_0R_0^\beta R^{-\beta-2}$.

##### Density positivity for a flattened power-law potential

↑ **Parent:** [Flattened power-law gravitational potential](#flattened-power-law-gravitational-potential)

Applying the [Poisson equation for Newtonian gravity](#poisson-equation-for-newtonian-gravity) to a [flattened power-law gravitational potential](#flattened-power-law-gravitational-potential) yields

$$
\rho=-\frac{\beta\Phi_0R_0^\beta}{4\pi G}\frac{(\lambda^2-\beta)R^2+\lambda^2[2-(\beta+1)\lambda^2]z^2}{(R^2+\lambda^2z^2)^{(\beta+4)/2}}.
$$

For $0<\beta<1$, nonnegative [mass density](fluid-mechanics.md#density) everywhere outside the origin requires and is ensured by $\beta\leq\lambda^2\leq2/(\beta+1)$. The central density singularity is locally integrable and carries no point mass, although the total mass diverges at large radius in this scale-free model.

#### Newtonian potential of a point mass

↑ **Parent:** [Newtonian gravitational potential](#newtonian-gravitational-potential)

The [Newtonian potential of a point mass](#newtonian-potential-of-a-point-mass) $M$ at the origin is

$$
\Phi(r)=-\frac{GM}{r},\qquad r>0,\qquad \Phi(\infty)=0.
$$

It is the free-space [Green function of the Laplacian](partial-differential-equation.md#green-function-of-the-laplacian) with the normalization of the [Poisson equation for Newtonian gravity](#poisson-equation-for-newtonian-gravity). Differentiating gives inward [gravitational acceleration](#gravitational-acceleration) $-GM/r^2$. With $z=r/r_0$, the normalized [Newtonian gravitational potential](#newtonian-gravitational-potential) is $\Phi/(GM/r_0)=-1/z$; at $z=1,2,4$ it equals $-1,-1/2,-1/4$.

For a radially outward launch from $r_0$, [conservation of mechanical energy](energy.md#conservation-of-mechanical-energy) in the fixed-source [test particle](classical-mechanics.md#test-particle) approximation gives the minimum [escape velocity](energy.md#escape-velocity):

$$
\frac{E}{m}=\frac{v_0^2}{2}-\frac{GM}{r_0}=0
\quad\Longrightarrow\quad v_{\mathrm{esc}}=\sqrt{\frac{2GM}{r_0}}.
$$

At this threshold the [speed](classical-mechanics.md#speed) tends to zero only at infinite separation. The model neglects air resistance, external [tidal forces](#tidal-force), and [general relativity](general-relativity.md). [13.3 Gravitational Potential Energy and Total Energy](physics-bibliography.md#university-physics-volume-1-by-william-moebs-and-others/13-3-gravitational-potential-energy-and-total-energy)

A [circular orbit](classical-mechanics.md#circular-orbit) at $r_0$ instead requires tangential [speed](classical-mechanics.md#speed) $v_c=\sqrt{GM/r_0}$. Choosing units with $G=M=r_0=1$ gives $g_0=1$, $v_c=1$, and $v_{\mathrm{esc}}=\sqrt2\simeq1.41421$. A radial launch at [speed](classical-mechanics.md#speed) $1$ reaches $r=2$ and returns; the same [speed](classical-mechanics.md#speed) directed tangentially gives a [circular orbit](classical-mechanics.md#circular-orbit). [13.4 Satellite Orbits and Energy](physics-bibliography.md#university-physics-volume-1-by-william-moebs-and-others/13-4-satellite-orbits-and-energy)

<a id="image-energy-balance-and-outward-radial-speeds-below-at-and-above-escape"></a>
![](gravitational-escape-energy.png)

**[Figure 7](#image-energy-balance-and-outward-radial-speeds-below-at-and-above-escape). Energy balance and outward radial speeds below, at, and above escape**. Left: at the [escape velocity](energy.md#escape-velocity), positive [kinetic energy](energy.md#kinetic-energy) exactly balances negative [Newtonian gravitational potential energy](#newtonian-gravitational-potential-energy). Right: radial launches at normalized [speeds](classical-mechanics.md#speed) $1$, $\sqrt2$, and $1.6$ respectively turn at $r/r_0=2$, approach zero [speed](classical-mechanics.md#speed) at infinity, and retain a positive limiting [speed](classical-mechanics.md#speed). The plotted trajectories use a fixed source and the [test particle](classical-mechanics.md#test-particle) approximation.

##### Self-gravity in a thin spherical shell expansion

↑ **Parent:** [Newtonian potential of a point mass](#newtonian-potential-of-a-point-mass)

A shell of fixed mass $M_s$ and radius $R$ has self-energy $-GM_s^2/(2R)$. Its inward generalized force opposing an increase of radius is $GM_s^2/(2R^2)$. Including this in a swept-gas shell threshold changes an interior-only factor $f(1-f)$ to $f(1-f/2)$ when the original total mass is held fixed.

##### Gravitational potential of a truncated inverse-radius sphere

↑ **Parent:** [Newtonian potential of a point mass](#newtonian-potential-of-a-point-mass)

The sphere $\rho=k^\prime/(2\pi Gr)$ for $r<r_0$ has $M(r)=k^\prime r^2/G$ and $\Phi(r)=-k^\prime(2r_0-r)$, with zero potential at infinity. Its finite central potential contrasts with the logarithmic central divergence of a truncated inverse-square density.

##### Axisymmetric gravitational potential of a displaced cylindrical interface

↑ **Parent:** [Newtonian potential of a point mass](#newtonian-potential-of-a-point-mass)

Consider a uniform-density cylinder with an axisymmetric radial [Fourier mode](fourier-analysis.md#fourier-mode) $\eta=\epsilon e^{ikz}$. Its displaced boundary gives a first-order [surface mass density](fluid-mechanics.md#projected-surface-mass-density) $\rho\eta$, although the interior density perturbation vanishes. The gravitational [Poisson equation](partial-differential-equation.md#poisson-s-equation) reduces to [Laplace equation](partial-differential-equation.md#laplace-equation) away from the interface. Regularity internally and decay externally give $\psi_{\rm in}=AI_0(kr)e^{ikz}$ and $\psi_{\rm out}=BK_0(kr)e^{ikz}$. Continuity at $R$ and the derivative jump $\psi'_{\rm out}-\psi'_{\rm in}=4\pi G\rho\epsilon e^{ikz}$, together with $I_0(\kappa)K'_0(\kappa)-I'_0(\kappa)K_0(\kappa)=-1/\kappa$, give the title amplitude. The prime differentiates the [modified Bessel function](bessel-function.md#modified-bessel-function) argument. This axial mode is different from an azimuthal mode on a [gravitational potential of a displaced cylindrical interface](astrophysical-fluid-dynamics.md#gravitational-potential-of-a-displaced-cylindrical-interface).

#### Spherically symmetric potential

↑ **Parent:** [Newtonian gravitational potential](#newtonian-gravitational-potential)

A spherically symmetric potential depends only on distance $r$ from one point. Its force is central, so angular momentum is conserved.

### Newtonian gravitational potential energy

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)

Two point masses $m_1,m_2$ separated by distance $r$ have [potential energy](energy.md#potential-energy)

$$
V(r)=-\frac{Gm_1m_2}{r}.
$$

The corresponding attractive force is $-\nabla V$.

This is the Newtonian point-mass specialization of [gravitational energy](energy.md#gravitational-energy), with the reference value chosen at infinite separation.

#### Spherical binding-energy mass integral

↑ **Parent:** [Newtonian gravitational potential energy](#newtonian-gravitational-potential-energy)

Assembling a spherical mass distribution in shells gives [gravitational potential energy](energy.md#gravitational-energy) $W=-G\int M(r)\,dM(r)/r$. Integration by parts gives the displayed identity when $M(r)^2/r$ vanishes at both endpoints. It includes each interacting pair once; no extra factor of one half belongs in the original shell-assembly integral.

#### Minimum-separation binding-energy bounds

↑ **Parent:** [Newtonian gravitational potential energy](#newtonian-gravitational-potential-energy)

For positive [masses](classical-mechanics.md#mass), let $r$ be the actual minimum pairwise separation and use positive binding [energy](energy.md) $U=\sum_{j<k}Gm_jm_k/r_{jk}$. If $m_{(1)},m_{(2)}$ are the smallest [masses](classical-mechanics.md#mass), then $Gm_{(1)}m_{(2)}\leq rU\leq G\sum_{j<k}m_jm_k$. Thus $U^{-1}$ is comparable to $r$ with constants depending only on the masses.

##### Negative-energy minimum-separation upper bound

↑ **Parent:** [Minimum-separation binding-energy bounds](#minimum-separation-binding-energy-bounds)

With $E=T-U<0$ and $T\geq0$, the positive binding [energy](energy.md) satisfies $U\geq|E|$. The [minimum-separation binding-energy bounds](#minimum-separation-binding-energy-bounds) imply $r\leq A_0/|E|$. At least one pair stays close; this does not bound every particle's distance or exclude a [negative-energy gravitational collision](celestial-mechanics.md#negative-energy-gravitational-collision).

### Cavendish experiment

↑ **Parent:** [Newtonian gravitational field](#newtonian-gravitational-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cavendish_experiment)

The [Cavendish experiment](#cavendish-experiment) makes the attraction predicted by [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md) measurable between laboratory [masses](classical-mechanics.md#mass). Two small test [masses](classical-mechanics.md#mass) hang at the ends of a horizontal rod in a [Cavendish torsion balance](#cavendish-torsion-balance); nearby larger source [masses](classical-mechanics.md#mass) exert a tiny [torque](momentum.md#torque). A thin suspension fiber supplies an opposing [torque](momentum.md#torque) as it twists. Measuring its twist and calibrating its [torsion constant](classical-mechanics.md#torsion-constant) lets an experimenter infer the gravitational [force](force.md) and, in a modern analysis, the [gravitational constant](#gravitational-constant). [University of Connecticut, Physics 258/259, The Cavendish Experiment: apparatus and equations of motion, pp. 1–3](https://www.phys.uconn.edu/~hamilton/phys258/N/cav.pdf)

The beautiful feature is that the two horizontal [forces](force.md) can cancel as vectors while their [torques](momentum.md#torque) add. The instrument converts weak attraction into a rotation, with sensitivity set by the fiber's [torsion constant](classical-mechanics.md#torsion-constant). Earth's much larger downward [gravitational weight](force.md#weight-physics) is supported by the suspension rather than supplying the intended [torque](momentum.md#torque) about its vertical axis. A laboratory measurement can therefore probe the same [Newtonian gravitational field](#newtonian-gravitational-field) that governs the [two-body problem](celestial-mechanics.md#two-body-problem).

Henry Cavendish's original paper was _Experiments to determine the Density of the Earth_, published in _Philosophical Transactions_, volume 88 (1798), pp. 469–526, and read on 21 June 1798. On p. 469 he credits John Michell with the apparatus idea and explains that Michell died before using it; the instrument reached Cavendish through Francis John Hyde Wollaston. Cavendish's stated aim was Earth's mean [mass density](fluid-mechanics.md#density). Calling the experiment a determination of the [gravitational constant](#gravitational-constant) is a modern interpretation, not Cavendish's own formulation of his result. [Cavendish (1798), original paper, opening p. 469; DOI 10.1098/rstl.1798.0022](https://www.famaf.unc.edu.ar/~wolf/FisicaI/Phil.%20Trans.%20R.%20Soc.%20Lond.-1798-Cavendish-rstl.1798.0022.pdf)

The connection between Earth's mean [mass density](fluid-mechanics.md#density) and the [gravitational constant](#gravitational-constant) follows in a spherical, nonrotating model of [Earth](planetary-science.md#earth). With Earth [mass](classical-mechanics.md#mass) $M_E$, radius $R_E$, and surface [gravitational acceleration](#gravitational-acceleration) $g$, the [spherical shell theorem](mathematical-physics.md#spherical-shell-theorem) and [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md) give

$$
g=\frac{GM_E}{R_E^2},\qquad \overline\rho_E=\frac{3M_E}{4\pi R_E^3},\qquad G=\frac{3g}{4\pi R_E\overline\rho_E}.
$$

Thus a local comparison of gravitational attractions, together with knowledge of Earth's size and surface [gravitational acceleration](#gravitational-acceleration), reaches a property of the entire planet. These are modern equations explaining the connection, not equations quoted from Cavendish's paper.

For a worked example, use an explicitly simplified two-near-pair model. Each test [point mass](classical-mechanics.md#point-mass) is $m$, each source [point mass](classical-mechanics.md#point-mass) is $M$, and each [lever arm](momentum.md#lever-arm) is $L$, so the rod's full [length](physics.md#length) is $2L$. Neglect the rod's [mass](classical-mechanics.md#mass). At zero twist put the test [masses](classical-mechanics.md#mass) at $(-L,0)$ and $(L,0)$, and the sources at $(-L,-r)$ and $(L,r)$. Here $r$ is the near-pair center separation. Ignore each source's attraction on the test [mass](classical-mechanics.md#mass) at the opposite end. Evaluate the two near-pair [forces](force.md) at zero twist and treat their [torque](momentum.md#torque) as constant for a small twist, requiring $L|\theta|\ll r$. This is a teaching model, not a precision model of Cavendish's actual apparatus.

By [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md), each retained [force](force.md) has magnitude $F=GmM/r^2$. The left [force](force.md) points down and the right [force](force.md) points up. Using [torque](momentum.md#torque) about the suspension axis, both contributions are counterclockwise when viewed from above:

$$
\tau_{z,\mathrm{left}}=(-L)(-F)=LF,\qquad \tau_{z,\mathrm{right}}=LF,\qquad |\tau_g|=2L\frac{GmM}{r^2}.
$$

The net retained horizontal [force](force.md) is zero, yet the net [torque](momentum.md#torque) is positive. Moving the sources to $(-L,r)$ and $(L,-r)$ reverses both [forces](force.md) and hence the [torque](momentum.md#torque). In a real apparatus, the opposite source also attracts each test [mass](classical-mechanics.md#mass); that correction is explicitly included in the university derivation. [University of Connecticut, The Cavendish Experiment, p. 2, equation (1): opposite-source correction](https://www.phys.uconn.edu/~hamilton/phys258/N/cav.pdf)

<a id="image-two-near-pair-forces-give-the-same-counterclockwise-torque-about-a-vertical-suspension-fiber"></a>
![](cavendish-torsion-balance-schematic.png)

**[Figure 8](#image-two-near-pair-forces-give-the-same-counterclockwise-torque-about-a-vertical-suspension-fiber). Two near-pair forces give the same counterclockwise torque about a vertical suspension fiber**.

For illustrative parameters, take $m=0.010\,\mathrm{kg}$, $M=1.0\,\mathrm{kg}$, $r=0.050\,\mathrm m$, $L=0.10\,\mathrm m$, and [torsion constant](classical-mechanics.md#torsion-constant) $\kappa=1.0\times10^{-8}\,\mathrm{N\,m/rad}$. Use $G=6.67430\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$, the central value in NIST's 2022 CODATA table; that table gives standard uncertainty $0.00015\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$. This is an input for the example, not a measurement made with these assumed parameters. [Fundamental Physical Constants — Complete Listing by National Institute of Standards and Technology and others](chemistry-bibliography.md#fundamental-physical-constants-complete-listing-by-national-institute-of-standards-and-technology-and-others)

$$
F=\frac{(6.67430\times10^{-11})(0.010)(1.0)}{(0.050)^2}=2.66972\times10^{-10}\,\mathrm N,\qquad |\tau_g|=2(0.10)F=5.33944\times10^{-11}\,\mathrm{N\,m}.
$$

This sub-nanonewton [force](force.md) produces a measurable twist in the [Cavendish torsion balance](#cavendish-torsion-balance). The displayed digits make the toy calculation reproducible; they do not describe experimental precision.

#### Cavendish torsion balance

↑ **Parent:** [Cavendish experiment](#cavendish-experiment)

A [Cavendish torsion balance](#cavendish-torsion-balance) is a [torsion balance](classical-mechanics.md#torsion-balance) arranged to measure gravitational [torque](momentum.md#torque) from nearby source [masses](classical-mechanics.md#mass). Its suspended horizontal rod rotates about a vertical fiber. In the linear elastic regime, a twist [angle](geometry-and-topology.md#angle) $\theta$, measured from the fiber's untwisted orientation, gives a restoring [torque](momentum.md#torque) $\tau_{\mathrm{fiber}}=-\kappa\theta$, where $\kappa>0$ is the [torsion constant](classical-mechanics.md#torsion-constant). The minus sign is essential: the fiber resists the twist. Under an approximately constant gravitational [torque](momentum.md#torque), the rotational equation using [moment of inertia](rigid-body-dynamics.md#moment-of-inertia) $I$ and [angular acceleration](rigid-body-dynamics.md#angular-acceleration) $\ddot\theta$ is

$$
I\ddot\theta=\tau_g-\kappa\theta,\qquad \theta_{\mathrm{eq}}=\frac{\tau_g}{\kappa}.
$$

At [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system), the two [torques](momentum.md#torque) balance. The [angle](geometry-and-topology.md#angle) is a displacement from the fiber's reference orientation, not the largest excursion during an [oscillation](wave.md#oscillation). [University of Connecticut, The Cavendish Experiment, pp. 2–3: restoring torque and equilibrium deflection](https://www.phys.uconn.edu/~hamilton/phys258/N/cav.pdf)

For the toy parameters in the [Cavendish experiment](#cavendish-experiment), the predicted [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) twist is

$$
\theta_{\mathrm{eq}}=\frac{5.33944\times10^{-11}}{1.0\times10^{-8}}=0.00533944\,\mathrm{rad}\simeq0.3059^\circ.
$$

Here $L|\theta_{\mathrm{eq}}|/r\simeq0.0107$, consistent with using a small geometric displacement in the toy model, but not an estimate of its total [measurement error](probability-and-statistics.md#measurement-error). Reversing the source positions ideally takes the [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) [angle](geometry-and-topology.md#angle) from $+\theta_{\mathrm{eq}}$ to $-\theta_{\mathrm{eq}}$: the magnitude of the change is $2|\theta_{\mathrm{eq}}|\simeq0.6119^\circ$. A stable zero offset then cancels in the difference. A real reading may track a reflected light spot; the [law of reflection](geometrical-optics.md#law-of-reflection) doubles a mirror's rotation in the outgoing beam, so the spot's angular change must not be confused with the rod's [angle](geometry-and-topology.md#angle). [Harvard Natural Sciences Lecture Demonstrations, Cavendish Experiment: mirror readout and source reversal](https://sciencedemonstrations.fas.harvard.edu/presentations/cavendish-experiment)

How can the fiber's [torsion constant](classical-mechanics.md#torsion-constant) be found without already knowing the gravitational [force](force.md)? Measure the [oscillation period](classical-mechanics.md#period-of-an-oscillation) and calculate the [moment of inertia](rigid-body-dynamics.md#moment-of-inertia). For the same toy rod, neglecting its [mass](classical-mechanics.md#mass) and treating both test [masses](classical-mechanics.md#mass) as [point masses](classical-mechanics.md#point-mass), $I=mL^2+mL^2=2mL^2$. With the source [torque](momentum.md#torque) absent or treated as constant, let $\phi=\theta-\theta_{\mathrm{eq}}$ be a small departure from [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system). Neglect [damping](wave-equation.md#damping) and any change of gravitational [torque](momentum.md#torque) with [angle](geometry-and-topology.md#angle). The rotational equation becomes [simple harmonic motion](classical-mechanics.md#simple-harmonic-motion):

$$
I\ddot\phi+\kappa\phi=0,\qquad \phi(t)=A\cos(\omega t+\delta),\qquad \omega=\sqrt{\frac{\kappa}{I}},\qquad T=2\pi\sqrt{\frac I\kappa},\qquad \kappa=\frac{4\pi^2I}{T^2}.
$$

Here $A$ is the angular amplitude, $\delta$ specifies the initial phase, and $\omega$ is the [angular frequency](lagrangian-mechanics.md#angular-frequency). A softer fiber gives a larger [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) twist but also a longer [oscillation period](classical-mechanics.md#period-of-an-oscillation): greater sensitivity costs observation time. An undamped [oscillation](wave.md#oscillation) does not settle at [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system); [damping](wave-equation.md#damping) is needed for settling. [University of Connecticut, The Cavendish Experiment, p. 3, equation (7): period calibration neglecting damping](https://www.phys.uconn.edu/~hamilton/phys258/N/cav.pdf)

The toy [moment of inertia](rigid-body-dynamics.md#moment-of-inertia) and undamped [oscillation period](classical-mechanics.md#period-of-an-oscillation) are

$$
I=2(0.010)(0.10)^2=2.0\times10^{-4}\,\mathrm{kg\,m^2},\qquad T=2\pi\sqrt{\frac{2.0\times10^{-4}}{1.0\times10^{-8}}}\simeq888.5766\,\mathrm s\simeq14.81\,\mathrm{min}.
$$

Timing this [oscillation period](classical-mechanics.md#period-of-an-oscillation) would recover the assumed [torsion constant](classical-mechanics.md#torsion-constant). The units check explains the result: [torque](momentum.md#torque) divided by [torsion constant](classical-mechanics.md#torsion-constant) is an [angle](geometry-and-topology.md#angle) in [radians](geometry-and-topology.md#radian), and $I/\kappa$ has units of [time](classical-mechanics.md#time-in-physics) squared when [radians](geometry-and-topology.md#radian) are treated as dimensionless in [SI](physics.md#international-system-of-units).

<a id="image-undamped-small-torsional-oscillations-calibrate-the-restoring-torque-a-softer-fiber-has-a-longer-period"></a>
![](torsion-balance-period-calibration.png)

**[Figure 9](#image-undamped-small-torsional-oscillations-calibrate-the-restoring-torque-a-softer-fiber-has-a-longer-period). Undamped small torsional oscillations calibrate the restoring torque: a softer fiber has a longer period**.

Combining the [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) twist with the period calibration, the two-near-pair model would infer the [gravitational constant](#gravitational-constant) as

$$
G=\frac{\kappa|\theta_{\mathrm{eq}}|r^2}{2LmM}=\frac{4\pi^2Lr^2|\theta_{\mathrm{eq}}|}{MT^2}.
$$

The test [mass](classical-mechanics.md#mass) cancels in the second expression because it enters both the gravitational [torque](momentum.md#torque) and the toy [moment of inertia](rigid-body-dynamics.md#moment-of-inertia). If the measured quantity is the magnitude $|\Delta\theta|$ of the change between opposite source positions, use $|\theta_{\mathrm{eq}}|=|\Delta\theta|/2$. Substituting the toy twist and [oscillation period](classical-mechanics.md#period-of-an-oscillation) returns the input $G$; it is a consistency check, not independent experimental evidence.

The sensitivity of a [Cavendish torsion balance](#cavendish-torsion-balance) also explains its practical difficulty. Air motion can exert unwanted [torque](momentum.md#torque); unequal [temperatures](temperature.md) can drive that motion. Cavendish discusses this effect on p. 471 and describes observing from outside a closed room to avoid disturbing the instrument. [Cavendish (1798), original paper, p. 471: temperature-driven air currents and remote observation](https://www.infinitoteatrodelcosmo.it/wp-content/uploads/2021/07/cavendish-1997-xxi-experiments-to-determine-the-density-of-the-earth.pdf) Mechanical vibrations can excite the same slow [oscillations](wave.md#oscillation) used to calibrate the [torsion constant](classical-mechanics.md#torsion-constant), while changes in the fiber or source separations alter the inferred [force](force.md). Precision therefore depends on resolving the [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) [angle](geometry-and-topology.md#angle), calibrating the full suspended [moment of inertia](rigid-body-dynamics.md#moment-of-inertia) and [torsion constant](classical-mechanics.md#torsion-constant), and modeling the actual source geometry. The two-near-pair model omits opposite-source attraction, rod contributions, finite-size effects, [damping](wave-equation.md#damping), and the variation of gravitational [torque](momentum.md#torque) as the rod turns. [Harvard Cavendish demonstration: sensitivity, settling, and separation-dependent measurement](https://sciencedemonstrations.fas.harvard.edu/presentations/cavendish-experiment)

## ↑ Ancestors (4)

1. [Classical mechanics](classical-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (31)

- [Cavendish experiment](#cavendish-experiment)
- [Circular-binary quadrupole radiation](gravitational-wave.md#circular-binary-quadrupole-radiation)
- [Geodesic deviation](riemann-curvature-tensor.md#geodesic-deviation)
- [Geostationary orbit](celestial-mechanics.md#geostationary-orbit)
- [Gravitational constant](#gravitational-constant)
- [Gravitational-electrostatic balance of equal charged spheres](#gravitational-electrostatic-balance-of-equal-charged-spheres)
- [Gravitational mass](classical-mechanics.md#gravitational-mass)
- [Inverse-square potential](energy.md#inverse-square-potential)
- [Jerk (kinematics)](classical-mechanics.md#jerk-kinematics)
- [Kepler's laws of planetary motion](mathematical-physics.md#kepler-s-laws-of-planetary-motion)
- [Low circular-orbit period measures mean density](celestial-mechanics.md#low-circular-orbit-period-measures-mean-density)
- [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4.md#9e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-59.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-49.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-56.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4.md#3b/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-321.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-322.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-322.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-322.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-316.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-316.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1.md#14/a/i/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#section-e/e15/a/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1.md#e14/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018.md#section-b/7/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018.md#section-e/14/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018.md#section-e/15/d/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#section-b/b5/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-a/5/solution)
