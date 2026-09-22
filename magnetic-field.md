# Magnetic field

↑ **Parent:** [Electromagnetism](electromagnetism.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetic_field)

A [magnetic field](magnetic-field.md) is a [vector field](multivariable-calculus.md#vector-field) $\mathbf B(\mathbf r,t)$ whose local value determines the magnetic part of the [Lorentz force](relativistic-electromagnetism.md#lorentz-force) on a body with [electric charge](electric-charge.md) $q$ and [velocity](classical-mechanics.md#velocity) $\mathbf v$. In [SI](physics.md#international-system-of-units) units,

$$
\mathbf F_B=q\mathbf v\times\mathbf B,\qquad
|\mathbf F_B|=|q|vB\sin\alpha,
$$

where $v$ is the [speed](classical-mechanics.md#speed), $B=|\mathbf B|$, and $\alpha$ is the [angle](geometry-and-topology.md#angle) between the [velocity](classical-mechanics.md#velocity) and the [magnetic field](magnetic-field.md). The [cross product](vector-space.md#cross-product) makes a nonzero magnetic [force](force.md) perpendicular to both the [velocity](classical-mechanics.md#velocity) and the [magnetic field](magnetic-field.md). The [right-hand rule](electromagnetism.md#right-hand-rule) gives its direction for positive [electric charge](electric-charge.md); negative [electric charge](electric-charge.md) reverses it. [OpenStax, magnetic fields and forces](https://openstax.org/books/university-physics-volume-2/pages/11-2-magnetic-fields-and-lines).

The [SI](physics.md#international-system-of-units) unit of [magnetic field](magnetic-field.md) is the [tesla](#tesla-unit):

$$
1\,\mathrm T=\frac{1\,\mathrm N}{(1\,\mathrm C)(1\,\mathrm{m\,s^{-1}})}.
$$

For a stipulated example in [SI](physics.md#international-system-of-units) units, take [electric charge](electric-charge.md) $q=2\,\mathrm C$, [velocity](classical-mechanics.md#velocity) $\mathbf v=(3,0,0)\,\mathrm{m\,s^{-1}}$, and [magnetic field](magnetic-field.md) $\mathbf B=(0,0,4)\,\mathrm T$. The [cross product](vector-space.md#cross-product) gives magnetic [force](force.md) $\mathbf F_B=(0,-24,0)\,\mathrm N$. With the same [speed](classical-mechanics.md#speed) directed along $+z$, the magnetic [force](force.md) is zero: motion parallel to a [magnetic field](magnetic-field.md) produces no magnetic [acceleration](classical-mechanics.md#acceleration).

[Magnetic field lines](#magnetic-field-line) visualize the direction of a [magnetic field](magnetic-field.md) by being tangent to it at each point. They are not generally the path of a body with [electric charge](electric-charge.md): in a uniform [magnetic field](magnetic-field.md) along $+z$, the [magnetic field lines](#magnetic-field-line) are straight while transverse [velocity](classical-mechanics.md#velocity) produces [circular motion](classical-mechanics.md#circular-motion), and adding parallel [velocity](classical-mechanics.md#velocity) produces [helical motion in a uniform magnetic field](electromagnetism.md#helical-motion-in-a-uniform-magnetic-field). The worked [Lorentz force](relativistic-electromagnetism.md#lorentz-force) example below illustrates this distinction.

A [magnetic field](magnetic-field.md) need not be static. [Magnetostatics](electromagnetism.md#magnetostatics) is the restricted case with no dependence on [time](classical-mechanics.md#time-in-physics); an [electromagnetic wave](electromagnetic-wave.md) has changing [electric field](electric-field.md) and [magnetic field](magnetic-field.md) even in vacuum. A changing [magnetic field](magnetic-field.md) is coupled to the [electric field](electric-field.md) through [Faraday's law of induction](maxwell-equations.md#faraday-s-law-of-induction). [Feynman lectures, II.20: electromagnetic waves in free space](https://www.feynmanlectures.caltech.edu/II_20.html). The useful separation is between local bending, described by the [Lorentz force](relativistic-electromagnetism.md#lorentz-force), and the amount of [magnetic field](magnetic-field.md) crossing a [surface](topological-surface.md), described by [magnetic flux](#magnetic-flux).

**Table of contents**

- [Magnetic energy density](#magnetic-energy-density)
- [Magnetic field strength](#magnetic-field-strength)
- [Magnetic field gradient](#magnetic-field-gradient)
- [Tesla (unit)](#tesla-unit)
- [Solenoid](#solenoid)
  - [Relativistic solenoid magnetic lens](#relativistic-solenoid-magnetic-lens)
  - [Helical solenoid trajectory with zero incident angular momentum](#helical-solenoid-trajectory-with-zero-incident-angular-momentum)
  - [Solenoid fringe field from an axisymmetric vector potential](#solenoid-fringe-field-from-an-axisymmetric-vector-potential)
  - [Solenoid turn density](#solenoid-turn-density)
  - [Long-solenoid approximation](#long-solenoid-approximation)
  - [On-axis magnetic field of a finite solenoid](#on-axis-magnetic-field-of-a-finite-solenoid)
  - [Solenoid inductance](#solenoid-inductance)
    - [Stored energy of a solenoid](#stored-energy-of-a-solenoid)
- [Compass](#compass)
- [Solenoidal magnetic-field constraint](#solenoidal-magnetic-field-constraint)
- [Magnetic field line](#magnetic-field-line)
  - [Flux tube](#flux-tube)
    - [Flux-tube area](#flux-tube-area)
  - [Magnetic-field-line equation](#magnetic-field-line-equation)
  - [Magnetic dipole field](#magnetic-dipole-field)
    - [Force between distant coaxial current loops](#force-between-distant-coaxial-current-loops)
    - [Magnetic dipole inclination versus latitude](#magnetic-dipole-inclination-versus-latitude)
    - [Dipole magnetic-field line](#dipole-magnetic-field-line)
      - [Dipolar flux-tube area](#dipolar-flux-tube-area)
- [Magnetostatic equilibrium](#magnetostatic-equilibrium)
  - [Spherical magnetostatic pressure balance](#spherical-magnetostatic-pressure-balance)
    - [Confined linear-pressure spherical magnetic equilibrium](#confined-linear-pressure-spherical-magnetic-equilibrium)
  - [Magnetized isothermal atmosphere](#magnetized-isothermal-atmosphere)
  - [Cylindrical magnetostatic equilibrium](#cylindrical-magnetostatic-equilibrium)
    - [Z-pinch](#z-pinch)
    - [Cylindrical magnetostatic pressure balance](#cylindrical-magnetostatic-pressure-balance)
      - [Flux-tube axial field virial identity](#flux-tube-axial-field-virial-identity)
        - [Uniform-twist central axial field bound](#uniform-twist-central-axial-field-bound)
      - [Power-law pressure-supported axial current](#power-law-pressure-supported-axial-current)
      - [Magnetic pressure support with vanishing axial field](#magnetic-pressure-support-with-vanishing-axial-field)
- [Motional electric field](#motional-electric-field)
- [London equations](#london-equations)
  - [London screening](#london-screening)
  - [London penetration depth](#london-penetration-depth)
    - [Plasma-frequency form of London penetration depth](#plasma-frequency-form-of-london-penetration-depth)
    - [Superconducting carrier density from London screening](#superconducting-carrier-density-from-london-screening)
  - [Meissner effect](#meissner-effect)
    - [Superconducting plane image dipole](#superconducting-plane-image-dipole)
      - [Dipole levitation force above a superconducting plane](#dipole-levitation-force-above-a-superconducting-plane)
    - [Meissner state](#meissner-state)
      - [Planar London screening](#planar-london-screening)
        - [Meissner screening current](#meissner-screening-current)
      - [Finite-thickness Meissner screening](#finite-thickness-meissner-screening)
    - [Meissner effect and flux history](#meissner-effect-and-flux-history)
    - [Meissner effect discovery](#meissner-effect-discovery)
    - [Limits of Meissner screening](#limits-of-meissner-screening)
- [Magnetic flux](#magnetic-flux)
  - [Weber (unit)](#weber-unit)
- [Electromagnet](#electromagnet)

## Magnetic energy density

↑ **Parent:** [Magnetic field](magnetic-field.md)

In vacuum or an approximately nonmagnetizable plasma, the field [energy](energy.md) per volume is $B^2/(2\mu_0)$. [magnetic pressure](magnetohydrodynamics.md#magnetic-pressure) has the same scale, but a [magnetic field](magnetic-field.md) also exerts directional tension, so its stress is not universally an isotropic pressure. Material magnetization can require a different constitutive treatment.

## Magnetic field strength

↑ **Parent:** [Magnetic field](magnetic-field.md)

In macroscopic [electromagnetism](electromagnetism.md), [magnetic field strength](#magnetic-field-strength) is $\mathbf H=\mathbf B/\mu_0-\mathbf M$, where $\mathbf B$ is [magnetic flux density](magnetic-field.md) and $\mathbf M$ is [magnetization](electromagnetism.md#magnetization). In [SI](physics.md#international-system-of-units) units $\mathbf H$ is measured in $\mathrm{A\,m^{-1}}$, while $\mathbf B$ is measured in [tesla](#tesla-unit) units. In a linear isotropic medium $\mathbf B=\mu\mathbf H$, where $\mu$ is [magnetic permeability](maxwell-equations.md#permeability-electromagnetism). The macroscopic [Ampère-Maxwell equation](maxwell-equations.md#ampere-s-circuital-law) writes its [curl](multivariable-calculus.md#curl) in terms of free current and [displacement current](maxwell-equations.md#displacement-current). The electromagnetic [Poynting vector](electromagnetic-wave.md#poynting-vector) is $\mathbf E\times\mathbf H$ in this convention.

## Magnetic field gradient

↑ **Parent:** [Magnetic field](magnetic-field.md)

## Tesla (unit)

↑ **Parent:** [Magnetic field](magnetic-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tesla_(unit))

The [tesla](#tesla-unit) is the [SI](physics.md#international-system-of-units) unit of [magnetic field](magnetic-field.md). From the magnetic [Lorentz force](relativistic-electromagnetism.md#lorentz-force), $1\,\mathrm T=1\,\mathrm{N\,s\,C^{-1}\,m^{-1}}$. [OpenStax, magnetic-field units](https://openstax.org/books/university-physics-volume-2/pages/11-2-magnetic-fields-and-lines).

## Solenoid

↑ **Parent:** [Magnetic field](magnetic-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Solenoid)

A [solenoid](#solenoid) is a coil of [electrical conductor](electric-charge.md#electrical-conductor), usually wire wound into a [helix](topology.md#helix) around a [circular cylinder](differential-geometry.md#circular-cylinder). The same [electric current](electric-charge.md#electric-current) $I$ flows through its successive turns. Each turn contributes a [magnetic field](magnetic-field.md); the [superposition principle](vector-space.md#superposition-principle) makes their axial contributions reinforce inside the coil. Curl the fingers of your right hand in the direction of the [electric current](electric-charge.md#electric-current) around the turns: the thumb gives the interior [magnetic field](magnetic-field.md) direction by the [right-hand rule](electromagnetism.md#right-hand-rule). Throughout this branch, $N$ is the total number of turns, $\ell$ is the coil [length](physics.md#length), and $n=N/\ell$ is the [solenoid turn density](#solenoid-turn-density). [Feynman, Leighton and Sands, The Feynman Lectures on Physics, II.13–5: the field of a long coil](https://www.feynmanlectures.caltech.edu/II_13.html#Ch13-S5).

The attraction of a long [solenoid](#solenoid) is a controllable, nearly uniform [magnetic field](magnetic-field.md) over an interior working region: change the [electric current](electric-charge.md#electric-current) to tune its strength, or reverse the [electric current](electric-charge.md#electric-current) to reverse its direction. This makes it a useful setting for studying the [Lorentz force](relativistic-electromagnetism.md#lorentz-force), measuring [magnetic flux](#magnetic-flux), and constructing an [inductor](electromagnetism.md#inductor). Its geometry turns the many contributions from individual turns into the simple [long-solenoid approximation](#long-solenoid-approximation). A real finite coil has end fields and leakage; its exterior [magnetic field](magnetic-field.md) is not zero. The [on-axis magnetic field of a finite solenoid](#on-axis-magnetic-field-of-a-finite-solenoid) below quantifies that difference.

Historically, the coil helped connect [magnetic fields](magnetic-field.md) to [electric currents](electric-charge.md#electric-current). In his memoir on the mathematical theory of electrodynamic phenomena, Ampère modeled the interactions of magnets using the ends of solenoids in place of microscopic magnetic constituents. This was a route toward explaining magnetism by [electric currents](electric-charge.md#electric-current), rather than a modern microscopic account of [magnetization](electromagnetism.md#magnetization). [Ampère, Mémoire sur la théorie mathématique des phénomènes électro-dynamiques, concluding discussion on p. 289](https://www.e-rara.ch/zut/download/pdf/1038813). The historical setting is documented by the [Ampère archives, investigations of current interactions in 1820–1826](https://ampere-archives.fr/histoire-electricite/parcours-historique/lois-courants/ampere-loi).

### Relativistic solenoid magnetic lens

↑ **Parent:** [Solenoid](#solenoid)

For a near-axis beam of equal incoming speed $v$ through a uniform solenoid of length $l$, define $\omega=|qB|/(2\gamma m)$. Neglecting the small axial-speed changes, the internal radius is $\rho=\rho_0\cos(\omega z/v)$. The exit fringe removes the azimuthal velocity for zero incident canonical angular momentum. The field-free radial trajectory then reaches the axis a distance

$$
f=\frac v\omega\cot\left(\frac{\omega l}v\right)
$$

beyond the exit, when $0<\omega l/v<\pi/2$. In the weak-lens limit, $f\simeq4(\gamma mv)^2/(q^2B^2l)$. Without the paraxial approximation, the radius-dependent axial speed produces aberration; the ideal common focus is then only approximate.

### Helical solenoid trajectory with zero incident angular momentum

↑ **Parent:** [Solenoid](#solenoid)

Let a particle enter a uniform solenoid at transverse position $u_0=x_0+iy_0$ with zero radial velocity after an ideal fringe. Define signed $\Omega=qB/(2\gamma m)$ and initial field-free speed $v$. Its [Lorentz force](relativistic-electromagnetism.md#lorentz-force) trajectory inside is

$$
u(t)=u_0\cos(\Omega t)e^{-i\Omega t}=\frac{u_0}{2}(1+e^{-2i\Omega t}),\qquad
z(t)=z_0+wt,\qquad w^2=v^2-\Omega^2|u_0|^2.
$$

The transverse motion is a circle about the guiding centre $u_0/2$ at cyclotron angular frequency $2|\Omega|$. Cylindrical radius is $|u_0\cos\Omega t|$; its apparent azimuthal jumps when the orbit crosses the axis are coordinate singularities. Forward entry requires $v>|\Omega u_0|$ in this ideal model.

### Solenoid fringe field from an axisymmetric vector potential

↑ **Parent:** [Solenoid](#solenoid)

Near the axis of a [solenoid](#solenoid), the [magnetic vector potential](electromagnetism.md#magnetic-vector-potential) $A_\theta=\rho B(z)/2$ gives

$$
B_z=B(z),\qquad B_\rho=-\frac\rho2 B'(z),\qquad B_\theta=0.
$$

The radial fringe component enforces the [solenoidal magnetic-field constraint](#solenoidal-magnetic-field-constraint). A sharp axial step in $B$ must retain this fringe as a distributional field; a purely axial field that jumps to zero violates [Gauss's law for magnetism](maxwell-equations.md#gauss-s-law-for-magnetism). The hard-edge model is a convenient limit for near-axis trajectories, not a literal monopole sheet.

### Solenoid turn density

↑ **Parent:** [Solenoid](#solenoid)

The [solenoid turn density](#solenoid-turn-density) $n$ counts turns per unit axial length in a uniformly wound [solenoid](#solenoid). The total turn count $N$ is dimensionless, whereas $n$ has units $\mathrm{m^{-1}}$. A $1000$-turn coil of length $0.50\,\mathrm m$ has $n=2000\,\mathrm{m^{-1}}$; an axial interval of length $s=0.010\,\mathrm m$ then contains $ns=20$ turns. The effective circumferential [surface current density](electric-charge.md#surface-current-density) in the closely spaced circular-turn model is $K=nI$, with units $\mathrm{A/m}$. [MIT 8.02 course notes, §9.4, equations 9.4.3–9.4.4: turns per length and surface current](https://web.mit.edu/8.02t/www/test/materials/StudyGuide/guide09_revised.pdf).

For a single-layer [helix](topology.md#helix), the axial advance per turn is approximately $1/n$. The circular-turn model neglects this advance and the associated axial component of [electric current](electric-charge.md#electric-current), as well as the detailed [magnetic field](magnetic-field.md) close to individual wires. The number of turns around the whole coil is always $N=n\ell$ here; it must not be substituted for $n$ in $B=\mu_0nI$.

### Long-solenoid approximation

↑ **Parent:** [Solenoid](#solenoid)

In [magnetostatics](electromagnetism.md#magnetostatics), an ideal infinitely long [solenoid](#solenoid) is a cylindrical sheet of circumferential [surface current density](electric-charge.md#surface-current-density) $K=nI$. It has negligible winding advance, no magnetic core, and no imposed external [magnetic field](magnetic-field.md). Choose positive [electric current](electric-charge.md#electric-current) to produce [magnetic field](magnetic-field.md) along $+z$. In this ideal model the interior [magnetic field](magnetic-field.md) is uniform and axial, $B=\mu_0nI$, and the exterior [magnetic field](magnetic-field.md) is zero; $\mu_0$ is the [vacuum permeability](maxwell-equations.md#vacuum-permeability). For a finite, closely wound air-core coil, the same result is an approximation well inside the coil, several radii from either end. Air is treated as having the [magnetic permeability](maxwell-equations.md#permeability-electromagnetism) of vacuum. [Feynman lectures, II.13–5: long-solenoid field and the return field near the ends](https://www.feynmanlectures.caltech.edu/II_13.html#Ch13-S5).

For a short proof, the translational and rotational [symmetries](physics.md#symmetry-physics) of the ideal cylindrical [current sheet](electric-charge.md#current-sheet), together with the [Biot-Savart law](electromagnetism.md#biot-savart-law), give an axial [magnetic field](magnetic-field.md). [Ampère's law](maxwell-equations.md#ampere-s-circuital-law) on rectangles wholly outside makes that axial exterior value independent of radius; the condition of no imposed [magnetic field](magnetic-field.md) makes it zero at infinity and hence everywhere outside. Rectangles wholly inside similarly show that the interior value is independent of radius. Now choose an [Amperian loop](maxwell-equations.md#amperian-loop) with axial length $s$, one long side inside and the other outside. The transverse sides are perpendicular to the [magnetic field](magnetic-field.md), so their contributions to the [line integral](multivariable-calculus.md#line-integral) vanish. The loop crosses $ns$ turns of the winding, giving

$$
\oint_\Gamma\mathbf B\cdot d\mathbf l
=Bs=\mu_0(ns)I,
\qquad B=\mu_0nI.
$$

Here $s$ is the integration-path length, not the whole coil [length](physics.md#length) $\ell$. An [Amperian loop](maxwell-equations.md#amperian-loop) surrounding both sides of the winding encloses equal and opposite [electric currents](electric-charge.md#electric-current); zero net circulation alone would not prove zero [magnetic field](magnetic-field.md) at every exterior point.

<a id="image-ampere-s-law-for-the-ideal-long-solenoid-approximation"></a>
![](solenoid-ampere-loop.png)

**[Figure 1](#image-ampere-s-law-for-the-ideal-long-solenoid-approximation). Ampère's law for the ideal long-solenoid approximation**. Axial cross-section of an infinite ideal winding: paired dots and crosses show [electric current](electric-charge.md#electric-current) out of and into the page. The indicated [right-hand rule](electromagnetism.md#right-hand-rule) produces interior [magnetic field](magnetic-field.md) along $+z$. The counterclockwise [Amperian loop](maxwell-equations.md#amperian-loop) crosses only the upper row, with $ns=6$ positive crossings; its interior side runs along $+z$, and its exterior return lies where the ideal [magnetic field](magnetic-field.md) is zero.

For the $1000$-turn, $0.50\,\mathrm m$ coil with [electric current](electric-charge.md#electric-current) $I=0.50\,\mathrm A$, the [long-solenoid approximation](#long-solenoid-approximation) gives

$$
B\approx(1.256637\times10^{-6})(2000)(0.50)\,\mathrm T
=1.256637\times10^{-3}\,\mathrm T
\approx1.257\,\mathrm{mT}.
$$

This illustrative calculation uses [vacuum permeability](maxwell-equations.md#vacuum-permeability) $\mu_0\approx1.256637\times10^{-6}\,\mathrm{H/m}$, a rounded value, not an exact constant. Since the 2019 redefinition of [SI](physics.md#international-system-of-units), [vacuum permeability](maxwell-equations.md#vacuum-permeability) is determined experimentally.[§2.3.1: the ampere and vacuum permeability](physics-bibliography.md#the-international-system-of-units-si-ninth-edition-si-brochure) Doubling $I$ doubles the ideal [magnetic field](magnetic-field.md); doubling $N$ at fixed $\ell$ does the same. Increasing $\ell$ while keeping $N$ fixed decreases $n$ and hence the ideal [magnetic field](magnetic-field.md).

### On-axis magnetic field of a finite solenoid

↑ **Parent:** [Solenoid](#solenoid)

Model a finite [solenoid](#solenoid) as a continuum of coaxial turns shaped as [circles](topology.md#circle) of [radius](topology.md#radius) $a>0$, uniformly distributed over length $\ell$ with [solenoid turn density](#solenoid-turn-density) $n=N/\ell$. Put its centre at $z=0$, so its ends are $z=\pm\ell/2$. With the same [electric current](electric-charge.md#electric-current) orientation as in the [long-solenoid approximation](#long-solenoid-approximation), its axial [magnetic field](magnetic-field.md) is

$$
B_z(z)=\frac{\mu_0nI}{2}
\left[
\frac{z+\ell/2}{\sqrt{a^2+(z+\ell/2)^2}}
-\frac{z-\ell/2}{\sqrt{a^2+(z-\ell/2)^2}}
\right].
$$

This formula applies only on the axis, where [symmetry](physics.md#symmetry-physics) cancels the transverse [magnetic field](magnetic-field.md). It does not describe points off the axis. It is exact for the continuum circular-turn model, which neglects winding thickness, discrete wire spacing, and helical advance. [MIT 8.02 course notes, §9.4, equations 9.4.5–9.4.6: the finite-solenoid axial field](https://web.mit.edu/8.02t/www/test/materials/StudyGuide/guide09_revised.pdf).

The derivation is an especially direct use of the [superposition principle](vector-space.md#superposition-principle). The [on-axis magnetic field of a circular current loop](electromagnetism.md#on-axis-magnetic-field-of-a-circular-current-loop) at source position $z'$ is $\mu_0Ia^2/[2(a^2+(z-z')^2)^{3/2}]$. There are $n\,dz'$ turns in an axial slice, so

$$
B_z(z)=\frac{\mu_0nIa^2}{2}
\int_{-\ell/2}^{\ell/2}
\frac{dz'}{[a^2+(z-z')^2]^{3/2}}.
$$

Substitute $u=z-z'$ and use the [antiderivative](integral.md#antiderivative) $u/[a^2\sqrt{a^2+u^2}]$ to obtain the displayed expression. If the centre is instead at $z=z_0$, replace every $z$ in that expression by $z-z_0$.

At the centre and at either end, respectively,

$$
\frac{B_z(0)}{\mu_0nI}=\frac{\ell}{\sqrt{\ell^2+4a^2}},
\qquad
\frac{B_z(\ell/2)}{\mu_0nI}
=\frac{\ell}{2\sqrt{\ell^2+a^2}}.
$$

For aspect ratios $\ell/a=2,6,20$, the centre ratios are approximately $0.7071,0.9487,0.9950$. The end ratio tends to $1/2$ as $\ell/a$ becomes large, even though the centre ratio tends to $1$. Thus a long coil can have an excellent central [magnetic field](magnetic-field.md) while the ends still differ strongly from that value. Convergence to the [long-solenoid approximation](#long-solenoid-approximation) is not uniform across the end region.

<a id="image-finite-solenoid-axial-magnetic-fields-compared-with-the-ideal-interior-value"></a>
![](solenoid-axial-field-profile.png)

**[Figure 2](#image-finite-solenoid-axial-magnetic-fields-compared-with-the-ideal-interior-value). Finite solenoid axial magnetic fields compared with the ideal interior value**. Original profiles for $\ell/a=2,6,20$ on the axis, normalized by $\mu_0nI$. The dashed step is the approximation that assigns the ideal interior value within the coil and zero outside; an infinite [solenoid](#solenoid) itself has no ends. The finite profiles stay smooth through the end planes and remain nonzero beyond them. These curves describe no off-axis points.

For a concrete geometry, give the earlier coil [radius](topology.md#radius) $a=0.025\,\mathrm m$, so $\ell/a=20$. Its central [magnetic field](magnetic-field.md) is approximately $1.2504\,\mathrm{mT}$, its end value is $0.6275\,\mathrm{mT}$, and at $z=\ell$ its axial [magnetic field](magnetic-field.md) is still $0.00277\,\mathrm{mT}$. The last point is outside the coil: finite length does not permit the zero-exterior conclusion of the infinite model. Off the axis, the [magnetic field lines](#magnetic-field-line) bend around to form the return field. A central axial value alone also does not determine the total [magnetic flux](#magnetic-flux) through every turn of a short coil.

### Solenoid inductance

↑ **Parent:** [Solenoid](#solenoid)

For a long vacuum-core or air-core [solenoid](#solenoid) with fixed geometry and linear magnetic response, neglecting end effects gives [self-inductance](electromagnetism.md#self-inductance)

$$
L\approx\frac{\mu_0N^2A}{\ell}
=\mu_0n^2A\ell,
\qquad A=\pi a^2.
$$

Here $N$ is the total number of turns, $n=N/\ell$ is the [solenoid turn density](#solenoid-turn-density), and $A$ is the interior cross-sectional [area](differential-geometry.md#surface-area). The reason for the square of $N$ is physical: more turns produce more [magnetic field](magnetic-field.md), and more turns link the resulting [magnetic flux](#magnetic-flux). Approximately equal [magnetic flux](#magnetic-flux) $\Phi\approx BA$ through each turn gives [magnetic flux linkage](electromagnetism.md#magnetic-flux-linkage) $\Lambda\approx N\Phi\approx\mu_0N^2AI/\ell$; division by the [electric current](electric-charge.md#electric-current) yields $L$. [MIT 8.02 course notes, Example 11.2: self-inductance of a solenoid](https://s3.amazonaws.com/edx-textbooks/mit_802_textbook/Chapter11.pdf).

For the same $N=1000$, $\ell=0.50\,\mathrm m$, and $a=0.025\,\mathrm m$, the [area](differential-geometry.md#surface-area) is $A=\pi(0.025)^2\,\mathrm{m^2}\approx1.9635\times10^{-3}\,\mathrm{m^2}$. The long-coil estimate is

$$
L\approx\frac{(1.256637\times10^{-6})(1000)^2\pi(0.025)^2}{0.50}\,\mathrm H
\approx4.9348\,\mathrm{mH}.
$$

At $I=0.50\,\mathrm A$, each turn links approximately $2.4674\times10^{-6}\,\mathrm{Wb}$ and the total [magnetic flux linkage](electromagnetism.md#magnetic-flux-linkage) is approximately $2.4674\times10^{-3}\,\mathrm{Wb}$. Their ratio to $I$ is the stated [self-inductance](electromagnetism.md#self-inductance). A real finite coil need not give precisely these values: the axial centre correction above is not by itself a correction formula for [inductance](electromagnetism.md#inductance), which depends on [magnetic flux](#magnetic-flux) across all the turns.

At fixed $A$ and $\ell$, doubling $N$ quadruples $L$. At fixed [solenoid turn density](#solenoid-turn-density) $n$ and [area](differential-geometry.md#surface-area) $A$, doubling $\ell$ doubles both $N$ and $L$. These are different changes to the geometry, so there is no contradiction between $L\propto1/\ell$ at fixed $N$ and $L\propto\ell$ at fixed $n$. A magnetic core requires its own [magnetic permeability](maxwell-equations.md#permeability-electromagnetism) model; nonlinear [magnetization](electromagnetism.md#magnetization) can make a constant-$L$ description inadequate.

#### Stored energy of a solenoid

↑ **Parent:** [Solenoid inductance](#solenoid-inductance)

The [magnetic energy](electromagnetic-wave.md#magnetic-energy) stored in a linear [solenoid](#solenoid) of constant [self-inductance](electromagnetism.md#self-inductance) $L$ is

$$
U=\frac12LI^2,
\qquad
U\approx\frac{B^2}{2\mu_0}A\ell
$$

in the [long-solenoid approximation](#long-solenoid-approximation). The first formula is an [inductor](electromagnetism.md#inductor) relation; the second identifies its storage with [magnetic energy](electromagnetic-wave.md#magnetic-energy) in the interior [magnetic field](magnetic-field.md), under the vacuum-core approximation. This agreement joins the [electrical circuit](electrical-circuit.md) description to the spatial [magnetic field](magnetic-field.md) description. The expression $B^2/(2\mu_0)$ is the vacuum magnetic [energy density](statistical-physics.md#energy-density). [MIT 8.02 course notes, §11.3: magnetic energy and its density](https://s3.amazonaws.com/edx-textbooks/mit_802_textbook/Chapter11.pdf).

A short derivation starts from the terminal [electric potential difference](electric-field.md#electric-potential-difference) $v_L=L\,dI/dt$, with positive [electric current](electric-charge.md#electric-current) entering the terminal at higher potential. The absorbed [power](energy.md#power) is $v_LI$, and integrating from zero [electric current](electric-charge.md#electric-current) gives

$$
U=\int_0^I Li\,di=\frac12LI^2.
$$

The result describes recoverable storage in the [inductor](electromagnetism.md#inductor); [Joule heating](electric-charge.md#joule-heating) in the wire is a separate expenditure of [energy](energy.md). [Feynman lectures, II.17–8: inductance and magnetic energy](https://www.feynmanlectures.caltech.edu/II_17.html#Ch17-S8).

For the long-coil example, $L\approx4.9348\,\mathrm{mH}$ and $I=0.50\,\mathrm A$ give $U\approx6.1685\times10^{-4}\,\mathrm J=0.61685\,\mathrm{mJ}$. Substituting the ideal $B\approx1.256637\,\mathrm{mT}$ and volume $A\ell\approx9.8175\times10^{-4}\,\mathrm{m^3}$ into $B^2A\ell/(2\mu_0)$ gives the same value. Doubling [electric current](electric-charge.md#electric-current) quadruples stored [magnetic energy](electromagnetic-wave.md#magnetic-energy). In a real coil, reducing [electric current](electric-charge.md#electric-current) can return this [energy](energy.md) to an [electrical circuit](electrical-circuit.md), or release it as [Joule heating](electric-charge.md#joule-heating) in a closed [RL circuit](electrical-circuit.md#rl-circuit).

## Compass

↑ **Parent:** [Magnetic field](magnetic-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compass)

A [magnetic compass](#compass) uses the orientation of a magnetic needle to indicate the direction of a [magnetic field](magnetic-field.md).

## Solenoidal magnetic-field constraint

↑ **Parent:** [Magnetic field](magnetic-field.md)

The [magnetic field](magnetic-field.md) has zero divergence. The [ideal magnetohydrodynamic induction equation](ideal-magnetohydrodynamics.md#ideal-magnetohydrodynamic-induction-equation) preserves this constraint from initial data, since the divergence of its curl is zero.

## Magnetic field line

↑ **Parent:** [Magnetic field](magnetic-field.md)

A magnetic field line is an integral curve tangent to the [magnetic field](magnetic-field.md). In coordinates $x^i$, it obeys $dx^i/B^i=dx^j/B^j$ wherever the relevant components are nonzero.

### Flux tube

↑ **Parent:** [Magnetic field line](#magnetic-field-line)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flux_tube)

A flux tube is a bundle of [magnetic field lines](#magnetic-field-line) bounded by a surface everywhere tangent to the [magnetic field](magnetic-field.md). [Gauss's law for magnetism](maxwell-equations.md#gauss-s-law-for-magnetism) makes the [magnetic flux](#magnetic-flux) through any transverse cross-section constant along the tube. For a narrow tube with nearly uniform field magnitude $B$ and transverse area $A$, this gives $BA=\mathrm{constant}$.

#### Flux-tube area

↑ **Parent:** [Flux tube](#flux-tube)

The cross-sectional area of a narrow [flux tube](#flux-tube), measured normal to its [magnetic field](magnetic-field.md). Constancy of the [magnetic flux](#magnetic-flux) gives $A|\mathbf B|=\mathrm{constant}$ along the tube. This area controls the mass transport when flow follows the field.

### Magnetic-field-line equation

↑ **Parent:** [Magnetic field line](#magnetic-field-line)

The magnetic-field-line equation states that the tangent to a field line is parallel to $\mathbf B$. In spherical coordinates for an axisymmetric poloidal field, it can be written $dr/(r\,d\theta)=B_r/B_\theta$.

### Magnetic dipole field

↑ **Parent:** [Magnetic field line](#magnetic-field-line)

Outside a localized magnetic dipole $\boldsymbol\mu$, the vacuum field in Gaussian conventions is

$$
\mathbf B(\mathbf r)=\frac{3(\boldsymbol\mu\mathbin\cdot\mathbf r)\mathbf r}{r^5}-\frac{\boldsymbol\mu}{r^3}.
$$

For a dipole along the polar axis, $B_r=2\mu\cos\theta/r^3$ and $B_\theta=\mu\sin\theta/r^3$.

#### Force between distant coaxial current loops

↑ **Parent:** [Magnetic dipole field](#magnetic-dipole-field)

For coaxial circular loops with radii $a_1,a_2\ll d$, the first loop's [on-axis magnetic field of a circular current loop](electromagnetism.md#on-axis-magnetic-field-of-a-circular-current-loop) has far value $B_0\simeq\mu_0I_1a_1^2/(2d^3)$. Its [near-axis radial magnetic field](maxwell-equations.md#near-axis-radial-magnetic-field) at the second loop is $B_\rho\simeq3\mu_0I_1a_1^2a_2/(4d^4)$. Integrating the axial [Lorentz force](relativistic-electromagnetism.md#lorentz-force) from $I_2a_2\,d\phi\,\widehat{\boldsymbol\phi}\times B_\rho\widehat{\boldsymbol\rho}$ gives the displayed magnitude. Equal current senses attract; opposite senses repel. This is the leading dipole limit and is not an exact close-coil force law.

#### Magnetic dipole inclination versus latitude

↑ **Parent:** [Magnetic dipole field](#magnetic-dipole-field)

For a centred [magnetic dipole moment](electromagnetism.md#magnetic-dipole-moment) pointing toward geographic south, the field at northern latitude $\lambda$ has northward component $B_N=B_{\rm eq}\cos\lambda$ and downward component $B_D=2B_{\rm eq}\sin\lambda$. These follow by resolving the [magnetic dipole field](#magnetic-dipole-field) into local radial and meridional directions. The downward inclination is therefore $\tan\iota=B_D/B_N=2\tan\lambda$, while the magnitude is $B_{\rm eq}\sqrt{1+3\sin^2\lambda}$. This ideal aligned-dipole model has no eastward component and does not capture actual geographic departures of the geomagnetic field.

#### Dipole magnetic-field line

↑ **Parent:** [Magnetic dipole field](#magnetic-dipole-field)

An axisymmetric dipole field line satisfies $r=C\sin^2\theta$, where $C$ is its equatorial crossing radius. This follows by integrating $dr/(r\,d\theta)=B_r/B_\theta=2\cot\theta$.

##### Dipolar flux-tube area

↑ **Parent:** [Dipole magnetic-field line](#dipole-magnetic-field-line)

Near the polar axis of a [magnetic dipole field](#magnetic-dipole-field), $B\propto r^{-3}$. Conservation of [magnetic flux](#magnetic-flux) in a [flux tube](#flux-tube) consequently gives $A(r)\propto r^3$. A [dipole magnetic-field line](#dipole-magnetic-field-line) intersecting a sphere of radius $R_\star$ at small polar angle $\theta_\star$ obeys

$$
\theta(r)^2\simeq\theta_\star^2\frac r{R_\star},
\qquad
A(r)\simeq\pi r^2\theta(r)^2
=\pi\theta_\star^2\frac{r^3}{R_\star}.
$$

This area is for one polar tube. The approximation requires $\theta_\star^2r/R_\star\ll1$; the full [magnetic dipole field](#magnetic-dipole-field) does not remain a narrow polar tube at arbitrarily large radius.

## Magnetostatic equilibrium

↑ **Parent:** [Magnetic field](magnetic-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetostatic_equilibrium)

A magnetostatic equilibrium is a time-independent configuration in which magnetic, pressure, gravitational, and any other body-force densities balance.

### Spherical magnetostatic pressure balance

↑ **Parent:** [Magnetostatic equilibrium](#magnetostatic-equilibrium)

For an axisymmetric [magnetic field](magnetic-field.md) $\mathbf B=\psi\mathbf e_\phi/(r\sin\theta)+\nabla\times[\chi\mathbf e_\phi/(r\sin\theta)]$, the [poloidal magnetic flux function](ideal-magnetohydrodynamics.md#poloidal-magnetic-flux-function) gives $B_r=\chi_\theta/(r^2\sin\theta)$ and $B_\theta=-\chi_r/(r\sin\theta)$. Force balance implies locally $p=p(\chi)$ and $\psi=\psi(\chi)$ on regular connected flux surfaces. Direct calculation gives $(\nabla\times\mathbf B)\times\mathbf B=-(\Delta_*\chi+\psi\psi')\nabla\chi/(r^2\sin^2\theta)$, with $\Delta_*\chi=\chi_{rr}+\sin\theta\,\partial_\theta(\chi_\theta/\sin\theta)/r^2$. Equating this to $\mu_0\nabla p$ proves the displayed [magnetostatic equilibrium](#magnetostatic-equilibrium) equation, including its sign and dimensions.

#### Confined linear-pressure spherical magnetic equilibrium

↑ **Parent:** [Spherical magnetostatic pressure balance](#spherical-magnetostatic-pressure-balance)

Set $\psi=\alpha\chi$, $p=p_0+P\chi$ and $\chi=F(r)\sin^2\theta$. A regular family is $F=A[\cos(\alpha r)-\sin(\alpha r)/(\alpha r)]+cr^2$, where $P=-\alpha^2c/\mu_0$. A zero [magnetic field](magnetic-field.md) at radius a requires $F(a)=F'(a)=0$. For nonzero A this yields the displayed condition with $x=\alpha a$ and $c=-A[\cos x-\sin x/x]/a^2$. The boundary pressure is $p_0$, independent of angle. The trigonometric pair is tied by regularity and the radial differential equation; its coefficients are not independent.

### Magnetized isothermal atmosphere

↑ **Parent:** [Magnetostatic equilibrium](#magnetostatic-equilibrium)

A plane-parallel [magnetostatic equilibrium](#magnetostatic-equilibrium) with constant downward [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) $g$, horizontal [magnetic field](magnetic-field.md), constant [isothermal sound speed](compressible-flow.md#isothermal-sound-speed) $c_s$, and constant [Alfvén speed](ideal-magnetohydrodynamics.md#alfven-speed) $v_a$ has

$$
H=\frac{c_s^2+v_a^2/2}{g},\qquad \rho=\rho_0e^{-z/H},\qquad p=c_s^2\rho,\qquad B=B_0e^{-z/(2H)}.
$$

Indeed the [magnetohydrodynamic total pressure](magnetohydrodynamics.md#magnetohydrodynamic-total-pressure) is $(c_s^2+v_a^2/2)\rho$, and its vertical derivative is $-g\rho$. The [magnetic pressure](magnetohydrodynamics.md#magnetic-pressure) therefore increases the [scale height](statistical-physics.md#scale-height) above that of an unmagnetized atmosphere.

### Cylindrical magnetostatic equilibrium

↑ **Parent:** [Magnetostatic equilibrium](#magnetostatic-equilibrium)

A cylindrical magnetostatic equilibrium is an [axisymmetric vector field](multivariable-calculus.md#axisymmetric-vector-field) and [pressure](pressure.md) configuration independent of the axial coordinate. Its radial [Lorentz force density](relativistic-electromagnetism.md#lorentz-force-density) balances the [pressure gradient](fluid-mechanics.md#pressure-gradient), as expressed by [cylindrical magnetostatic pressure balance](#cylindrical-magnetostatic-pressure-balance).

#### Z-pinch

↑ **Parent:** [Cylindrical magnetostatic equilibrium](#cylindrical-magnetostatic-equilibrium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Z-pinch)

In a Z-pinch, an axial [electric current](electric-charge.md#electric-current) produces a [toroidal magnetic field](magnetohydrodynamics.md#toroidal-magnetic-field) whose inward [magnetic tension](magnetohydrodynamics.md#magnetic-tension) confines a plasma. A cylindrical [magnetostatic equilibrium](#magnetostatic-equilibrium) balances the resulting [Lorentz force density](relativistic-electromagnetism.md#lorentz-force-density) against a [pressure gradient](fluid-mechanics.md#pressure-gradient).

#### Cylindrical magnetostatic pressure balance

↑ **Parent:** [Cylindrical magnetostatic equilibrium](#cylindrical-magnetostatic-equilibrium)

For an [axisymmetric vector field](multivariable-calculus.md#axisymmetric-vector-field) independent of the axial coordinate and regular on the axis, [Gauss's law for magnetism](maxwell-equations.md#gauss-s-law-for-magnetism) gives $B_R=0$. The magnetostatic [Ampère-Maxwell equation](maxwell-equations.md#ampere-s-circuital-law) then gives $j_R=0$, $j_\phi=-cB_z'/(4\pi)$, and $j_z=c(RB_\phi)'/(4\pi R)$ in Gaussian units. Radial [magnetostatic equilibrium](#magnetostatic-equilibrium) is

$$
\frac d{dR}\left(p+\frac{B_z^2+B_\phi^2}{8\pi}\right)+\frac{B_\phi^2}{4\pi R}=0.
$$

For enclosed axial [electric current](electric-charge.md#electric-current) $I(R)$, the magnetostatic [Ampère-Maxwell equation](maxwell-equations.md#ampere-s-circuital-law) gives $B_\phi=2I/(cR)$, hence

$$
\frac d{dR}\left(p+\frac{B_z^2}{8\pi}\right)
+\frac1{2\pi c^2R^2}\frac{dI^2}{dR}=0.
$$

The first term contains [pressure](pressure.md) and axial [magnetic pressure](magnetohydrodynamics.md#magnetic-pressure); the second combines toroidal [magnetic pressure](magnetohydrodynamics.md#magnetic-pressure) with the hoop force from [magnetic tension](magnetohydrodynamics.md#magnetic-tension).

##### Flux-tube axial field virial identity

↑ **Parent:** [Cylindrical magnetostatic pressure balance](#cylindrical-magnetostatic-pressure-balance)

For a regular cylindrical [flux tube](#flux-tube) with $\mathbf B=(0,B_\phi(s),B_z(s))$, vanishing field beyond radius $s_0$, and exterior [pressure](pressure.md) $p_e$, define $\langle h\rangle=2s_0^{-2}\int_0^{s_0}sh(s)\,ds$ and $B_p^2=2\mu_0p_e$. Integrating [cylindrical magnetostatic pressure balance](#cylindrical-magnetostatic-pressure-balance) against $s^2$ gives the displayed identity. The toroidal [magnetic pressure](magnetohydrodynamics.md#magnetic-pressure) and hoop [magnetic tension](magnetohydrodynamics.md#magnetic-tension) cancel in this cross-sectional axial-field average. Nonnegative gas [pressure](pressure.md) gives $\langle B_z^2\rangle\leq B_p^2$, with strict inequality precisely when $\langle p\rangle>0$.

###### Uniform-twist central axial field bound

↑ **Parent:** [Flux-tube axial field virial identity](#flux-tube-axial-field-virial-identity)

For a [flux tube](#flux-tube) with $B_\phi=\gamma(s/s_0)B_z$, regularity at the axis and [cylindrical magnetostatic pressure balance](#cylindrical-magnetostatic-pressure-balance) give $B_z(0)^2=B_p^2-2\mu_0p(0)+\gamma^2\langle B_z^2\rangle$. The [flux-tube axial field virial identity](#flux-tube-axial-field-virial-identity) and $p\geq0$ give the bound. A twisted [toroidal magnetic field](magnetohydrodynamics.md#toroidal-magnetic-field) can support a central axial field above the untwisted [magnetic pressure](magnetohydrodynamics.md#magnetic-pressure) limit even though its cross-sectional mean obeys that limit.

##### Power-law pressure-supported axial current

↑ **Parent:** [Cylindrical magnetostatic pressure balance](#cylindrical-magnetostatic-pressure-balance)

For constant axial [magnetic field](magnetic-field.md) and $p=p_0(1+R^2/a^2)^{-k}$ with $p_0>0$ and $k>0$, [cylindrical magnetostatic pressure balance](#cylindrical-magnetostatic-pressure-balance) gives, with $x=R^2/a^2$,

$$
I^2(R)=2\pi c^2p_0a^2
\begin{cases}
\displaystyle\frac{1-(1+kx)(1+x)^{-k}}{k-1},&k\ne1,\\
\log(1+x)+(1+x)^{-1}-1,&k=1.
\end{cases}
$$

The nontrivial [electric current](electric-charge.md#electric-current) is finite at infinity exactly when $k>1$, in which case $I^2(\infty)=2\pi c^2p_0a^2/(k-1)$. Either sign of $I$ is possible because the [pressure](pressure.md) balance fixes its square.

##### Magnetic pressure support with vanishing axial field

↑ **Parent:** [Cylindrical magnetostatic pressure balance](#cylindrical-magnetostatic-pressure-balance)

With no axial [electric current](electric-charge.md#electric-current), [cylindrical magnetostatic pressure balance](#cylindrical-magnetostatic-pressure-balance) reduces to constant $p+B_z^2/(8\pi)$. For $p=p_0e^{-R^2/a^2}$ and $B_z(0)=0$, its radial solutions are

$$
B_z=\sigma\sqrt{8\pi p_0}\sqrt{1-e^{-R^2/a^2}},
\qquad
j_\phi=-\sigma\frac{c\sqrt{8\pi p_0}}{4\pi a^2}
\frac{R e^{-R^2/a^2}}{\sqrt{1-e^{-R^2/a^2}}},
\qquad \sigma\in\{-1,1\}.
$$

As $R\downarrow0$, $B_z\sim\sigma\sqrt{8\pi p_0}R/a$ and $j_\phi\to-\sigma c\sqrt{8\pi p_0}/(4\pi a)$. These finite scalar limits do not give a [smooth function](analysis.md#smooth-function) of Cartesian position: $R=\sqrt{x^2+y^2}$ has a cusp at the axis, and the azimuthal unit vector has no unique limit there. Thus these data describe radial equilibrium away from the axis, but cannot satisfy smooth vector-field regularity on the axis without modifying the data.

## Motional electric field

↑ **Parent:** [Magnetic field](magnetic-field.md)

A conductor or plasma moving with nonrelativistic velocity $\mathbf u$ through a magnetic field experiences the motional electric field $\mathbf E=-\mathbf u\times\mathbf B/c$ in Gaussian units when the electric field vanishes in its rest frame.

## London equations

↑ **Parent:** [Magnetic field](magnetic-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/London_equations)

The London equations relate the superconducting [electric current](electric-charge.md#electric-current) to the [electromagnetic field](electromagnetism.md#electromagnetic-field): $\partial_t\mathbf J=\mathbf E/(\mu_0\lambda_L^2)$ and $\nabla\times\mathbf J=-\mathbf B/(\mu_0\lambda_L^2)$. In a gauge with constant condensate phase the second follows from $\mathbf J=-\mathbf A/(\mu_0\lambda_L^2)$; it implies exponential [magnetic field](magnetic-field.md) screening.

### London screening

↑ **Parent:** [London equations](#london-equations)

Combining the static [London equations](#london-equations) with the [magnetostatic Ampère law](maxwell-equations.md#magnetostatic-ampere-law) and $\nabla\cdot\mathbf B=0$ gives the displayed bulk equation for a uniform superconducting carrier density. A planar boundary gives exponentially decaying field on the [London penetration depth](#london-penetration-depth) scale; boundary geometry and vortices require their corresponding field solutions.

### London penetration depth

↑ **Parent:** [London equations](#london-equations)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/London_penetration_depth)

For uniform vortex-free [superconductivity](superconductivity.md), the [London equation](#london-equations) and stationary Maxwell equations give $\nabla^2\mathbf B=\mathbf B/\lambda_L^2$. A field tangential to a planar superconducting half-space decays as $\mathbf B(z)=\mathbf B(0)e^{-z/\lambda_L}$. A nonzero normal boundary field is incompatible with this translation-invariant decaying Meissner solution, because divergence-free magnetic flux would require that component to remain constant.

#### Plasma-frequency form of London penetration depth

↑ **Parent:** [London penetration depth](#london-penetration-depth)

For carrier [number density](statistical-physics.md#number-density) $n$, charge $q$ and effective [mass](classical-mechanics.md#mass) $m$, the [plasma frequency](physics.md#plasma-frequency) is $\omega_p^2=nq^2/(\epsilon_0m)$. Combining the second [London equation](#london-equations) with the [magnetostatic Ampère law](maxwell-equations.md#magnetostatic-ampere-law) and [Gauss's law for magnetism](maxwell-equations.md#gauss-s-law-for-magnetism) gives $\nabla^2\mathbf B=(\omega_p^2/c^2)\mathbf B$. Therefore the decaying planar solution has length $\lambda_L=c/\omega_p=\sqrt{m/(\mu_0nq^2)}$.

#### Superconducting carrier density from London screening

↑ **Parent:** [London penetration depth](#london-penetration-depth)

In a local [London equation](#london-equations) description, the measured [London penetration depth](#london-penetration-depth) satisfies $\lambda_L^2=m/(\mu_0n_se^2)$ when $n_s$ counts superconducting [electrons](physics.md#electron) and $m$ is their [effective mass](bloch-s-theorem.md#band-effective-mass). Thus screening measures $n_s/m$. If instead one counts [Cooper pairs](fermi-liquid.md#cooper-pair), use pair [mass](classical-mechanics.md#mass) $2m$ and pair [electric charge](electric-charge.md) $-2e$, giving pair density $n_s/2$ for the same screening length. Identifying this superconducting carrier density with the total conduction-electron density requires the additional assumption that the relevant carriers all participate in screening at the measurement [temperature](temperature.md).

### Meissner effect

↑ **Parent:** [London equations](#london-equations)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Meissner_effect)

The [Meissner effect](#meissner-effect) is the equilibrium expulsion of a sufficiently weak, static [magnetic field](magnetic-field.md) from the bulk of a material exhibiting [superconductivity](superconductivity.md). Expulsion includes a [magnetic field](magnetic-field.md) that was already present before cooling: zero [electrical resistance](electric-charge.md#electrical-resistance) alone does not predict this. The [Field-cooled Meissner experiment](superconductivity.md#field-cooled-meissner-experiment) tests that distinction. A finite [London penetration depth](#london-penetration-depth) means that the [magnetic field](magnetic-field.md) and screening [electric current](electric-charge.md#electric-current) occupy a surface layer, rather than disappearing at a mathematical boundary.[§2, pp. 12–13, Eqs. (64)–(74): acceleration, additional magnetic constraint and penetration length](physics-bibliography.md#lecture-notes-on-the-electrodynamics-of-metals-and-superconductors)

This makes [superconductivity](superconductivity.md) useful for shielding weak [magnetic fields](magnetic-field.md), and makes its magnetic response an independent test of the phase. The striking result is that the same screened equilibrium can be reached by two different preparation histories. The assumptions matter: [Finite-thickness Meissner screening](#finite-thickness-meissner-screening) can leave an appreciable [magnetic field](magnetic-field.md) throughout a small sample, and the [Limits of Meissner screening](#limits-of-meissner-screening) distinguish [quantum vortex](critical-phenomenon.md#quantum-vortex) penetration and retained [magnetic flux](#magnetic-flux) from this equilibrium state.

#### Superconducting plane image dipole

↑ **Parent:** [Meissner effect](#meissner-effect)

A perpendicular magnetic dipole $m\widehat z$ a height $h$ above an ideal flux-excluding plane has image $-m\widehat z$ at $-h$. The exterior field has zero normal component at the plane. Images are a mathematical construction outside the physical solution domain.

##### Dipole levitation force above a superconducting plane

↑ **Parent:** [Superconducting plane image dipole](#superconducting-plane-image-dipole)

For a small fixed-current loop with moment $m=I\pi R^2$ and $R\ll h$, the image field gives upward [force](force.md) $3\mu_0m^2/(32\pi h^4)$. Differentiating the external field holds the image position fixed; moving both source and image in that derivative would double the [force](force.md) incorrectly.

#### Meissner state

↑ **Parent:** [Meissner effect](#meissner-effect)

A [Meissner state](#meissner-state) is an equilibrium state of [superconductivity](superconductivity.md) without [quantum vortex](critical-phenomenon.md#quantum-vortex) penetration, with screening [electric currents](electric-charge.md#electric-current) responding to the applied [magnetic field](magnetic-field.md). In a solid, [simply connected](algebraic-topology.md#simply-connected-space) sample much thicker than the [London penetration depth](#london-penetration-depth), the deep interior [magnetic field](magnetic-field.md) is approximately zero. This is a statement about a phase and a geometry, not a rule that every sample exhibiting [superconductivity](superconductivity.md) always has $\mathbf B=0$. In particular, the [Meissner state](#meissner-state) exists for sufficiently weak [magnetic fields](magnetic-field.md) in both [type-I superconductors](superconductivity.md#type-i-superconductor) and [type-II superconductors](superconductivity.md#type-ii-superconductor). [§9.8, Properties of Superconductors, paragraphs distinguishing type I, type II and their two critical fields](physics-bibliography.md#university-physics-volume-3-by-samuel-j-ling-and-others/9-8-superconductivity)

##### Planar London screening

↑ **Parent:** [Meissner state](#meissner-state)

Take a homogeneous material exhibiting [superconductivity](superconductivity.md) in the [half-space](geometry-and-topology.md#half-space) $z\geq0$, bounded by vacuum at $z=0$. Fix the [temperature](temperature.md) below the [superconducting transition temperature](superconductivity.md#superconducting-transition-temperature), take a constant positive [London penetration depth](#london-penetration-depth) $\lambda_L$, and assume a local, linear [London equation](#london-equations) description in a [Meissner state](#meissner-state). The applied [magnetic field](magnetic-field.md) is weak enough that it neither nucleates a [quantum vortex](critical-phenomenon.md#quantum-vortex) nor appreciably suppresses the material's [superconductivity](superconductivity.md). Assume translation invariance in $x,y$, no imposed transport [electric current](electric-charge.md#electric-current), and a tangential boundary [magnetic field](magnetic-field.md) $\mathbf B(0)=B_0\widehat{\mathbf x}$. Here $B_0$ is the local surface [magnetic flux density](magnetic-field.md), equal to the imposed vacuum [magnetic field](magnetic-field.md) in this infinite planar geometry; it is not automatically the far-away applied value for a finite object.

For a bounded, decaying interior solution, the [London equations](#london-equations), [magnetostatic Ampère law](maxwell-equations.md#magnetostatic-ampere-law) and [Gauss's law for magnetism](maxwell-equations.md#gauss-s-law-for-magnetism) give

$$
\nabla^2\mathbf B=\frac{\mathbf B}{\lambda_L^2},\qquad
\frac{d^2B_x}{dz^2}=\frac{B_x}{\lambda_L^2},\qquad
B_x(0)=B_0,\quad B_x(\infty)=0.
$$

The solution is

$$
\mathbf B(z)=B_0e^{-z/\lambda_L}\widehat{\mathbf x}.
$$

At one [London penetration depth](#london-penetration-depth) the [magnetic field](magnetic-field.md) is $e^{-1}\simeq0.368$ of its surface value; at five it is $e^{-5}\simeq0.00674$. There is no finite depth where this exponential is exactly zero. The [differential equation](differential-equation.md) excludes the growing exponential through the deep-interior boundary condition. A constant normal component cannot decay in this geometry: [Gauss's law for magnetism](maxwell-equations.md#gauss-s-law-for-magnetism) would require $\partial_zB_z=0$. A perpendicular applied [magnetic field](magnetic-field.md) on a finite plate therefore requires a different spatial problem.[§2, p. 13, Eqs. (68)–(74): London screening equation; the planar boundary-value solution here follows directly](physics-bibliography.md#lecture-notes-on-the-electrodynamics-of-metals-and-superconductors)

<a id="image-magnetic-field-and-signed-meissner-screening-current-profiles-with-finite-london-penetration-depth"></a>
![](meissner-field-and-screening-current-profiles.png)

**[Figure 3](#image-magnetic-field-and-signed-meissner-screening-current-profiles-with-finite-london-penetration-depth). Magnetic field and signed Meissner screening current profiles with finite London penetration depth**. Original analytic profiles, not measured data. Left: the [Planar London screening](#planar-london-screening) solution, with vacuum at $z<0$ and the material at $z\geq0$. Right: [Finite-thickness Meissner screening](#finite-thickness-meissner-screening) in a slab of thickness $2\lambda_L$, with equal tangential surface [magnetic fields](magnetic-field.md). Blue is $B_x/B_0$; orange is the signed [current density](electric-charge.md#current-density) $\mu_0\lambda_LJ_y/B_0$. Different horizontal origins are labeled explicitly.

###### Meissner screening current

↑ **Parent:** [Planar London screening](#planar-london-screening)

In [SI](physics.md#international-system-of-units) units, the [magnetostatic Ampère law](maxwell-equations.md#magnetostatic-ampere-law) gives the [current density](electric-charge.md#current-density) supporting [Planar London screening](#planar-london-screening):

$$
\mathbf J=\frac{1}{\mu_0}\nabla\times\mathbf B
=-\frac{B_0}{\mu_0\lambda_L}e^{-z/\lambda_L}\widehat{\mathbf y}.
$$

Here $\mu_0$ is the [vacuum permeability](maxwell-equations.md#vacuum-permeability). The sign follows from $(\nabla\times\mathbf B)_y=\partial_zB_x$ in the chosen coordinates. Thus $B_0>0$ requires [electric current](electric-charge.md#electric-current) along $-\widehat{\mathbf y}$. Its own [magnetic field](magnetic-field.md) opposes the imposed [magnetic field](magnetic-field.md) inside the material. The [electric current](electric-charge.md#electric-current) is distributed over a finite layer; its depth [integral](integral.md) is the effective [surface current density](electric-charge.md#surface-current-density)

$$
\mathbf K=\int_0^\infty\mathbf J(z)\,dz
=-\frac{B_0}{\mu_0}\widehat{\mathbf y}.
$$

The units are $\mathrm{A\,m^{-2}}$ for $\mathbf J$ and $\mathrm{A\,m^{-1}}$ for $\mathbf K$. Shrinking $\lambda_L$ at fixed $B_0$ increases the surface [current density](electric-charge.md#current-density), while this integrated [surface current density](electric-charge.md#surface-current-density) stays fixed. The [current sheet](electric-charge.md#current-sheet) approximation is the large-length-scale limit of this layer, not a claim that an actual sample carries an infinitely thin [electric current](electric-charge.md#electric-current). It reproduces the [magnetic-field jump across a surface current](electric-charge.md#magnetic-field-jump-across-a-surface-current) between the exterior $B_0\widehat{\mathbf x}$ and a field-free interior, with outward [unit normal](differential-geometry.md#unit-normal) $-\widehat{\mathbf z}$.

##### Finite-thickness Meissner screening

↑ **Parent:** [Meissner state](#meissner-state)

To isolate finite size from [quantum vortex](critical-phenomenon.md#quantum-vortex) penetration, keep the same weak-field [London equations](#london-equations) but replace the [half-space](geometry-and-topology.md#half-space) by an infinite slab $-d/2\leq z\leq d/2$. Put equal tangential [magnetic fields](magnetic-field.md) $B_0\widehat{\mathbf x}$ at its two faces. With $z=0$ now at the slab center, the even solution and its signed [current density](electric-charge.md#current-density) are

$$
B_x(z)=B_0\frac{\cosh(z/\lambda_L)}{\cosh(d/(2\lambda_L))},\qquad
J_y(z)=\frac{B_0}{\mu_0\lambda_L}\frac{\sinh(z/\lambda_L)}{\cosh(d/(2\lambda_L))}.
$$

The [hyperbolic cosine](calculus.md#hyperbolic-cosine) profile has equal boundary values, while the [electric currents](electric-charge.md#electric-current) on the two sides have opposite signs. In particular,

$$
\frac{B_x(0)}{B_0}=\frac{1}{\cosh(d/(2\lambda_L))},\qquad
\frac{\overline B_x}{B_0}=\frac{1}{dB_0}\int_{-d/2}^{d/2}B_x(z)\,dz
=\frac{2\lambda_L}{d}\tanh\!\left(\frac{d}{2\lambda_L}\right).
$$

For the stipulated thickness $d=2\lambda_L$, the center retains about $0.648B_0$ and the mean is about $0.762B_0$, even though this is a [Meissner state](#meissner-state). For $d\gg\lambda_L$, the center [magnetic field](magnetic-field.md) is exponentially small and the mean is about $2\lambda_LB_0/d$, reflecting the two surface layers. For $d\ll\lambda_L$, the mean tends to $B_0$: little screening is possible across such a short distance. These are analytic model examples, not material measurements. Real finite objects also need their [demagnetizing field](statistical-physics.md#demagnetizing-field) and edge geometry accounted for; the slab calculation only isolates the effect of thickness.

#### Meissner effect and flux history

↑ **Parent:** [Meissner effect](#meissner-effect)

Compare two ideal models for a stationary, solid, [simply connected](algebraic-topology.md#simply-connected-space) sample. In the [perfect conductor](electromagnetic-wave.md#perfect-conductor) flux-history model the interior [electric field](electric-field.md) is constrained to zero from the moment perfect conduction starts. [Faraday's law of induction](maxwell-equations.md#faraday-s-law-of-induction) then gives

$$
\partial_t\mathbf B=-\nabla\times\mathbf E=0.
$$

Consequently the interior [magnetic field](magnetic-field.md) retains its value at that moment. Cooling in an already applied [magnetic field](magnetic-field.md) freezes a nonzero interior value; starting perfect conduction in zero [magnetic field](magnetic-field.md) and then applying a [magnetic field](magnetic-field.md) preserves zero. The zero initial interior [magnetic field](magnetic-field.md) often assumed in [perfect conductor](electromagnetic-wave.md#perfect-conductor) wave-reflection problems is one particular preparation, not a general prediction of expulsion. [§9.8, Eq. (9.38) and the argument that zero resistivity conserves existing flux rather than expelling it](physics-bibliography.md#university-physics-volume-3-by-samuel-j-ling-and-others/9-8-superconductivity)

<a id="image-two-preparation-histories-distinguish-the-meissner-state-from-perfect-conductor-flux-memory"></a>
![](meissner-cooling-and-field-history.png)

**[Figure 4](#image-two-preparation-histories-distinguish-the-meissner-state-from-perfect-conductor-flux-memory). Two preparation histories distinguish the Meissner state from perfect conductor flux memory**. Original schematic end states for a solid sample much thicker than its [London penetration depth](#london-penetration-depth), not measured data or transition kinetics. Both rows end at the same low [temperature](temperature.md) and applied weak [magnetic field](magnetic-field.md). Blue arrows indicate interior [magnetic field](magnetic-field.md); orange edges represent screening [electric currents](electric-charge.md#electric-current). The near-zero interior in the [Meissner state](#meissner-state) omits its finite penetration layer. The [perfect conductor](electromagnetic-wave.md#perfect-conductor) panel uses the ideal zero-interior-[electric field](electric-field.md) constraint.

The [Meissner state](#meissner-state) instead selects the screened equilibrium after either preparation, provided that equilibrium is accessible and the applied [magnetic field](magnetic-field.md) lies in the [Meissner state](#meissner-state) regime. The first [London equation](#london-equations) alone illustrates the missing information: at fixed $\lambda_L$, combining it with [Faraday's law of induction](maxwell-equations.md#faraday-s-law-of-induction) gives

$$
\partial_t\!\left(\nabla\times\mathbf J+\frac{\mathbf B}{\mu_0\lambda_L^2}\right)=0.
$$

This permits an arbitrary time-independent integration field. The second [London equation](#london-equations) imposes the additional zero value of that bracket in the vortex-free local model.[§2, pp. 12–13, Eqs. (64), (66)–(68): time-independent freedom and the second London equation](physics-bibliography.md#lecture-notes-on-the-electrodynamics-of-metals-and-superconductors) Establishing [superconductivity](superconductivity.md) during cooling is not the fixed-parameter, zero-[electric field](electric-field.md) model: transient [electric fields](electric-field.md) accompany changing [magnetic flux](#magnetic-flux), and $\lambda_L$ itself depends on [temperature](temperature.md). The equilibrium [London equations](#london-equations) predict final spatial screening, not the cooling rate or the time-resolved expulsion pulse.

#### Meissner effect discovery

↑ **Parent:** [Meissner effect](#meissner-effect)

The 1933 report [Ein neuer Effekt bei Eintritt der Supraleitfähigkeit by W. Meissner and R. Ochsenfeld](https://link.springer.com/article/10.1007/BF01504252) describes cooling tin and [lead](chemical-substance.md#lead) cylinders in a fixed transverse [magnetic field](magnetic-field.md). Two parallel cylinders were about $140\,\mathrm{mm}$ long and $3\,\mathrm{mm}$ thick, separated by $1.5\,\mathrm{mm}$. A roughly $10\,\mathrm{mm}$ rotating search coil between them drove a ballistic [galvanometer](electric-charge.md#galvanometer). At about $5\,\mathrm{G}$, the reported below/above-transition induction ratios were $1.70$ for tin single crystals and $1.77$ for polycrystalline [lead](chemical-substance.md#lead). The increased gap [magnetic field](magnetic-field.md) indicates redistribution outside the cylinders, rather than an unchanged frozen field. Coil-winding geometry and noncircular tin specimens limited comparison with the ideal prediction. [1933 report, first arrangement; English translation PDF pp. 1–2, printed p. 119, alongside the German text](physics-bibliography.md#ein-neuer-effekt-bei-eintritt-der-supraleitfahigkeit-by-walther-meissner-and-others)

Their second arrangement used a [lead](chemical-substance.md#lead) tube, about $130\,\mathrm{mm}$ long with $3\,\mathrm{mm}$ outer and $2\,\mathrm{mm}$ inner diameters. A rotating search coil could sit inside or alongside it. The bore retained [magnetic flux](#magnetic-flux) after removing the applied [magnetic field](magnetic-field.md); the coil nearly filled the bore, preventing a test of interior field uniformity. A hole containing [magnetic field](magnetic-field.md) is distinct from [magnetic field](magnetic-field.md) penetrating the surrounding material exhibiting [superconductivity](superconductivity.md). [1933 report, second arrangement; translation PDF p. 2, printed p. 119, bore retention and explicitly stated spatial-resolution limitation](physics-bibliography.md#ein-neuer-effekt-bei-eintritt-der-supraleitfahigkeit-by-walther-meissner-and-others)

The modern [Field-cooled Meissner experiment](superconductivity.md#field-cooled-meissner-experiment) provides a complementary readout. MIT's probe I places a sample in a brass holder, with an $810$-turn test coil of $7.1\,\mathrm{mm}$ inner diameter, $10.5\,\mathrm{mm}$ outer diameter and $12.3\,\mathrm{mm}$ length, inside a longer [solenoid](#solenoid). A nearby silicon-diode [thermometer](temperature.md#thermometer) tracks cooling by helium gas. With [lead](chemical-substance.md#lead) still normal, the guide applies about $200\,\mathrm{mA}$ to the [solenoid](#solenoid) and connects the test coil to a current-integrator box and [oscilloscope](wave-equation.md#oscilloscope). Cooling produces a transient; warming gives the opposite sign. Switching off the [solenoid](#solenoid) while the sample is normal checks the sign. [Probe I, §4.2 and Fig. 6, printed pp. 5–6; §4.3 temperature control; §5.2.2, printed p. 10, DC field cooling and sign control](physics-bibliography.md#superconductivity-the-meissner-effect-persistent-currents-and-the-josephson-effects-by-mit-department-of-physics)

The inferred change is in linked [magnetic flux](#magnetic-flux), not a direct scan of $B(z)$. For a stationary test coil the pulse obeys $\int V\,dt=-\Delta\Psi$, where $\Psi$ is its [magnetic flux linkage](electromagnetism.md#magnetic-flux-linkage). An integrator or AC-coupled [oscilloscope](wave-equation.md#oscilloscope) needs its transfer response accounted for before extracting this pulse area. Keep the source [electric current](electric-charge.md#electric-current) fixed during cooling, monitor [temperature](temperature.md), and compare warming and cooling slowly enough to reduce sample–[thermometer](temperature.md#thermometer) lag. An AC [inductance](electromagnetism.md#inductance) change alone can reflect changed normal-state [electrical conductivity](electric-charge.md#electrical-conductivity); the fixed-field expulsion test distinguishes that alternative. [§5.1, printed pp. 8–9, thermometer lag; §5.2.2, printed p. 10, limitation of AC mutual-inductance evidence](physics-bibliography.md#superconductivity-the-meissner-effect-persistent-currents-and-the-josephson-effects-by-mit-department-of-physics) Neither this coil readout nor the historical gap-field measurement resolves the microscopic [London penetration depth](#london-penetration-depth) by itself.

#### Limits of Meissner screening

↑ **Parent:** [Meissner effect](#meissner-effect)

For a bulk [type-II superconductor](superconductivity.md#type-ii-superconductor) with negligible [demagnetizing field](statistical-physics.md#demagnetizing-field), raising the applied [magnetic field intensity](electromagnetism.md#magnetic-field-intensity) past the lower critical value $H_{c1}$ favors a [superconducting mixed state](superconductivity.md#superconducting-mixed-state) containing [quantum vortex](critical-phenomenon.md#quantum-vortex) lines; [superconductivity](superconductivity.md) survives until the upper critical value $H_{c2}$. The [magnetic field](magnetic-field.md) extends around each vortex over a penetration scale, not solely inside its core. Thus a nonzero average [magnetic flux density](magnetic-field.md) can coexist with [superconductivity](superconductivity.md). Below $H_{c1}$, a [type-II superconductor](superconductivity.md#type-ii-superconductor) also supports a [Meissner state](#meissner-state); a vortex-free state above the equilibrium entry field may instead be [metastable](critical-phenomenon.md#metastability). [§9.8, type-II critical-field and mixed-state paragraphs; the source uses B\_c1 and B\_c2 for applied-field scales](physics-bibliography.md#university-physics-volume-3-by-samuel-j-ling-and-others/9-8-superconductivity)

Real preparation histories may leave [quantum vortex](critical-phenomenon.md#quantum-vortex) lines held in place by material inhomogeneities, retaining [magnetic flux](#magnetic-flux) and producing [hysteresis](critical-phenomenon.md#hysteresis). This [flux pinning](superconductivity.md#flux-pinning) restricts access to equilibrium: it is different from the arbitrary frozen interior [magnetic field](magnetic-field.md) of the ideal [perfect conductor](electromagnetic-wave.md#perfect-conductor) model. Harvard's vortex-imaging work illustrates strong pinning to bulk disorder in a [type-II superconductor](superconductivity.md#type-ii-superconductor). [Vortex Imaging in Iron Pnictide Superconductor, Fig. 2 and the discussion of disordered vortices and bulk pinning](physics-bibliography.md#scanning-tunneling-microscopy-research-by-hoffman-laboratory) Separately, [flux conservation in a superconducting loop](mathematical-physics.md#flux-conservation-in-a-superconducting-loop) and [fluxoid and flux quantization in a superconductor](quantum-theory.md#fluxoid-and-flux-quantization-in-a-superconductor) explain why a hole can retain [magnetic flux](#magnetic-flux). Neither bore retention, vortex penetration nor weak screening in a thin sample should be silently identified with the equilibrium [Planar London screening](#planar-london-screening) calculation.

## Magnetic flux

↑ **Parent:** [Magnetic field](magnetic-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetic_flux)

[Magnetic flux](#magnetic-flux) measures the signed amount of [magnetic field](magnetic-field.md) crossing an [oriented surface](differential-geometry.md#oriented-surface) $S$. Choose a [unit normal](differential-geometry.md#unit-normal) $\widehat{\mathbf n}$ and use the [oriented surface element](multivariable-calculus.md#oriented-surface-element) $d\mathbf S=\widehat{\mathbf n}\,dA$. The defining [surface integral](multivariable-calculus.md#surface-integral) is

$$
\Phi_B=\int_S\mathbf B\cdot d\mathbf S
=\int_S\mathbf B\cdot\widehat{\mathbf n}\,dA.
$$

For a uniform [magnetic field](magnetic-field.md) across a flat [surface](topological-surface.md) of [area](differential-geometry.md#surface-area) $A$, the [dot product](inner-product.md#dot-product) reduces this to

$$
\Phi_B=BA\cos\theta,
$$

where $\theta$ is the [angle](geometry-and-topology.md#angle) between the [magnetic field](magnetic-field.md) and the chosen [unit normal](differential-geometry.md#unit-normal), rather than the [plane](geometry-and-topology.md#plane) of the [surface](topological-surface.md). The [SI](physics.md#international-system-of-units) unit is the [weber](#weber-unit), $1\,\mathrm{Wb}=1\,\mathrm{T\,m^2}$. [OpenStax, magnetic flux and its orientation](https://openstax.org/books/university-physics-volume-2/pages/13-1-faradays-law).

For a stipulated [magnetic field](magnetic-field.md) $B=2\,\mathrm T$ and [area](differential-geometry.md#surface-area) $A=3\,\mathrm{m^2}$, the [magnetic flux](#magnetic-flux) is $6\,\mathrm{Wb}$ at $\theta=0$, $3\,\mathrm{Wb}$ at $\theta=\pi/3$, and zero at $\theta=\pi/2$. In the last case the [magnetic field](magnetic-field.md) lies in the [plane](geometry-and-topology.md#plane) of the [surface](topological-surface.md), so it does not cross it. Reversing the chosen [unit normal](differential-geometry.md#unit-normal) reverses the sign of [magnetic flux](#magnetic-flux) without changing the physical [magnetic field](magnetic-field.md); at $\theta=\pi$ the same example gives $-6\,\mathrm{Wb}$.

<a id="image-magnetic-flux-as-a-flat-surface-rotates-in-a-fixed-magnetic-field"></a>
![](magnetic-flux-orientation.png)

**[Figure 5](#image-magnetic-flux-as-a-flat-surface-rotates-in-a-fixed-magnetic-field). Magnetic flux as a flat surface rotates in a fixed magnetic field**. Left: an edge-on [surface](topological-surface.md) and its [unit normal](differential-geometry.md#unit-normal) at three [angles](geometry-and-topology.md#angle) to the fixed [magnetic field](magnetic-field.md). Right: the signed [magnetic flux](#magnetic-flux) $\Phi_B=6\cos\theta\,\mathrm{Wb}$, including reversal of the [unit normal](differential-geometry.md#unit-normal). The stipulated [magnetic field](magnetic-field.md) is $2\,\mathrm T$ and the [area](differential-geometry.md#surface-area) is $3\,\mathrm{m^2}$.

The geometric idea is projected [area](differential-geometry.md#surface-area): tilting a flat [surface](topological-surface.md) reduces the [area](differential-geometry.md#surface-area) seen perpendicular to the [magnetic field](magnetic-field.md) by the factor $\cos\theta$. This explains how rotation alone can change [magnetic flux](#magnetic-flux) even when the [magnetic field](magnetic-field.md) is constant; [Faraday's law of induction](maxwell-equations.md#faraday-s-law-of-induction) turns such changes into an [electromotive force](electric-charge.md#electromotive-force). [OpenStax, induction from changing magnetic flux](https://openstax.org/books/university-physics-volume-2/pages/13-1-faradays-law).

### Weber (unit)

↑ **Parent:** [Magnetic flux](#magnetic-flux)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weber_(unit))

The [weber](#weber-unit) is the [SI](physics.md#international-system-of-units) unit of [magnetic flux](#magnetic-flux), with $1\,\mathrm{Wb}=1\,\mathrm{T\,m^2}$. A uniform [magnetic field](magnetic-field.md) of $1\,\mathrm T$ crossing a flat [surface](topological-surface.md) of [area](differential-geometry.md#surface-area) $1\,\mathrm{m^2}$ along its chosen [unit normal](differential-geometry.md#unit-normal) gives $1\,\mathrm{Wb}$. [OpenStax, magnetic-flux units](https://openstax.org/books/university-physics-volume-2/pages/13-1-faradays-law).

## Electromagnet

↑ **Parent:** [Magnetic field](magnetic-field.md)

A device that produces a [magnetic field](magnetic-field.md) from an [electric current](electric-charge.md#electric-current).

## ↑ Ancestors (4)

1. [Electromagnetism](electromagnetism.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (746)

- [Accreting X-ray pulsar](stellar-astrophysics.md#accreting-x-ray-pulsar)
- [Accretion column](astrophysical-disk.md#accretion-column)
- [Adiabatic demagnetization](temperature.md#adiabatic-demagnetization)
- [Aharonov-Bohm effect](topological-quantum-matter.md#aharonov-bohm-effect)
- [Alfvén frequency](ideal-magnetohydrodynamics.md#alfven-frequency)
- [Alfvén-resonant vorticity in a parallel magnetic shear flow](ideal-magnetohydrodynamics.md#alfven-resonant-vorticity-in-a-parallel-magnetic-shear-flow)
- [Alfvén velocity](ideal-magnetohydrodynamics.md#alfven-velocity)
- [Alfvén wave](ideal-magnetohydrodynamics.md#alfven-wave)
- [Alfvén wave energy transport](ideal-magnetohydrodynamics.md#alfven-wave-energy-transport)
- [Alpha effect](resistive-magnetohydrodynamics.md#alpha-effect)
- [Alpha-squared dynamo](resistive-magnetohydrodynamics.md#alpha-squared-dynamo)
- [Alpha tensor](resistive-magnetohydrodynamics.md#alpha-tensor)
- [Alvarez hydrogen-bubble-chamber reconstruction and resonances](particle-detection.md#alvarez-hydrogen-bubble-chamber-reconstruction-and-resonances)
- [Anderson positron track experiment](relativistic-electromagnetism.md#anderson-positron-track-experiment)
- [Anomalous Zeeman effect](atomic-physics.md#anomalous-zeeman-effect)
- [Antiproton](relativistic-quantum-field.md#antiproton)
- [Antiproton mass from momentum and velocity](relativistic-quantum-field.md#antiproton-mass-from-momentum-and-velocity)
- [Arrott plot](critical-phenomenon.md#arrott-plot)
- [Axisymmetric magnetic field near a regular axis](maxwell-equations.md#axisymmetric-magnetic-field-near-a-regular-axis)
- [Axisymmetric magnetic flux surface](ideal-magnetohydrodynamics.md#axisymmetric-magnetic-flux-surface)
- [Barkhausen effect](electromagnetism.md#barkhausen-effect)
- [Barnett effect](electromagnetism.md#barnett-effect)
- [Barnett equivalent magnetic field](electromagnetism.md#barnett-equivalent-magnetic-field)
- [Barnett response of a magnetic material](electromagnetism.md#barnett-response-of-a-magnetic-material)
- [Barnett rotation magnetometry experiment](electromagnetism.md#barnett-rotation-magnetometry-experiment)
- [Biot-Savart law](electromagnetism.md#biot-savart-law)
- [Blackett-Occhialini triggered cloud-chamber experiment](particle-detection.md#blackett-occhialini-triggered-cloud-chamber-experiment)
- [Bloch nuclear induction experiment](nuclear-magnetic-resonance.md#bloch-nuclear-induction-experiment)
- [Boosted uniform line charge](relativistic-electromagnetism.md#boosted-uniform-line-charge)
- [Brookhaven J pair-spectrometer experiment](particle-detection.md#brookhaven-j-pair-spectrometer-experiment)
- [Bubble-chamber stereo reconstruction](particle-detection.md#bubble-chamber-stereo-reconstruction)
- [Bubble-chamber track readout](particle-detection.md#bubble-chamber-track-readout)
- [Calorimeter addenda](heat.md#calorimeter-addenda)
- [Canonical Hamiltonian of a magnetic elastic ring](lagrangian-mechanics.md#canonical-hamiltonian-of-a-magnetic-elastic-ring)
- [Capacitor](electromagnetism.md#capacitor)
- [Cartesian magnetic flux function](ideal-magnetohydrodynamics.md#cartesian-magnetic-flux-function)
- [Cesium-beam clock procedure](special-relativity.md#cesium-beam-clock-procedure)
- [Chamberlain-Segrè antiproton identification](relativistic-quantum-field.md#chamberlain-segre-antiproton-identification)
- [Charge conservation](electric-charge.md#charge-conservation)
- [Charge-sign ambiguity of a curved track](relativistic-electromagnetism.md#charge-sign-ambiguity-of-a-curved-track)
- [Charge-to-mass ratio](relativistic-electromagnetism.md#charge-to-mass-ratio)
- [Circular modes of a charged isotropic oscillator](wave-equation.md#circular-modes-of-a-charged-isotropic-oscillator)
- [Classical Heisenberg model](angular-momentum-operator.md#classical-heisenberg-model)
- [Closed-return induction under a voltage pulse](maxwell-equations.md#closed-return-induction-under-a-voltage-pulse)
- [Cold-atom collapse and revival after a lattice quench](quantum-mechanics.md#cold-atom-collapse-and-revival-after-a-lattice-quench)
- [Cold-plasma radio dispersion](geophysics.md#cold-plasma-radio-dispersion)
- [Collapse of a planar magnetic separatrix](ideal-magnetohydrodynamics.md#collapse-of-a-planar-magnetic-separatrix)
- [Compass](#compass)
- [Confined linear-pressure spherical magnetic equilibrium](#confined-linear-pressure-spherical-magnetic-equilibrium)
- [Conformal-surface vortex square completion](classical-field-theory-soliton.md#conformal-surface-vortex-square-completion)
- [Constant-entropy magnetic cooling example](temperature.md#constant-entropy-magnetic-cooling-example)
- [Cosmic ray](galaxy.md#cosmic-ray)
- [Coulomb-gauge vector potential of a long solenoid](electromagnetism.md#coulomb-gauge-vector-potential-of-a-long-solenoid)
- [Covalent bond](covalent-bond.md)
- [Covariant transversality of a vacuum plane wave](electromagnetic-wave.md#covariant-transversality-of-a-vacuum-plane-wave)
- [Cowling anti-dynamo theorem](resistive-magnetohydrodynamics.md#cowling-anti-dynamo-theorem)
- [Cross-helicity conservation law](ideal-magnetohydrodynamics.md#cross-helicity-conservation-law)
- [Cubic-time resistive damping in a differentially rotating cell](resistive-magnetohydrodynamics.md#cubic-time-resistive-damping-in-a-differentially-rotating-cell)
- [Curie temperature](electromagnetism.md#curie-temperature)
- [Current helicity](electromagnetism.md#current-helicity)
- [Current-loop torque experiment](electromagnetism.md#current-loop-torque-experiment)
- [Current sheet](electric-charge.md#current-sheet)
- [Cyclotron](particle-accelerator.md#cyclotron)
- [Cyclotron energy and orbit radius](particle-accelerator.md#cyclotron-energy-and-orbit-radius)
- [Cyclotron period](quantum-theory.md#cyclotron-period)
- [Cyclotron radius](relativistic-electromagnetism.md#cyclotron-radius)
- [Cyclotron resonance](quantum-theory.md#cyclotron-resonance)
- [Cyclotron resonance condition](particle-accelerator.md#cyclotron-resonance-condition)
- [Derrick scaling of the Abelian Higgs energy](classical-field-theory-soliton.md#derrick-scaling-of-the-abelian-higgs-energy)
- [Dimensional freedom of an MHD spectrum](turbulence.md#dimensional-freedom-of-an-mhd-spectrum)
- [Displacement equation for a parallel magnetic shear flow](ideal-magnetohydrodynamics.md#displacement-equation-for-a-parallel-magnetic-shear-flow)
- [DPPH electron spin resonance experiment](chemistry.md#dpph-electron-spin-resonance-experiment)
- [Drift chamber](particle-detection.md#drift-chamber)
- [Drude conductivity and Hall experiment](electric-charge.md#drude-conductivity-and-hall-experiment)
- [Drude model](electric-charge.md#drude-model)
- [Dynamo action](resistive-magnetohydrodynamics.md#dynamo-action)
- [Earth's outer core](planetary-science.md#earth-s-outer-core)
- [Eddy current](electromagnetism.md#eddy-current)
- [Eddy-current damping](wave-equation.md#eddy-current-damping)
- [Einstein-de Haas effect](electromagnetism.md#einstein-de-haas-effect)
- [Einstein-de Haas experiment](electromagnetism.md#einstein-de-haas-experiment)
- [Electric drift in crossed uniform fields](relativistic-electromagnetism.md#electric-drift-in-crossed-uniform-fields)
- [Electric field of a uniformly moving point charge](relativistic-electromagnetism.md#electric-field-of-a-uniformly-moving-point-charge)
- [Electromagnet](#electromagnet)
- [Electromagnetic field](electromagnetism.md#electromagnetic-field)
- [Electromagnetic induction](electromagnetism.md#electromagnetic-induction)
- [Electromagnetic radiation](electromagnetic-radiation.md)
- [Electromagnetic wave](electromagnetic-wave.md)
- [Electromagnetic wave equation](electromagnetic-wave.md#electromagnetic-wave-equation)
- [Electromagnetism](electromagnetism.md)
- [Electron lens](optics.md#electron-lens)
- [Electron magnetic moment](electromagnetism.md#electron-magnetic-moment)
- [Electron magnetohydrodynamics](magnetohydrodynamics.md#electron-magnetohydrodynamics)
- [Electron optics](optics.md#electron-optics)
- [Electrostatics](electrostatics.md)
- [Elsässer energy invariant](ideal-magnetohydrodynamics.md#elsasser-energy-invariant)
- [Energy decay criterion for a viscous-resistive shearing box](gravitational-instability-of-an-astrophysical-disk.md#energy-decay-criterion-for-a-viscous-resistive-shearing-box)
- [Evanescent transverse electric mode in a rectangular waveguide](electromagnetic-wave.md#evanescent-transverse-electric-mode-in-a-rectangular-waveguide)
- [Far-field approximation for a current loop](electromagnetism.md#far-field-approximation-for-a-current-loop)
- [Faraday effect](electromagnetic-wave.md#faraday-effect)
- [Faraday rotation in a glass-rod experiment](electromagnetic-wave.md#faraday-rotation-in-a-glass-rod-experiment)
- [Faraday rotation on a round trip](electromagnetic-wave.md#faraday-rotation-on-a-round-trip)
- [Faraday's law of induction](maxwell-equations.md#faraday-s-law-of-induction)
- [Fe-Cr giant magnetoresistance experiments](electric-charge.md#fe-cr-giant-magnetoresistance-experiments)
- [Fermi energy](quantum-ideal-gas-statistics.md#fermi-energy)
- [Fermi-energy oscillations in a two-dimensional electron gas](quantum-theory.md#fermi-energy-oscillations-in-a-two-dimensional-electron-gas)
- [Fermionic atom antibunching](tensor-product-of-quantum-systems.md#fermionic-atom-antibunching)
- [Ferraro's law of isorotation](ideal-magnetohydrodynamics.md#ferraro-s-law-of-isorotation)
- [Ferromagnetism](electromagnetism.md#ferromagnetism)
- [Field-cooled Meissner experiment](superconductivity.md#field-cooled-meissner-experiment)
- [Field-induced triplon condensation](quantum-ideal-gas-statistics.md#field-induced-triplon-condensation)
- [Field-line angular velocity of an axisymmetric wind](ideal-magnetohydrodynamics.md#field-line-angular-velocity-of-an-axisymmetric-wind)
- [Filling factor (quantum Hall effect)](quantum-theory.md#filling-factor-quantum-hall-effect)
- [Finite-thickness magnetorotational instability criterion](astrophysical-disk.md#finite-thickness-magnetorotational-instability-criterion)
- [Finite-thickness Meissner screening](#finite-thickness-meissner-screening)
- [Flux expulsion](resistive-magnetohydrodynamics.md#flux-expulsion)
- [Flux-lattice spacing](superconductivity.md#flux-lattice-spacing)
- [Flux tube](#flux-tube)
- [Flux-tube area](#flux-tube-area)
- [Fluxgate magnetometer](electromagnetism.md#fluxgate-magnetometer)
- [Fock-Darwin spectrum](semiconductor.md#fock-darwin-spectrum)
- [Force on a current sheet from the mean magnetic field](electric-charge.md#force-on-a-current-sheet-from-the-mean-magnetic-field)
- [Free-particle momentum convention](wave-function.md#free-particle-momentum-convention)
- [Frustrated Ising triangle](spin-model.md#frustrated-ising-triangle)
- [Galvanometer](electric-charge.md#galvanometer)
- [Galvanometer current sensitivity](electric-charge.md#galvanometer-current-sensitivity)
- [Galvanometer radial field](electric-charge.md#galvanometer-radial-field)
- [Geodynamo](planetary-science.md#geodynamo)
- [Geomagnetic reversal](planetary-science.md#geomagnetic-reversal)
- [Geophysics](geophysics.md)
- [Geselowitz formula](electromagnetism.md#geselowitz-formula)
- [Giaever gap experiment](superconductivity.md#giaever-gap-experiment)
- [Giauque-MacDougall magnetic cooling experiment](temperature.md#giauque-macdougall-magnetic-cooling-experiment)
- [Ginzburg-Landau theory of superconductivity](superconductivity.md#ginzburg-landau-theory-of-superconductivity)
- [Gold-iron alloy susceptibility experiment](spin-model.md#gold-iron-alloy-susceptibility-experiment)
- [Gouy balance](statistical-physics.md#gouy-balance)
- [Graphene exfoliation and field-effect experiments](chemical-substance.md#graphene-exfoliation-and-field-effect-experiments)
- [Gyroradius](relativistic-electromagnetism.md#gyroradius)
- [Hahn spin echo experiment](nuclear-magnetic-resonance.md#hahn-spin-echo-experiment)
- [Hall angle](relativistic-electromagnetism.md#hall-angle)
- [Hall coefficient](relativistic-electromagnetism.md#hall-coefficient)
- [Hall effect](relativistic-electromagnetism.md#hall-effect)
- [Hall voltage](relativistic-electromagnetism.md#hall-voltage)
- [Hartmann flow](resistive-magnetohydrodynamics.md#hartmann-flow)
- [Hartmann flow rate with normal-field walls](resistive-magnetohydrodynamics.md#hartmann-flow-rate-with-normal-field-walls)
- [Hartmann layer](resistive-magnetohydrodynamics.md#hartmann-layer)
- [Heat capacity of a classical magnetic dipole](statistical-physics.md#heat-capacity-of-a-classical-magnetic-dipole)
- [Helical motion in a uniform magnetic field](electromagnetism.md#helical-motion-in-a-uniform-magnetic-field)
- [Helicity formula for isotropic first-order smoothing](resistive-magnetohydrodynamics.md#helicity-formula-for-isotropic-first-order-smoothing)
- [Helium-3 superfluid discovery experiment](statistical-physics.md#helium-3-superfluid-discovery-experiment)
- [Helmholtz coil](electromagnetism.md#helmholtz-coil)
- [Hendrik Antoon Lorentz](physicist.md#hendrik-antoon-lorentz)
- [High-pressure limit of magnetosonic waves](ideal-magnetohydrodynamics.md#high-pressure-limit-of-magnetosonic-waves)
- [High-temperature superconductivity](superconductivity.md#high-temperature-superconductivity)
- [Hofstadter nuclear electron scattering experiment](atomic-nucleus.md#hofstadter-nuclear-electron-scattering-experiment)
- [Homopolar generator](electromagnetism.md#homopolar-generator)
- [Horizontally invariant magnetized shearing-sheet equations](astrophysical-disk.md#horizontally-invariant-magnetized-shearing-sheet-equations)
- [Hyperbolic one-vortex at curvature minus one half](classical-field-theory-soliton.md#hyperbolic-one-vortex-at-curvature-minus-one-half)
- [Ideal magnetorotational dispersion relation](astrophysical-disk.md#ideal-magnetorotational-dispersion-relation)
- [Independent spin Barnett response](electromagnetism.md#independent-spin-barnett-response)
- [Induced current in a tilted resistive loop](maxwell-equations.md#induced-current-in-a-tilted-resistive-loop)
- [Induced magnetosphere](planetary-science.md#induced-magnetosphere)
- [Inductance](electromagnetism.md#inductance)
- [Inductive Barkhausen experiment](electromagnetism.md#inductive-barkhausen-experiment)
- [Inductor](electromagnetism.md#inductor)
- [Inelastic neutron scattering](neutron.md#inelastic-neutron-scattering)
- [Inferring incident power from a transmitted plasma field](physics.md#inferring-incident-power-from-a-transmitted-plasma-field)
- [Insulating boundary condition for the radial magnetic scalar](resistive-magnetohydrodynamics.md#insulating-boundary-condition-for-the-radial-magnetic-scalar)
- [Interference (wave propagation)](physical-optics.md#interference-wave-propagation)
- [Invariant-mass resolution](particle-detection.md#invariant-mass-resolution)
- [Ion trap](atomic-physics.md#ion-trap)
- [Ising model](spin-model.md#ising-model)
- [Ising ring magnetization fluctuations](spin-model.md#ising-ring-magnetization-fluctuations)
- [Isothermal magnetic Bernoulli integral](ideal-magnetohydrodynamics.md#isothermal-magnetic-bernoulli-integral)
- [Kastler-Brossel optical pumping experiments](atomic-physics.md#kastler-brossel-optical-pumping-experiments)
- [Kelvin thermoelectric relation](thermoelectric-effect.md#kelvin-thermoelectric-relation)
- [Kinematic magnetic dynamo](magnetohydrodynamics.md#kinematic-magnetic-dynamo)
- [Lamb-Retherford experiment](atomic-physics.md#lamb-retherford-experiment)
- [Landau diamagnetism](electromagnetism.md#landau-diamagnetism)
- [Larmor frequency](angular-momentum-operator.md#larmor-frequency)
- [Larmor theorem](relativistic-electromagnetism.md#larmor-theorem)
- [Laughlin wavefunction](relativistic-electromagnetism.md#laughlin-wavefunction)
- [Lawrence-Livingston cyclotron experiment](particle-accelerator.md#lawrence-livingston-cyclotron-experiment)
- [Lenz's law](maxwell-equations.md#lenz-s-law)
- [Liénard-Wiechert field](relativistic-electromagnetism.md#lienard-wiechert-field)
- [Limits of adiabatic demagnetization](temperature.md#limits-of-adiabatic-demagnetization)
- [Limits of Meissner screening](#limits-of-meissner-screening)
- [Linear Alfvén wave equations](ideal-magnetohydrodynamics.md#linear-alfven-wave-equations)
- [Localized interchange criterion for a magnetized atmosphere](magnetohydrodynamics.md#localized-interchange-criterion-for-a-magnetized-atmosphere)
- [London equations](#london-equations)
- [Long-solenoid approximation](#long-solenoid-approximation)
- [Longitudinal nuclear spin relaxation](nuclear-magnetic-resonance.md#longitudinal-nuclear-spin-relaxation)
- [Longitudinal solenoid field under an axial boost](relativistic-electromagnetism.md#longitudinal-solenoid-field-under-an-axial-boost)
- [Lorentz force](relativistic-electromagnetism.md#lorentz-force)
- [Lower critical magnetic field](superconductivity.md#lower-critical-magnetic-field)
- [Lowest Landau level](quantum-theory.md#lowest-landau-level)
- [Lundquist liquid-metal Alfvén wave experiment](ideal-magnetohydrodynamics.md#lundquist-liquid-metal-alfven-wave-experiment)
- [Magnet](electromagnetism.md#magnet)
- [Magnetic angular-momentum invariant](electromagnetism.md#magnetic-angular-momentum-invariant)
- [Magnetic anisotropy](electromagnetism.md#magnetic-anisotropy)
- [Magnetic anomaly](geophysics.md#magnetic-anomaly)
- [Magnetic buoyancy instability](magnetohydrodynamics.md#magnetic-buoyancy-instability)
- [Magnetic compensation temperature](electromagnetism.md#magnetic-compensation-temperature)
- [Magnetic concentration by an incompressible stagnation flow](resistive-magnetohydrodynamics.md#magnetic-concentration-by-an-incompressible-stagnation-flow)
- [Magnetic diffusion](magnetohydrodynamics.md#magnetic-diffusion)
- [Magnetic dipole force](electromagnetism.md#magnetic-dipole-force)
- [Magnetic dipole moment](electromagnetism.md#magnetic-dipole-moment)
- [Magnetic dipole torque](electromagnetism.md#magnetic-dipole-torque)
- [Magnetic dipole transition](atomic-physics.md#magnetic-dipole-transition)
- [Magnetic domain-wall pinning](electromagnetism.md#magnetic-domain-wall-pinning)
- [Magnetic electron lens](optics.md#magnetic-electron-lens)
- [Magnetic energy density](#magnetic-energy-density)
- [Magnetic entropy](temperature.md#magnetic-entropy)
- [Magnetic field](magnetic-field.md)
- [Magnetic-field-aligned rolls evade steady magnetic inhibition](magnetohydrodynamics.md#magnetic-field-aligned-rolls-evade-steady-magnetic-inhibition)
- [Magnetic-field cancellation of an arc and tangent leads](electromagnetism.md#magnetic-field-cancellation-of-an-arc-and-tangent-leads)
- [Magnetic-field-dependent Langmuir adsorption](physical-chemistry.md#magnetic-field-dependent-langmuir-adsorption)
- [Magnetic field line](#magnetic-field-line)
- [Magnetic field of a finite straight wire](electromagnetism.md#magnetic-field-of-a-finite-straight-wire)
- [Magnetic field of a rotating charged solid cylinder](electromagnetism.md#magnetic-field-of-a-rotating-charged-solid-cylinder)
- [Magnetic field of a rotating charged spherical body](electromagnetism.md#magnetic-field-of-a-rotating-charged-spherical-body)
- [Magnetic field of a uniformly conducting strip](electromagnetism.md#magnetic-field-of-a-uniformly-conducting-strip)
- [Magnetic flux](#magnetic-flux)
- [Magnetic flux linkage](electromagnetism.md#magnetic-flux-linkage)
- [Magnetic flux transport for a moving circuit](electric-charge.md#magnetic-flux-transport-for-a-moving-circuit)
- [Magnetic helicity](electromagnetism.md#magnetic-helicity)
- [Magnetic-history constant in an undamped plasma](electromagnetic-wave.md#magnetic-history-constant-in-an-undamped-plasma)
- [Magnetic island](ideal-magnetohydrodynamics.md#magnetic-island)
- [Magnetic Jeans mass](stellar-astrophysics.md#magnetic-jeans-mass)
- [Magnetic length](quantum-theory.md#magnetic-length)
- [Magnetic polarizability of a perfectly conducting sphere](electromagnetism.md#magnetic-polarizability-of-a-perfectly-conducting-sphere)
- [Magnetic pressure discontinuity in an isothermal atmosphere](magnetohydrodynamics.md#magnetic-pressure-discontinuity-in-an-isothermal-atmosphere)
- [Magnetic relaxation](ideal-magnetohydrodynamics.md#magnetic-relaxation)
- [Magnetic reversal and domain averaging](elasticity-physics.md#magnetic-reversal-and-domain-averaging)
- [Magnetic reversal measurement of Faraday rotation](electromagnetic-wave.md#magnetic-reversal-measurement-of-faraday-rotation)
- [Magnetic rigidity](relativistic-electromagnetism.md#magnetic-rigidity)
- [Magnetic scalar potential](electromagnetism.md#magnetic-scalar-potential)
- [Magnetic shielding](electromagnetism.md#magnetic-shielding)
- [Magnetic skin layer](resistive-magnetohydrodynamics.md#magnetic-skin-layer)
- [Magnetic spectrometer](optical-instrument.md#magnetic-spectrometer)
- [Magnetic stabilization of an equal-density vortex sheet](ideal-magnetohydrodynamics.md#magnetic-stabilization-of-an-equal-density-vortex-sheet)
- [Magnetic sublevel](quantum-mechanics.md#magnetic-sublevel)
- [Magnetic susceptibility](statistical-physics.md#magnetic-susceptibility)
- [Magnetic tweezers](electromagnetism.md#magnetic-tweezers)
- [Magnetically channelled accretion](astrophysical-disk.md#magnetically-channelled-accretion)
- [Magnetism](electromagnetism.md#magnetism)
- [Magnetization](electromagnetism.md#magnetization)
- [Magnetized isothermal atmosphere](#magnetized-isothermal-atmosphere)
- [Magneto-optical trap](atomic-physics.md#magneto-optical-trap)
- [Magnetoconvection](magnetohydrodynamics.md#magnetoconvection)
- [Magnetohydrodynamic shear work](ideal-magnetohydrodynamics.md#magnetohydrodynamic-shear-work)
- [Magnetohydrodynamic turbulence](turbulence.md#magnetohydrodynamic-turbulence)
- [Magnetohydrodynamic wave polarization](ideal-magnetohydrodynamics.md#magnetohydrodynamic-wave-polarization)
- [Magnetometer](electromagnetism.md#magnetometer)
- [Magnetoresistance](electric-charge.md#magnetoresistance)
- [Magnetosphere](planetary-science.md#magnetosphere)
- [Magnetostriction](elasticity-physics.md#magnetostriction)
- [Magnetostrophic Taylor state](magnetohydrodynamics.md#magnetostrophic-taylor-state)
- [Magnetron motion](atomic-physics.md#magnetron-motion)
- [Martinis-Devoret-Clarke circuit experiments](superconductivity.md#martinis-devoret-clarke-circuit-experiments)
- [Mass spectrograph](chemistry.md#mass-spectrograph)
- [Mass spectrometry](chemistry.md#mass-spectrometry)
- [Material conservation of cross-helicity density](ideal-magnetohydrodynamics.md#material-conservation-of-cross-helicity-density)
- [Material transport of magnetic helicity density](electromagnetism.md#material-transport-of-magnetic-helicity-density)
- [Maxwell equations](maxwell-equations.md)
- [Mean-field dynamo](resistive-magnetohydrodynamics.md#mean-field-dynamo)
- [Meissner effect](#meissner-effect)
- [Meissner effect and flux history](#meissner-effect-and-flux-history)
- [Meissner effect discovery](#meissner-effect-discovery)
- [Meissner screening current](#meissner-screening-current)
- [Meissner state](#meissner-state)
- [Mercury (planet)](planetary-science.md#mercury-planet)
- [Michael criterion for axisymmetric toroidal-field interchange](magnetohydrodynamics.md#michael-criterion-for-axisymmetric-toroidal-field-interchange)
- [Molecular beam](physics.md#molecular-beam)
- [Momentum-space Poisson structure for a uniform magnetic field](symplectic-geometry.md#momentum-space-poisson-structure-for-a-uniform-magnetic-field)
- [Monochromatic small-Reynolds-number mean electromotive force](resistive-magnetohydrodynamics.md#monochromatic-small-reynolds-number-mean-electromotive-force)
- [Motional electromotive force](electric-charge.md#motional-electromotive-force)
- [Moving-coil galvanometer](electric-charge.md#moving-coil-galvanometer)
- [Moving-coil galvanometer torque](electric-charge.md#moving-coil-galvanometer-torque)
- [Near-axis radial magnetic field](maxwell-equations.md#near-axis-radial-magnetic-field)
- [Néel temperature](electromagnetism.md#neel-temperature)
- [Neutral Coulomb pair in a uniform magnetic field](quantum-theory.md#neutral-coulomb-pair-in-a-uniform-magnetic-field)
- [Neutral current filament in a boosted frame](relativistic-electromagnetism.md#neutral-current-filament-in-a-boosted-frame)
- [Neutron Stern-Gerlach splitting](angular-momentum-operator.md#neutron-stern-gerlach-splitting)
- [Nonlinear Alfvén wave](ideal-magnetohydrodynamics.md#nonlinear-alfven-wave)
- [Nonmagnetic cataclysmic variable](stellar-astrophysics.md#nonmagnetic-cataclysmic-variable)
- [Normal magnetic field boundary condition](resistive-magnetohydrodynamics.md#normal-magnetic-field-boundary-condition)
- [Nuclear magnetic moment](electromagnetism.md#nuclear-magnetic-moment)
- [Nuclear magnetic resonance](nuclear-magnetic-resonance.md)
- [Nuclear magnetic resonance fingerprint of superfluid helium-3](statistical-physics.md#nuclear-magnetic-resonance-fingerprint-of-superfluid-helium-3)
- [Nuclear magneton](electromagnetism.md#nuclear-magneton)
- [Numerical Calculations of the Dynamics of a Collapsing Proto-Star by Richard B. Larson](physics-bibliography.md#numerical-calculations-of-the-dynamics-of-a-collapsing-proto-star-by-richard-b-larson)
- [On-axis entry into a solenoidal tube](electromagnetism.md#on-axis-entry-into-a-solenoidal-tube)
- [On-axis magnetic field of a circular current loop](electromagnetism.md#on-axis-magnetic-field-of-a-circular-current-loop)
- [On-axis magnetic field of a finite solenoid](#on-axis-magnetic-field-of-a-finite-solenoid)
- [Onsager quantization](quantum-theory.md#onsager-quantization)
- [Optical molasses](atomic-physics.md#optical-molasses)
- [Optical nonreciprocity](optics.md#optical-nonreciprocity)
- [Optical pumping preparation and readout](atomic-physics.md#optical-pumping-preparation-and-readout)
- [Oscillation of a uniformly wound coil](electromagnetism.md#oscillation-of-a-uniformly-wound-coil)
- [Otto Stern](physicist.md#otto-stern)
- [Parallel current sheets with a resistive termination](electric-charge.md#parallel-current-sheets-with-a-resistive-termination)
- [Parallel magnetohydrodynamic shock](ideal-magnetohydrodynamics.md#parallel-magnetohydrodynamic-shock)
- [Parker instability](magnetohydrodynamics.md#parker-instability)
- [Particle accelerator](particle-accelerator.md)
- [Particle identification](particle-detection.md#particle-identification)
- [Paschen-Back effect](atomic-physics.md#paschen-back-effect)
- [Solution](past-exam-of-the-advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge/2013/paper-1.md#2/d/solution)
- [Solution](past-exam-of-the-advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge/2014/paper-1.md#3/b/solution)
- [Solution](past-exam-of-the-advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge/2016/paper-1.md#3/b/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2014/paper-1.md#4/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2015/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2016/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017.md#1/a/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017.md#2/b/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017.md#3/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2019.md#section-a/3/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-a/3/solution)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022.md#section-b/4/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2012/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2012/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2013/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2013/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2014/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2014/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2014/paper-1.md#3/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2015/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2017.md#2/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2018.md#section-a/a1/b/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2021.md#section-a/2/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2021.md#section-b/5/e/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2022.md#section-a/3/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2012/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2013/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2015/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2016/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2022/paper-2.md#a6/d/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#2/b/ii/solution)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2013/paper-1.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-35.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-35.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-36.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-36.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-36.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-36.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-36.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-36.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-38.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-38.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-42.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4.md#4e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-43.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-46.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-64.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4.md#11a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2.md#18b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2.md#7b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-62.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-62.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-62.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-68.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-4.md#9c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2.md#17h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-71.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-73.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-75.md#2/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-75.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-76.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-76.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-76.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2.md#17g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3.md#17g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1.md#34e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-51.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-51.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-70.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1.md#16e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4.md#7e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65.md#2/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-68.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-68.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-75.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1.md#16b/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-55.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-65.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-69.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-74.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-76.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2.md#17a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#15e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-64.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-67.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-67.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4.md#3b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#35b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#1/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#1/a/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-74.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1.md#9c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1.md#9c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-77.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3.md#11c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-52.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-52.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4.md#7a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-54.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-54.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4.md#10c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#33a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-57.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-57.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-57.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-57.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-60.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-60.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-60.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-64.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-64.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-65.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4.md#3b/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2.md#6d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3.md#17d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3.md#17d/b/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4.md#7d/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-318.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-318.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#35d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#8e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-303.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-303.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-305.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-308.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#4/h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-316.md#2/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-4.md#10a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-314.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-314.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-314.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-315.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-321.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-322.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2.md#15d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#34c/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#36d/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1.md#15d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-4.md#3c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#15d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#8d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-314.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-4.md#5d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1.md#37d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2.md#6/b/i/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2020/paper-2.md#section-a-ii/15/i/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2021/paper-2.md#section-a-ii/16/ii/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2012/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2012/paper-1.md#4/d/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2013/paper-1.md#1/c/i/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2013/paper-1.md#4/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2014/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2015/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2015/paper-1.md#3/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2016/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2016/paper-1.md#3/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2017.md#3/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2017.md#4/solution)
- [Vanishing field components](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2018.md#section-b/b3/vanishing-field-components)
- [Radiation fields](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2019.md#section-b/b4/radiation-fields)
- [Transversality and tensor conventions](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2019.md#section-b/b6/transversality-and-tensor-conventions)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2021.md#section-b/b5/d/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2022.md#section-b/4/b/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2022.md#section-b/4/e/1/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2022.md#section-b/4/e/2/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2022.md#section-b/6/b/1/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2022.md#section-b/6/d/solution)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2022.md#section-b/6/e/solution)
- [Solution](past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge/2021.md#section-b/4/b/solution)
- [Solution](past-exam-of-the-particle-astrophysics-course-of-the-university-of-cambridge/2012/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-1.md#section-d/d12/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-2.md#section-d/d13/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2.md#section-a/5/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1.md#section-c/c11/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2.md#section-d/d13/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1.md#section-b/b6/d/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2.md#section-d/d13/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1.md#section-a/3/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1.md#section-b/b6/d/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a.md#section-b/b8/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1.md#section-b/b6/c/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1.md#section-b/b6/d/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-2.md#section-b/b8/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-2.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-1.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-b/b6/d/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-b/b7/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-1.md#section-b/b7/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-1.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-1.md#section-b/b7/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-1.md#section-b/b8/b/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-1.md#section-b/b8/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2.md#section-b/b6/a/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2.md#section-c/c12/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1.md#section-a/a4/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1.md#section-b/b7/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1.md#section-a/a3/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1.md#section-b/b8/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2.md#section-b/b6/d/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-1.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-a/a5/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-b/b6/c/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-b/b7/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-a/a1/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-b/b6/a/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-b/b6/d/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2.md#section-a/a4/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2.md#section-b/b6/c/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-1.md#section-c/c9/d/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-2.md#section-a/a4/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2.md#section-b/b7/c/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#section-e/e15/a/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1.md#section-e/e15/d/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#section-e/e14/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#section-e/e15/b/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#section-e/e15/c/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#section-e/e14/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#section-e/e15/b/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#section-e/e15/d/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#section-e/e14/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#section-e/e15/c/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#section-e/e15/d/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017.md#section-e/15/a/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017.md#section-e/15/c/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018.md#section-e/15/c/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019.md#section-a/5/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021.md#section-b/10/a/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021.md#section-b/10/b/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021.md#section-b/10/c/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022.md#section-b/10/a/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022.md#section-b/10/b/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022.md#section-b/10/c/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022.md#section-b/10/d/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1.md#section-b/b5/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2012/paper-1.md#2/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2012/paper-1.md#3/b/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2013/paper-1.md#1/b/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2015/paper-1.md#1/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2015/paper-1.md#2/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2015/paper-1.md#3/b/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2016/paper-1.md#1/solution)
- [Solution](past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2016/paper-1.md#2/solution)
- [Solution](past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2016/paper-1.md#1/e/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-b/b9/a/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2006.md#section-b/b4/d/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2008.md#section-b/b1/a/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2008.md#section-b/b2/d/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2009.md#section-b/b2/c/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012.md#2/b/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012.md#2/c/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2014.md#2/b/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2016.md#2/c/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2019.md#section-a/1/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2019.md#section-b/5/a/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2022.md#section-b/6/e/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2013/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2014/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2014/paper-1.md#3/e/solution)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2015/paper-1.md#3/c/solution)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2016/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2016/paper-1.md#3/d/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2012/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2014/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2019.md#section-b/b4/solution)
- [Solution](past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2013/paper-1.md#1/solution)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2012/paper-1.md#3/solution)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2015/paper-1.md#1/b/solution)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2016/paper-1.md#3/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2013/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2015/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2016/paper-1.md#4/b/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2017.md#2/a/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2018.md#1/a/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2018.md#1/b/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2018.md#1/d/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2018.md#1/e/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2019.md#4/a/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2022.md#3/f/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2019.md#1/a/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017.md#3/a/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2018.md#section-b/b4/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2019.md#section-b/4/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021.md#section-b/5/a/solution)
- [Pauli exclusion principle](tensor-product-of-quantum-systems.md#pauli-exclusion-principle)
- [Penning trap](atomic-physics.md#penning-trap)
- [Penning trap normal modes](atomic-physics.md#penning-trap-normal-modes)
- [Perfect conductor](electromagnetic-wave.md#perfect-conductor)
- [Permanent magnet](electromagnetism.md#permanent-magnet)
- [Perpendicular fast magnetosonic simple wave](compressible-flow.md#perpendicular-fast-magnetosonic-simple-wave)
- [Perpendicular magnetohydrodynamic shock](ideal-magnetohydrodynamics.md#perpendicular-magnetohydrodynamic-shock)
- [Persistent current in a superconducting loop experiment](superconductivity.md#persistent-current-in-a-superconducting-loop-experiment)
- [Persistent current (superconductivity)](superconductivity.md#persistent-current-superconductivity)
- [Phase mixing in magnetic flux expulsion](resistive-magnetohydrodynamics.md#phase-mixing-in-magnetic-flux-expulsion)
- [Pieter Zeeman](physicist.md#pieter-zeeman)
- [Planar anti-dynamo theorem](resistive-magnetohydrodynamics.md#planar-anti-dynamo-theorem)
- [Planar London screening](#planar-london-screening)
- [Planetary dynamo](planetary-science.md#planetary-dynamo)
- [Polarization of Zeeman components](atomic-physics.md#polarization-of-zeeman-components)
- [Polarization-selective Zeeman splitting of an alkali D1 line](atomic-physics.md#polarization-selective-zeeman-splitting-of-an-alkali-d1-line)
- [Poloidal magnetic energy bound by the radial scalar gradient](multivariable-calculus.md#poloidal-magnetic-energy-bound-by-the-radial-scalar-gradient)
- [Poloidal magnetic field](magnetohydrodynamics.md#poloidal-magnetic-field)
- [Power-law poloidal field near a disk surface](ideal-magnetohydrodynamics.md#power-law-poloidal-field-near-a-disk-surface)
- [Power-law pressure-supported axial current](#power-law-pressure-supported-axial-current)
- [Poynting flux into lossy coaxial conductors](electrical-engineering.md#poynting-flux-into-lossy-coaxial-conductors)
- [Proton exclusion by magnetic rigidity and range](relativistic-electromagnetism.md#proton-exclusion-by-magnetic-rigidity-and-range)
- [Pseudo-Alfvén wave](ideal-magnetohydrodynamics.md#pseudo-alfven-wave)
- [Pulsed-field optical magnetostriction experiment](elasticity-physics.md#pulsed-field-optical-magnetostriction-experiment)
- [Quantum-dot versus antidot resonance topology](relativistic-electromagnetism.md#quantum-dot-versus-antidot-resonance-topology)
- [Quantum electrodynamics](perturbative-quantum-field-theory.md#quantum-electrodynamics)
- [Quantum Hall antidot](relativistic-electromagnetism.md#quantum-hall-antidot)
- [Quantum Hall conductivity tensor inversion](relativistic-electromagnetism.md#quantum-hall-conductivity-tensor-inversion)
- [Quantum Hall effect](relativistic-electromagnetism.md#quantum-hall-effect)
- [Quasistatic electromagnetic approximation](electromagnetism.md#quasistatic-electromagnetic-approximation)
- [Rabi molecular beam magnetic resonance experiment](quantum-system.md#rabi-molecular-beam-magnetic-resonance-experiment)
- [Rabi transit-time and field averaging](quantum-system.md#rabi-transit-time-and-field-averaging)
- [Radial current dipole](electric-charge.md#radial-current-dipole)
- [Radial energy flow after switching a line current](relativistic-electromagnetism.md#radial-energy-flow-after-switching-a-line-current)
- [Radial escape in an inverse-radius axial magnetic field](relativistic-electromagnetism.md#radial-escape-in-an-inverse-radius-axial-magnetic-field)
- [Radial magnetic induction scalar](resistive-magnetohydrodynamics.md#radial-magnetic-induction-scalar)
- [Radially stratified magnetorotational dispersion relation](astrophysical-disk.md#radially-stratified-magnetorotational-dispersion-relation)
- [Ramsey spectroscopy](quantum-system.md#ramsey-spectroscopy)
- [Rayleigh centrifugal stability criterion](astrophysical-disk.md#rayleigh-centrifugal-stability-criterion)
- [Rectangular electromagnetic waveguide](electromagnetic-wave.md#rectangular-electromagnetic-waveguide)
- [Relativistic cyclotron orbit](relativistic-electromagnetism.md#relativistic-cyclotron-orbit)
- [Relativistic detuning of a cyclotron](particle-accelerator.md#relativistic-detuning-of-a-cyclotron)
- [Release-expansion thermometry](atomic-physics.md#release-expansion-thermometry)
- [Remanent magnetization](electromagnetism.md#remanent-magnetization)
- [Resistive magnetic entry of a falling loop](electromagnetism.md#resistive-magnetic-entry-of-a-falling-loop)
- [Resistive magnetohydrodynamics](resistive-magnetohydrodynamics.md)
- [Resistivity and Hall Measurements by National Institute of Standards and Technology](physics-bibliography.md#resistivity-and-hall-measurements-by-national-institute-of-standards-and-technology)
- [Right-hand rule](electromagnetism.md#right-hand-rule)
- [RLC circuit](electrical-circuit.md#rlc-circuit)
- [Rotation measure](electromagnetic-wave.md#rotation-measure)
- [Seebeck effect](thermoelectric-effect.md#seebeck-effect)
- [Shearing-coordinate magnetic flux equation](resistive-magnetohydrodynamics.md#shearing-coordinate-magnetic-flux-equation)
- [Shielded toroidal-flux electron interference](topological-quantum-matter.md#shielded-toroidal-flux-electron-interference)
- [Shubnikov-de Haas effect](bloch-s-theorem.md#shubnikov-de-haas-effect)
- [SLAC-MIT spectrometer readout and corrections](standard-model.md#slac-mit-spectrometer-readout-and-corrections)
- [Small-angle magnetic dipole oscillation](electromagnetism.md#small-angle-magnetic-dipole-oscillation)
- [Sodium D-line Zeeman pattern](atomic-physics.md#sodium-d-line-zeeman-pattern)
- [Solar wind](astrophysics.md#solar-wind)
- [Solenoid](#solenoid)
- [Solenoid inductance](#solenoid-inductance)
- [Solenoid turn density](#solenoid-turn-density)
- [Solenoidal magnetic-field constraint](#solenoidal-magnetic-field-constraint)
- [Spherical magnetostatic pressure balance](#spherical-magnetostatic-pressure-balance)
- [Spin degeneracy](statistical-physics.md#spin-degeneracy)
- [Spin-orbit g-factor ratio from two P states](electromagnetism.md#spin-orbit-g-factor-ratio-from-two-p-states)
- [Standard Reference Materials: Critical current measurements on an NbTi superconducting wire standard reference material by A. F. Clark and others](physics-bibliography.md#standard-reference-materials-critical-current-measurements-on-an-nbti-superconducting-wire-standard-reference-material-by-a-f-clark-and-others)
- [Stark effect](mathematical-physics.md#stark-effect)
- [Starspot](exoplanet.md#starspot)
- [Statistical reflection symmetry](probability-and-statistics.md#statistical-reflection-symmetry)
- [Steady planar ideal-MHD field-line invariants](ideal-magnetohydrodynamics.md#steady-planar-ideal-mhd-field-line-invariants)
- [Steady toroidal induction by spherical differential rotation](magnetohydrodynamics.md#steady-toroidal-induction-by-spherical-differential-rotation)
- [Stellar rotation-activity feedback](stellar-astrophysics.md#stellar-rotation-activity-feedback)
- [Stern-Gerlach apparatus in 1922](angular-momentum-operator.md#stern-gerlach-apparatus-in-1922)
- [Stern-Gerlach discrete and classical profiles](angular-momentum-operator.md#stern-gerlach-discrete-and-classical-profiles)
- [Stern-Gerlach expectation estimation](quantum-system.md#stern-gerlach-expectation-estimation)
- [Stern-Gerlach experiment](angular-momentum-operator.md#stern-gerlach-experiment)
- [Stern-Gerlach force and flight model](angular-momentum-operator.md#stern-gerlach-force-and-flight-model)
- [Stern-Gerlach historical and modern interpretations](angular-momentum-operator.md#stern-gerlach-historical-and-modern-interpretations)
- [Stored energy of a solenoid](#stored-energy-of-a-solenoid)
- [Stratified magneto-Coriolis wave](magnetohydrodynamics.md#stratified-magneto-coriolis-wave)
- [Stream tube](fluid-mechanics.md#stream-tube)
- [Sunspot](stellar-astrophysics.md#sunspot)
- [Super Proton-Antiproton Synchrotron](particle-accelerator.md#super-proton-antiproton-synchrotron)
- [Superconducting coherence length](superconductivity.md#superconducting-coherence-length)
- [Superconducting critical current](superconductivity.md#superconducting-critical-current)
- [Superconducting critical current density](superconductivity.md#superconducting-critical-current-density)
- [Superconducting critical surface](superconductivity.md#superconducting-critical-surface)
- [Superconducting transition temperature](superconductivity.md#superconducting-transition-temperature)
- [Superconductivity](superconductivity.md)
- [Tesla (unit)](#tesla-unit)
- [Thermodynamic limit](statistical-physics.md#thermodynamic-limit)
- [Theta pinch](magnetohydrodynamics.md#theta-pinch)
- [Thomson charge-to-mass experiment](relativistic-electromagnetism.md#thomson-charge-to-mass-experiment)
- [Thomson electron transmission diffraction experiment](wave-function.md#thomson-electron-transmission-diffraction-experiment)
- [Time reversal of an electromagnetic gauge field](quantum-field-theory.md#time-reversal-of-an-electromagnetic-gauge-field)
- [Toroidal-velocity anti-dynamo theorem](resistive-magnetohydrodynamics.md#toroidal-velocity-anti-dynamo-theorem)
- [Transformer (electrical engineering)](electrical-engineering.md#transformer-electrical-engineering)
- [Transport and magnetic tests of superconducting ceramics](superconductivity.md#transport-and-magnetic-tests-of-superconducting-ceramics)
- [Transverse electric mode](electromagnetic-wave.md#transverse-electric-mode)
- [Transverse electric mode of a rectangular waveguide](electromagnetic-wave.md#transverse-electric-mode-of-a-rectangular-waveguide)
- [Transverse electromagnetic mode](electromagnetic-wave.md#transverse-electromagnetic-mode)
- [Transverse magnetic focusing](quantum-ideal-gas-statistics.md#transverse-magnetic-focusing)
- [Transverse nuclear magnetization decay](nuclear-magnetic-resonance.md#transverse-nuclear-magnetization-decay)
- [Transverse wave](wave.md#transverse-wave)
- [Trapped-electron spin-jump readout](atomic-physics.md#trapped-electron-spin-jump-readout)
- [Triplon](critical-phenomenon.md#triplon)
- [Tsui-Störmer-Gossard fractional Hall experiment](relativistic-electromagnetism.md#tsui-stormer-gossard-fractional-hall-experiment)
- [Turbulent magnetic diffusivity](magnetohydrodynamics.md#turbulent-magnetic-diffusivity)
- [Turbulent magnetic pumping](resistive-magnetohydrodynamics.md#turbulent-magnetic-pumping)
- [Two-dimensional electron gas](quantum-ideal-gas-statistics.md#two-dimensional-electron-gas)
- [Two-level paramagnetic cooling model](temperature.md#two-level-paramagnetic-cooling-model)
- [Uniform magnetic field with axial harmonic confinement](electromagnetism.md#uniform-magnetic-field-with-axial-harmonic-confinement)
- [Uniformly magnetized cylinder](electromagnetism.md#uniformly-magnetized-cylinder)
- [Upper critical magnetic field](superconductivity.md#upper-critical-magnetic-field)
- [Vector calculus](multivariable-calculus.md#vector-calculus)
- [Velocity selector](relativistic-electromagnetism.md#velocity-selector)
- [Verdet constant](electromagnetic-wave.md#verdet-constant)
- [Vibrating-sample magnetometer](electromagnetism.md#vibrating-sample-magnetometer)
- [Viscous magnetic-relaxation energy identity](ideal-magnetohydrodynamics.md#viscous-magnetic-relaxation-energy-identity)
- [W and Z discovery experiments](particle-detection.md#w-and-z-discovery-experiments)
- [Walther Gerlach](physicist.md#walther-gerlach)
- [Weak-field Zeeman splitting](atomic-physics.md#weak-field-zeeman-splitting)
- [Weak spin-forbidden Paschen-Back line](atomic-physics.md#weak-spin-forbidden-paschen-back-line)
- [Weber (unit)](#weber-unit)
- [Wu experiment](standard-model.md#wu-experiment)
- [Zeeman discovery experiment of 1896](atomic-physics.md#zeeman-discovery-experiment-of-1896)
- [Zeeman slower](atomic-physics.md#zeeman-slower)
- [Zeeman slower resonance tracking](atomic-physics.md#zeeman-slower-resonance-tracking)
- [Zeeman splitting](atomic-physics.md#zeeman-splitting)
- [Zeeman splitting of an antiferromagnetic spin wave](statistical-physics.md#zeeman-splitting-of-an-antiferromagnetic-spin-wave)
- [Zero-mean magnetic shearing wave](gravitational-instability-of-an-astrophysical-disk.md#zero-mean-magnetic-shearing-wave)
- [Zero-temperature filling of finite fermion levels](tensor-product-of-quantum-systems.md#zero-temperature-filling-of-finite-fermion-levels)
