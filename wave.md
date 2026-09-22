# Wave

↑ **Parent:** [Physics](physics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wave)

A wave is a propagating or standing disturbance that can carry [energy](energy.md) and momentum. Its oscillations are described by quantities such as [wavelength](wave-equation.md#wavelength), [frequency](#frequency), and [wave speed](wave-equation.md#wave-speed).

**Table of contents**

- [Spherical wave](#spherical-wave)
- [Waveguide](#waveguide)
- [Chirp](#chirp)
- [Transverse wave](#transverse-wave)
- [Longitudinal wave](#longitudinal-wave)
- [Monochromatic wave](#monochromatic-wave)
- [Intensity (physics)](#intensity-physics)
  - [Light intensity](#light-intensity)
- [Polarization (waves)](#polarization-waves)
  - [Pure polarization](#pure-polarization)
  - [Degree of polarization](#degree-of-polarization)
  - [Coherency matrix](#coherency-matrix)
  - [Jones calculus](#jones-calculus)
    - [Jones matrix](#jones-matrix)
      - [Circular-eigenmode Jones propagator](#circular-eigenmode-jones-propagator)
    - [Jones vector](#jones-vector)
      - [Jones-component ratio sensitivity](#jones-component-ratio-sensitivity)
  - [Elliptical polarization](#elliptical-polarization)
    - [Elliptical polarization from circular and linear components](#elliptical-polarization-from-circular-and-linear-components)
    - [Polarization ellipse](#polarization-ellipse)
  - [Malus's law](#malus-s-law)
    - [Transmission through a sequence of linear polarizers](#transmission-through-a-sequence-of-linear-polarizers)
  - [Unpolarized light](#unpolarized-light)
- [Oscillation](#oscillation)
  - [Oscillator](#oscillator)
    - [Coupled oscillator](#coupled-oscillator)
      - [Three coupled pendulums with equal end masses](#three-coupled-pendulums-with-equal-end-masses)
        - [End-displacement release of three coupled pendulums](#end-displacement-release-of-three-coupled-pendulums)
      - [Absolute and signed beat envelopes](#absolute-and-signed-beat-envelopes)
      - [Normal modes of two spring-coupled equal pendulums](#normal-modes-of-two-spring-coupled-equal-pendulums)
  - [Anharmonicity](#anharmonicity)
- [Wave period](#wave-period)
- [Angular spectrum](#angular-spectrum)
- [Wave focusing](#wave-focusing)
- [Wave amplitude](#wave-amplitude)
  - [Peak-to-peak amplitude](#peak-to-peak-amplitude)
  - [Scalar wave intensity](#scalar-wave-intensity)
  - [Complex amplitude](#complex-amplitude)
    - [Phase convention for complex amplitudes](#phase-convention-for-complex-amplitudes)
    - [Phasor](#phasor)
- [Phase (waves)](#phase-waves)
  - [Phase shift](#phase-shift)
  - [Phase factor](#phase-factor)
  - [Phase difference](#phase-difference)
  - [Phase quadrature](#phase-quadrature)
- [Wave absorption](#wave-absorption)
- [Wave reflection](#wave-reflection)
- [Multipath propagation](#multipath-propagation)
- [Wave reciprocity](#wave-reciprocity)
  - [Weighted acoustic Green-function reciprocity](#weighted-acoustic-green-function-reciprocity)
- [Time-harmonic wave](#time-harmonic-wave)
- [Wave scattering](#wave-scattering)
  - [Scattered wave](#scattered-wave)
  - [Incident wave](#incident-wave)
  - [Differential cross-section for scalar wave scattering](#differential-cross-section-for-scalar-wave-scattering)
    - [Finite-volume random scattering spectrum](#finite-volume-random-scattering-spectrum)
  - [Random medium](#random-medium)
    - [Wave propagation in a random medium](#wave-propagation-in-a-random-medium)
      - [Anderson localization](#anderson-localization)
        - [Weak localization](#weak-localization)
        - [Mobility gap](#mobility-gap)
        - [Localized eigenstate](#localized-eigenstate)
          - [Localization length](#localization-length)
          - [Participation ratio](#participation-ratio)
        - [Mobility edge](#mobility-edge)
        - [One-dimensional Anderson chain](#one-dimensional-anderson-chain)
        - [Semiconductor transport evidence for localization](#semiconductor-transport-evidence-for-localization)
      - [Uncentered wave-field correlation](#uncentered-wave-field-correlation)
      - [Ensemble-averaged wave intensity](#ensemble-averaged-wave-intensity)
      - [Coherent wave field](#coherent-wave-field)
        - [Gaussian coherent-field propagation in the Markov approximation](#gaussian-coherent-field-propagation-in-the-markov-approximation)
        - [Weak-fluctuation memory equation for the coherent field](#weak-fluctuation-memory-equation-for-the-coherent-field)
          - [Quadratic refractive-index shift in the coherent field](#quadratic-refractive-index-shift-in-the-coherent-field)
  - [Point scatterer](#point-scatterer)
    - [Short-distance regularization of a resonant point scatterer](#short-distance-regularization-of-a-resonant-point-scatterer)
  - [Multiple scattering](#multiple-scattering)
    - [Multiple Coulomb scattering](#multiple-coulomb-scattering)
- [Frequency](#frequency)
  - [Frequency ratio](#frequency-ratio)
  - [Radio frequency](#radio-frequency)
  - [Hertz](#hertz)
- [Doppler effect](#doppler-effect)
  - [Rotational Doppler effect](#rotational-doppler-effect)
    - [Rotating half-wave plate frequency shift](#rotating-half-wave-plate-frequency-shift)
  - [Relativistic Doppler effect](#relativistic-doppler-effect)
    - [Frequency ratio of corotating clocks](#frequency-ratio-of-corotating-clocks)
    - [Doppler extrema for a circularly moving source](#doppler-extrema-for-a-circularly-moving-source)
    - [Transverse Doppler shift and observation time](#transverse-doppler-shift-and-observation-time)
    - [Moving-mirror Doppler shift](#moving-mirror-doppler-shift)
      - [Moving-mirror photon interception rate](#moving-mirror-photon-interception-rate)
    - [Kinematic redshift](#kinematic-redshift)
  - [Classical Doppler effect for sound](#classical-doppler-effect-for-sound)
  - [Doppler frequency along a trajectory](#doppler-frequency-along-a-trajectory)
  - [Acoustic Doppler measurement](#acoustic-doppler-measurement)
- [Wave propagation](#wave-propagation)

## Spherical wave

↑ **Parent:** [Wave](wave.md)

For time dependence $e^{-i\omega t}$, the three-dimensional radial solutions $e^{ikr}/r$ and $e^{-ikr}/r$ describe outgoing and incoming [spherical waves](#spherical-wave) away from the origin. Their inverse-radius amplitudes make their flux through spheres independent of radius. They form the asymptotic radial ingredients of [partial-wave scattering](quantum-scattering.md#partial-wave-scattering).

## Waveguide

↑ **Parent:** [Wave](wave.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Waveguide)

A [waveguide](#waveguide) confines a wave transversely while allowing propagation along a longitudinal direction. Material properties and [boundary conditions](differential-equation.md#boundary-condition) select transverse [normal modes](wave-equation.md#normal-mode), whose longitudinal [dispersion relations](dispersion-relation.md) may have cutoffs even when the bulk material is nondispersive. Examples include an [optical fiber](optical-instrument.md#optical-fiber), a hollow [electromagnetic waveguide](electromagnetic-wave.md#electromagnetic-waveguide), and a [membrane waveguide](wave-equation.md#membrane-waveguide). Guiding reduces geometric spreading along the chosen route but does not eliminate absorption, scattering or leakage.

## Chirp

↑ **Parent:** [Wave](wave.md)

A [chirp](#chirp) is a signal whose instantaneous [frequency](#frequency) changes with time.

## Transverse wave

↑ **Parent:** [Wave](wave.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transverse_wave)

A [transverse wave](#transverse-wave) has its oscillating [vector](vector-space.md#vector) perpendicular to the direction of propagation. In a plane [electromagnetic wave](electromagnetic-wave.md) in vacuum, the [electric field](electric-field.md) and [magnetic field](magnetic-field.md) are transverse; their orientation is described by [polarization of waves](#polarization-waves).

## Longitudinal wave

↑ **Parent:** [Wave](wave.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Longitudinal_wave)

A [longitudinal wave](#longitudinal-wave) has an oscillating [displacement](classical-mechanics.md#displacement) parallel to the direction of propagation. An [acoustic wave](fluid-mechanics.md#acoustic-wave) in a fluid supplies a familiar example.

## Monochromatic wave

↑ **Parent:** [Wave](wave.md)

A [monochromatic wave](#monochromatic-wave) has a single [angular frequency](lagrangian-mechanics.md#angular-frequency). Its sinusoidal components can have different [wave amplitudes](#wave-amplitude) and [wave phases](#phase-waves) while sharing that [angular frequency](lagrangian-mechanics.md#angular-frequency), as in the [polarization of waves](#polarization-waves) examples.

## Intensity (physics)

↑ **Parent:** [Wave](wave.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Intensity_(physics))

[Wave intensity](#intensity-physics) measures the time-averaged [power](energy.md#power) transferred through unit [area](differential-geometry.md#surface-area) perpendicular to propagation. Its [SI](physics.md#international-system-of-units) units are $\mathrm{W\,m^{-2}}$.

### Light intensity

↑ **Parent:** [Intensity (physics)](#intensity-physics)

Here [light intensity](#light-intensity) means the time-averaged energy flux per perpendicular [area](differential-geometry.md#surface-area) for [light](optics.md#light). It is the propagation-direction component of the averaged [Poynting vector](electromagnetic-wave.md#poynting-vector). For plane [electromagnetic waves](electromagnetic-wave.md) in the same medium it is proportional to squared [electric field](electric-field.md) [wave amplitude](#wave-amplitude), giving the projection-squared factor in [Malus's law](#malus-s-law).

## Polarization (waves)

↑ **Parent:** [Wave](wave.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polarization_(waves))

[Polarization of waves](#polarization-waves) describes the direction and time-dependent geometry of a [transverse wave](#transverse-wave)'s [vector](vector-space.md#vector) during its [oscillation](#oscillation) at a fixed position. In three spatial dimensions, a [transverse wave](#transverse-wave) can have two independent directions of [oscillation](#oscillation), both perpendicular to its direction of propagation. For [polarization of an electromagnetic wave](electromagnetic-wave.md#polarization-of-an-electromagnetic-wave), the relevant [vector](vector-space.md#vector) is the transverse [electric field](electric-field.md); for a mechanical [transverse wave](#transverse-wave), it can be the transverse [displacement](classical-mechanics.md#displacement). A purely [longitudinal wave](#longitudinal-wave) has no choice between these transverse directions, and the orientation of a static [electric field](electric-field.md) is not [polarization of waves](#polarization-waves).

Choose transverse axes $x,y$ in a [Cartesian coordinate system](linear-algebra.md#cartesian-coordinate-system). A [monochromatic wave](#monochromatic-wave) with a fixed [phase difference](#phase-difference) has the real [electric field](electric-field.md)

$$
\mathbf E(t)=\bigl(A_x\cos\omega t,\ A_y\cos(\omega t+\delta)\bigr),\qquad A_x,A_y\geq0,\quad\omega>0.
$$

Here $A_x,A_y$ are [wave amplitudes](#wave-amplitude), $\omega$ is the [angular frequency](lagrangian-mechanics.md#angular-frequency), and $\delta$ is the [phase difference](#phase-difference) of the $y$ [oscillation](#oscillation) relative to the $x$ [oscillation](#oscillation). The [vector](vector-space.md#vector)'s tip traces its path during the [wave period](#wave-period) $T=2\pi/\omega$. Both plotted coordinates are real [electric field](electric-field.md) components; neither axis represents the [imaginary part](complex-analysis.md#imaginary-part) of a [complex amplitude](#complex-amplitude).

For nonzero [wave amplitudes](#wave-amplitude), $\delta=0$ or $\pi$ modulo $2\pi$ gives [linear polarization](electromagnetic-wave.md#linear-polarization): the [vector](vector-space.md#vector) moves back and forth along a fixed line. Equal nonzero [wave amplitudes](#wave-amplitude) and $\delta=\pm\pi/2$ modulo $2\pi$ give [circular polarization](electromagnetic-wave.md#circular-polarization): the tip traces a [circle](topology.md#circle) of constant [radius](topology.md#radius). Unequal nonzero [wave amplitudes](#wave-amplitude) with $\delta=\pm\pi/2$ give a noncircular [ellipse](euclidean-geometry.md#ellipse) whose axes coincide with $x,y$. More generally, nonzero [wave amplitudes](#wave-amplitude) and $\sin\delta\neq0$ give [elliptical polarization](#elliptical-polarization), with [circular polarization](electromagnetic-wave.md#circular-polarization) as a special case. If exactly one [wave amplitude](#wave-amplitude) vanishes, the nonzero [wave](wave.md) has [linear polarization](electromagnetic-wave.md#linear-polarization) for every $\delta$; if both vanish, there is no nonzero [wave](wave.md) to assign a [polarization of waves](#polarization-waves). [Feynman Lectures, I §33–1: the electric vector of light](https://www.feynmanlectures.caltech.edu/I_33.html#Ch33-S1).

For example, take $\omega=2\pi\,\mathrm{s}^{-1}$, so the [wave period](#wave-period) is $T=1\,\mathrm{s}$. The choices $(A_x,A_y,\delta)=(2,1,0)$, $(1,1,\pi/2)$ and $(2,1,\pi/2)$, with [electric field](electric-field.md) [wave amplitudes](#wave-amplitude) in $\mathrm{V/m}$, produce respectively the [line segment](convex-set.md#line-segment) $E_y=E_x/2$, the [circle](topology.md#circle) $E_x^2+E_y^2=1$ and the [ellipse](euclidean-geometry.md#ellipse) $E_x^2/4+E_y^2=1$, when coordinates are measured in $\mathrm{V/m}$. At $t=T/4$, their tips are respectively $(0,0)$, $(0,-1)$ and $(0,-1)\,\mathrm{V/m}$. The last two share a point without having the same path.

<a id="image-real-transverse-electric-field-trajectories-for-linear-polarization-circular-polarization-and-elliptical-polarization"></a>
![](wave-polarization-trajectories.png)

**[Figure 1](#image-real-transverse-electric-field-trajectories-for-linear-polarization-circular-polarization-and-elliptical-polarization). Real transverse electric field trajectories for linear polarization, circular polarization and elliptical polarization**. All panels use the same coordinate scale. Orange arrows follow increasing [wave phase](#phase-waves) $\phi=\omega t$; the dot marks $\phi=0$. The blue [vector](vector-space.md#vector) is the [electric field](electric-field.md) at $\phi=\pi/4$. These are paths at one fixed position, rather than spatial drawings of a propagating [wave](wave.md).

Resolving the [electric field](electric-field.md) into two transverse components makes [polarization of waves](#polarization-waves) useful: the same [frequency](#frequency) and [wave amplitudes](#wave-amplitude) can describe different paths when their [phase difference](#phase-difference) changes. An ideal linear [polarizer](electromagnetic-wave.md#polarizer) selects the component along its pass axis, letting its orientation probe the direction of [linear polarization](electromagnetic-wave.md#linear-polarization) through [Malus's law](#malus-s-law). A fixed pair of [wave amplitudes](#wave-amplitude) and a fixed [phase difference](#phase-difference) describe one stable path; [unpolarized light](#unpolarized-light) requires a statistical description rather than one fixed [ellipse](euclidean-geometry.md#ellipse).

### Pure polarization

↑ **Parent:** [Polarization (waves)](#polarization-waves)

[Pure polarization](#pure-polarization) means that the transverse components of a light field have a fixed complex amplitude ratio. A single [Jones vector](#jones-vector) describes the state; its [coherency matrix](#coherency-matrix) has rank one. Removing overall intensity and a common phase leaves two real parameters, which determine its [polarization ellipse](#polarization-ellipse).

### Degree of polarization

↑ **Parent:** [Polarization (waves)](#polarization-waves)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Degree_of_polarization)

The [degree of polarization](#degree-of-polarization) quantifies how strongly a transverse optical field departs from an unpolarized mixture. Here $\mu_1\geq\mu_2\geq0$ are the [eigenvalues](linear-operator-theory.md#eigenvalue) of its [coherency matrix](#coherency-matrix). For two mutually uncorrelated orthogonal linear components of intensities $I_1,I_2$, $\mathcal P=|I_1-I_2|/(I_1+I_2)$. It is undefined when the total [light intensity](#light-intensity) is zero. A signed difference is a separate convention that also identifies a preferred polarization direction.

### Coherency matrix

↑ **Parent:** [Polarization (waves)](#polarization-waves)

The optical [coherency matrix](#coherency-matrix) records the second moments of transverse [complex amplitudes](#complex-amplitude). Normalize its trace to [light intensity](#light-intensity). Under a deterministic [Jones matrix](#jones-matrix) $M$, $C\mapsto MCM^\dagger$. [Unpolarized light](#unpolarized-light) has $C=(I_0/2)I_2$, so its output intensity is $(I_0/2)\operatorname{tr}(MM^\dagger)$; it cannot be represented by one fixed [Jones vector](#jones-vector).

### Jones calculus

↑ **Parent:** [Polarization (waves)](#polarization-waves)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jones_calculus)

Jones calculus represents fully polarized [light](optics.md#light) by a [Jones vector](#jones-vector) and linear optical transformations by complex [matrices](vector-space.md#matrix).

#### Jones matrix

↑ **Parent:** [Jones calculus](#jones-calculus)

A [Jones matrix](#jones-matrix) is a complex two-by-two linear transformation of a [Jones vector](#jones-vector) through a deterministic nondepolarizing optical element. Successive elements multiply in reverse reading order. An ideal linear [polarizer](electromagnetic-wave.md#polarizer) along a real transverse [unit vector](vector-space.md#unit-vector) $\mathbf a$ has matrix $\mathbf a\mathbf a^{\mathsf T}$. A common nonzero scalar phase does not change the output [polarization of waves](#polarization-waves).

##### Circular-eigenmode Jones propagator

↑ **Parent:** [Jones matrix](#jones-matrix)

For fixed circular [eigenvectors](linear-operator-theory.md#eigenvector) $\mathbf u_\pm=(1,\mp i)^{\mathsf T}/\sqrt2$, let $P_\pm=\mathbf u_\pm\mathbf u_\pm^\dagger$. A uniform optical medium with amplitude propagation coefficients $\gamma^\pm$ has the displayed [Jones matrix](#jones-matrix). Put $\gamma=(\gamma^++\gamma^-)/2$ and $\delta=(\gamma^+-\gamma^-)/2$. Then

$$
\mathcal J(z)=e^{-\gamma z}
\begin{pmatrix}\cosh(\delta z)&-i\sinh(\delta z)\\i\sinh(\delta z)&\cosh(\delta z)\end{pmatrix}
=e^{-Kz},\qquad K=\begin{pmatrix}\gamma&i\delta\\-i\delta&\gamma\end{pmatrix}.
$$

The sum of the two modal exponentials supplies a hyperbolic cosine, not its reciprocal. The [determinant](multilinear-algebra.md#determinant) is $e^{-2\gamma z}$, and $\mathcal J(z_1+z_2)=\mathcal J(z_1)\mathcal J(z_2)$. Real modal coefficients give [circular dichroism](stereochemistry.md#circular-dichroism); purely imaginary coefficients give lossless [circular birefringence](maxwell-equations.md#circular-birefringence). Complex modal labels do not have an intrinsic numerical ordering.

#### Jones vector

↑ **Parent:** [Jones calculus](#jones-calculus)

A [Jones vector](#jones-vector) records the two transverse [complex amplitudes](#complex-amplitude) of a completely polarized [monochromatic wave](#monochromatic-wave). Multiplication by a common nonzero complex number preserves its [polarization of waves](#polarization-waves), while changing overall amplitude and phase. With the convention $\boldsymbol\Psi(t)=\operatorname{Re}[\mathbf J e^{i\omega t}]$, $\mathbf J=(1,2i)^{\mathsf T}$ gives $(\cos\omega t,-2\sin\omega t)$, an [ellipse](euclidean-geometry.md#ellipse) with the longer axis along $y$. Handedness labels require both a viewing direction and a naming convention.

##### Jones-component ratio sensitivity

↑ **Parent:** [Jones vector](#jones-vector)

For a differentiable [Jones vector](#jones-vector) with $J_x(0)\ne0$, the ratio $r=J_y/J_x$ fixes [polarization](#polarization-waves) independently of common [amplitude](#wave-amplitude) and [phase](#phase-waves). The title quotient derivative tests first-order [polarization](#polarization-waves) sensitivity. If $\mathbf J'(0)=a\mathbf J(0)$ for a complex scalar $a$, then $r'(0)=0$. For a lossless normalized output, differentiation of $\mathbf J^\dagger\mathbf J=1$ makes $\operatorname{Re}a=0$, so this change is a common [phase](#phase-waves). A vanishing component requires the complementary ratio or a basis-independent [polarization](#polarization-waves) coordinate instead.

### Elliptical polarization

↑ **Parent:** [Polarization (waves)](#polarization-waves)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elliptical_polarization)

For an [elliptically polarized wave](#elliptical-polarization), the tip of its transverse [vector](vector-space.md#vector) traces an [ellipse](euclidean-geometry.md#ellipse) at a fixed point during each [wave period](#wave-period). For [polarization of an electromagnetic wave](electromagnetic-wave.md#polarization-of-an-electromagnetic-wave), this is the [electric field](electric-field.md) [vector](vector-space.md#vector). With the real components in [polarization of waves](#polarization-waves), assume $A_x,A_y>0$ and $\sin\delta\neq0$. Eliminating time gives

$$
\frac{E_x^2}{A_x^2}+\frac{E_y^2}{A_y^2}-\frac{2E_xE_y}{A_xA_y}\cos\delta=\sin^2\delta.
$$

A short derivation uses $\phi=\omega t$ and the [cosine](geometry-and-topology.md#cosine) addition formula to obtain $E_y/A_y=(E_x/A_x)\cos\delta-\sin\phi\sin\delta$; squaring and using the [sine](geometry-and-topology.md#sine) and [cosine](geometry-and-topology.md#cosine) identity $\sin^2\phi=1-\cos^2\phi$ gives the displayed equation. Outside [phase quadrature](#phase-quadrature), the mixed term gives a tilted [ellipse](euclidean-geometry.md#ellipse); $A_x,A_y$ are component [wave amplitudes](#wave-amplitude) and need not be its [semi-major and semi-minor axes](euclidean-geometry.md#semi-major-and-semi-minor-axes).

In [phase quadrature](#phase-quadrature), $\delta=\pm\pi/2$, the mixed term vanishes. For $(A_x,A_y)=(2,1)\,\mathrm{V/m}$, the [ellipse](euclidean-geometry.md#ellipse) is $E_x^2/4+E_y^2=1$, its [semi-major and semi-minor axes](euclidean-geometry.md#semi-major-and-semi-minor-axes) have lengths $2$ and $1\,\mathrm{V/m}$, and its [electric field](electric-field.md) magnitude varies between $1$ and $2\,\mathrm{V/m}$. At $\phi=\pi/4$ with $\delta=\pi/2$, the [electric field](electric-field.md) is $(\sqrt2,-1/\sqrt2)\,\mathrm{V/m}$ and has magnitude $\sqrt{5/2}\,\mathrm{V/m}$. Equal [wave amplitudes](#wave-amplitude) instead give [circular polarization](electromagnetic-wave.md#circular-polarization), a special case of [elliptical polarization](#elliptical-polarization) with constant magnitude. As $\delta$ approaches $0$ or $\pi$, the [ellipse](euclidean-geometry.md#ellipse) collapses to a [line segment](convex-set.md#line-segment) and gives [linear polarization](electromagnetic-wave.md#linear-polarization); this limit is degenerate rather than a nondegenerate [ellipse](euclidean-geometry.md#ellipse).

Changing $\delta$ from $\pi/2$ to $-\pi/2$ reverses traversal of the same [ellipse](euclidean-geometry.md#ellipse). In the displayed $x,y$ plot, $\delta=\pi/2$ moves from $(A_x,0)$ toward negative $y$ as time increases. A label such as right- or left-handed [circular polarization](electromagnetic-wave.md#circular-polarization) additionally requires a stated viewing direction and naming convention: viewing along propagation and viewing against propagation reverse the apparent rotation. [Feynman Lectures, I §33–1: polarization conventions](https://www.feynmanlectures.caltech.edu/I_33.html#Ch33-S1).

The [ellipse](euclidean-geometry.md#ellipse) records both the relative [wave amplitudes](#wave-amplitude) and the [phase difference](#phase-difference) of two transverse [oscillations](#oscillation). This separates a change of [polarization of waves](#polarization-waves) from a change of overall [wave amplitude](#wave-amplitude): multiplying both components by the same positive factor enlarges the [ellipse](euclidean-geometry.md#ellipse) while preserving its shape and orientation.

A rotating ideal linear [polarizer](electromagnetic-wave.md#polarizer) can probe this geometry. For the $2:1$ [ellipse](euclidean-geometry.md#ellipse) in [phase quadrature](#phase-quadrature), [orthogonal projection](hilbert-space.md#orthogonal-projection) onto a pass axis at [angle](geometry-and-topology.md#angle) $\theta$ gives $E_{\mathrm{out}}(t)=2\cos\theta\cos\omega t-\sin\theta\sin\omega t$, in $\mathrm{V/m}$. Averaging its square over a [wave period](#wave-period) gives $(4\cos^2\theta+\sin^2\theta)/2$, while the incoming squared [electric field](electric-field.md) magnitude averages to $5/2$. Thus the transmitted fraction of [light intensity](#light-intensity) is $(4\cos^2\theta+\sin^2\theta)/5$: it is $4/5$ at $0^\circ$, $1/2$ at $45^\circ$ and $1/5$ at $90^\circ$. There is no single incident line of [linear polarization](electromagnetic-wave.md#linear-polarization) to insert into [Malus's law](#malus-s-law); projecting the [electric field](electric-field.md) and averaging its square is the appropriate generalization. This measurement cannot distinguish $\delta=\pi/2$ from $\delta=-\pi/2$, because reversing the traversal leaves all these squared averages unchanged.

#### Elliptical polarization from circular and linear components

↑ **Parent:** [Elliptical polarization](#elliptical-polarization)

Two coherent waves with common propagation direction and [frequency](#frequency) can combine into a [polarization ellipse](#polarization-ellipse). Take circular components $E_x=A\cos\psi$, $E_y=A\sin\psi$ and add $B\cos\psi$ along $x$. The resulting semiaxes are $|A+B|$ and $|A|$. Choosing positive $A,B$ gives a nondegenerate ellipse with unequal axes. Uncorrelated relative phases do not describe the same fixed pure polarization.

#### Polarization ellipse

↑ **Parent:** [Elliptical polarization](#elliptical-polarization)

The [polarization ellipse](#polarization-ellipse) is the curve traced by the transverse [electric field](electric-field.md) of a monochromatic wave at a fixed point. Its orientation and signed ratio of minor to major semiaxis specify a [pure polarization](#pure-polarization). A zero minor semiaxis gives [linear polarization](electromagnetic-wave.md#linear-polarization), and equal semiaxes give [circular polarization](electromagnetic-wave.md#circular-polarization).

<h3 id="malus-s-law">Malus's law</h3>

↑ **Parent:** [Polarization (waves)](#polarization-waves)

For incident [light](optics.md#light) with [linear polarization](electromagnetic-wave.md#linear-polarization), an ideal linear [polarizer](electromagnetic-wave.md#polarizer) transmits

$$
I_{\mathrm{out}}=I_{\mathrm{in}}\cos^2\theta,
$$

where $I$ is [light intensity](#light-intensity) and $\theta$ is the [angle](geometry-and-topology.md#angle) between the incident [electric field](electric-field.md)'s line of [oscillation](#oscillation) and the [polarizer](electromagnetic-wave.md#polarizer)'s pass axis. The input and output are compared in the same medium. The classical explanation is an [orthogonal projection](hilbert-space.md#orthogonal-projection): for a [unit vector](vector-space.md#unit-vector) $\mathbf u$ along the pass axis,

$$
\mathbf E_{\mathrm{out}}=(\mathbf E_{\mathrm{in}}\mathbin{\cdot}\mathbf u)\mathbf u.
$$

The [dot product](inner-product.md#dot-product) reduces the transmitted [wave amplitude](#wave-amplitude) by $\cos\theta$. For a [plane electromagnetic wave](electromagnetic-wave.md#plane-electromagnetic-wave) in the same medium, [light intensity](#light-intensity) is proportional to squared [electric field](electric-field.md) [wave amplitude](#wave-amplitude), giving [Malus's law](#malus-s-law). For example, $\theta=60^\circ$ transmits one quarter of the incident [light intensity](#light-intensity), although the transmitted [wave amplitude](#wave-amplitude) is one half. [Feynman Lectures, I §33–4: polarizers](https://www.feynmanlectures.caltech.edu/I_33.html#Ch33-S4).

Start with [light](optics.md#light) already in [linear polarization](electromagnetic-wave.md#linear-polarization) along the horizontal $0^\circ$ axis and let its [light intensity](#light-intensity) be $I_0$. Two ideal absorbing linear [polarizers](electromagnetic-wave.md#polarizer) with pass axes $0^\circ$ and $90^\circ$ give $I_0\cos^2 0^\circ\cos^2 90^\circ=0$. Insert a $45^\circ$ [polarizer](electromagnetic-wave.md#polarizer) between them: the first leaves $I_0$ unchanged, the middle transmits $I_0/2$ with [linear polarization](electromagnetic-wave.md#linear-polarization) along $45^\circ$, and the last transmits $I_0/4$ with [linear polarization](electromagnetic-wave.md#linear-polarization) along $90^\circ$. Each [angle](geometry-and-topology.md#angle) in [Malus's law](#malus-s-law) is relative to the preceding output, so the final step uses $90^\circ-45^\circ=45^\circ$:

$$
I_{\mathrm{out}}=I_0\cos^2 0^\circ\cos^2 45^\circ\cos^2(90^\circ-45^\circ)=\frac{I_0}{4}.
$$

<a id="image-two-crossed-polarizers-transmit-zero-inserting-a-middle-polarizer-transmits-i-0-4-for-initially-horizontal-linear-polarization"></a>
![](polarization-through-three-filters.png)

**[Figure 2](#image-two-crossed-polarizers-transmit-zero-inserting-a-middle-polarizer-transmits-i-0-4-for-initially-horizontal-linear-polarization). Two crossed polarizers transmit zero; inserting a middle polarizer transmits $I_0/4$ for initially horizontal linear polarization**. Pass axes are measured from horizontal. Each blue segment represents transmitted [light intensity](#light-intensity), and each inset shows the pass axis in the transverse plane. The two successive $45^\circ$ changes each halve [light intensity](#light-intensity) by [Malus's law](#malus-s-law).

For these ideal absorbing [polarizers](electromagnetic-wave.md#polarizer), the rejected [electric field](electric-field.md) component transfers [energy](energy.md) to the filter. In the three-filter arrangement the middle absorbs the fraction $I_0/2$, and the last absorbs $I_0/4$, leaving $I_0/4$ transmitted. [Conservation of energy](mathematical-physics.md#conservation-of-energy) holds at each step. Inserting the middle [polarizer](electromagnetic-wave.md#polarizer) changes the [linear polarization](electromagnetic-wave.md#linear-polarization) arriving at the last one; it does not create [light](optics.md#light). The effect illustrates why successive [orthogonal projections](hilbert-space.md#orthogonal-projection) cannot generally be replaced by a single comparison of the first and last axes.

The initially horizontal assumption matters. For [unpolarized light](#unpolarized-light) of [light intensity](#light-intensity) $I_0$, the first ideal linear [polarizer](electromagnetic-wave.md#polarizer) transmits $I_0/2$: averaging $\cos^2\theta$ over uniformly distributed incident orientations gives $1/2$. The same $0^\circ,45^\circ,90^\circ$ sequence then transmits $I_0/8$. This extra first-stage factor does not apply to the already horizontally polarized input in the figure.

#### Transmission through a sequence of linear polarizers

↑ **Parent:** [Malus's law](#malus-s-law)

For ideal [polarizers](electromagnetic-wave.md#polarizer) with successive transverse transmission directions $\theta_j$, the [Jones matrix](#jones-matrix) is the rank-one [orthogonal projection](hilbert-space.md#orthogonal-projection) $P_j=\mathbf u_j\mathbf u_j^{\mathsf T}$. The identity $\mathbf u_j^{\mathsf T}\mathbf u_{j-1}=\cos(\theta_j-\theta_{j-1})$ reduces the transmitted [probability amplitude](wave-function.md#probability-amplitude) analogue, here the optical [complex amplitude](#complex-amplitude), to a product of projections. For [unpolarized light](#unpolarized-light), the first element transmits half the incident [light intensity](#light-intensity), giving the displayed product. For a specified incident [linear polarization](electromagnetic-wave.md#linear-polarization), replace the first half-factor with its actual projection.

### Unpolarized light

↑ **Parent:** [Polarization (waves)](#polarization-waves)

[Unpolarized light](#unpolarized-light) has no preferred transverse polarization direction in its time-averaged statistics. An ideal linear [polarizer](electromagnetic-wave.md#polarizer) transmits half its incident [light intensity](#light-intensity): equal transverse components give the averaged projection factor $\langle\cos^2\theta\rangle=1/2$. This statistical description differs from the fixed deterministic phase relation of a [monochromatic wave](#monochromatic-wave) in a pure [polarization of waves](#polarization-waves) state.

## Oscillation

↑ **Parent:** [Wave](wave.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Oscillation)

An oscillation is a repeated variation about an equilibrium or central value. A [normal mode](wave-equation.md#normal-mode) describes a single frequency of oscillation.

### Oscillator

↑ **Parent:** [Oscillation](#oscillation)

#### Coupled oscillator

↑ **Parent:** [Oscillator](#oscillator)

[Coupled oscillators](#coupled-oscillator) exchange [energy](energy.md) through interactions. Linear equations can be transformed into [normal mode coordinates](classical-mechanics.md#normal-coordinate); the spatial pattern of an applied [force](force.md) determines which [normal modes](wave-equation.md#normal-mode) are driven.

##### Three coupled pendulums with equal end masses

↑ **Parent:** [Coupled oscillator](#coupled-oscillator)

For equal lengths, end masses $m$, middle mass $M$, and equal springs between adjacent bobs, [reflection symmetry](physics.md#reflection-symmetry) gives mode [vectors](vector-space.md#vector) $(1,1,1)$, $(1,0,-1)$ and $(1,-2m/M,1)$. Their squared frequencies are displayed above. These [vectors](vector-space.md#vector) are orthogonal in the [inner product](inner-product.md) weighted by $\operatorname{diag}(m,M,m)$. Equal end masses, rather than equality of all three masses, suffice for this [symmetry](physics.md#symmetry-physics) reduction.

###### End-displacement release of three coupled pendulums

↑ **Parent:** [Three coupled pendulums with equal end masses](#three-coupled-pendulums-with-equal-end-masses)

##### Absolute and signed beat envelopes

↑ **Parent:** [Coupled oscillator](#coupled-oscillator)

For $x_2=(a/2)[\cos\omega_1t-\cos\omega_2t]$, the slowly varying signed factor is $a\sin[(\omega_2-\omega_1)t/2]$. The absolute amplitude envelope repeats in $2\pi/|\omega_2-\omega_1|$, half the period of that signed factor.

##### Normal modes of two spring-coupled equal pendulums

↑ **Parent:** [Coupled oscillator](#coupled-oscillator)

Two equal small-angle pendulums coupled by a spring have displacement patterns $(1,1)$ and $(1,-1)$, with squared angular frequencies $g/l$ and $g/l+2k/m$. An initial displacement of only the first pendulum excites both patterns equally.

### Anharmonicity

↑ **Parent:** [Oscillation](#oscillation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Anharmonicity)

[Anharmonicity](#anharmonicity) is departure from the motion of a [harmonic oscillator](classical-mechanics.md#simple-harmonic-motion), often caused by nonquadratic terms in a [potential energy](energy.md#potential-energy). It can make the [oscillation](#oscillation) [frequency](#frequency) depend on [amplitude](#wave-amplitude) and generate higher harmonics. A [quartic oscillator](classical-mechanics.md#quartic-oscillator) has one such anharmonic [potential energy](energy.md#potential-energy).

## Wave period

↑ **Parent:** [Wave](wave.md)

A wave period is the time for a monochromatic [wave](wave.md) to complete one oscillation. For angular [frequency](#frequency) $\omega$, it is $2\pi/|\omega|$. In cascade order-of-magnitude estimates the factor $2\pi$ is normally suppressed, giving a linear interaction time of order $|\omega|^{-1}$.

## Angular spectrum

↑ **Parent:** [Wave](wave.md)

The angular spectrum is the transverse [Fourier transform](fourier-transform.md) of a monochromatic field on a reference plane. In a uniform medium, each transverse [wavevector](elasticity-physics.md#wavevector) component propagates with a longitudinal wavenumber satisfying the [Helmholtz equation](partial-differential-equation.md#helmholtz-equation). Components beyond the propagating wavenumber range are [evanescent waves](elasticity-physics.md#evanescent-wave). The [outgoing angular spectrum](physics.md#outgoing-angular-spectrum) chooses the longitudinal branch that propagates or decays away from the plane.

## Wave focusing

↑ **Parent:** [Wave](wave.md)

## Wave amplitude

↑ **Parent:** [Wave](wave.md)

### Peak-to-peak amplitude

↑ **Parent:** [Wave amplitude](#wave-amplitude)

### Scalar wave intensity

↑ **Parent:** [Wave amplitude](#wave-amplitude)

For a scalar complex [wave amplitude](#wave-amplitude) $E$, the squared-amplitude [scalar wave intensity](#scalar-wave-intensity) convention is $I=EE^*$. It is nonnegative and unchanged by multiplying $E$ by a unit-modulus [wave phase](#phase-waves) factor. This convention is useful in [paraxial propagation](partial-differential-equation.md#paraxial-approximation) and [phase screen](partial-differential-equation.md#phase-screen) models. Conversion to physical [energy flux](mathematical-physics.md#energy-flux) also depends on the field variable and medium; an arbitrary superposition need not have its full flux determined by this scalar alone. For a random field, $\langle I\rangle$ is the [mean wave intensity](#ensemble-averaged-wave-intensity), whereas $|\langle E\rangle|^2$ is the squared [coherent field](#coherent-wave-field); these generally differ.

### Complex amplitude

↑ **Parent:** [Wave amplitude](#wave-amplitude)

A [complex number](complex-analysis.md#complex-number) can encode both the [wave amplitude](#wave-amplitude) and phase of a harmonic disturbance: $a(x,t)=\operatorname{Re}\{\hat a e^{i(kx-\omega t)}\}$. Its [modulus](complex-analysis.md#modulus) is the real oscillation amplitude and its [complex argument](complex-analysis.md#argument-complex-analysis) fixes the [wave phase](#phase-waves).

#### Phase convention for complex amplitudes

↑ **Parent:** [Complex amplitude](#complex-amplitude)

Reference [wave phases](#phase-waves) label [complex amplitudes](#complex-amplitude) without changing measured [powers](energy.md#power). If $\mathbf b=S\mathbf a$, choose [diagonal matrices](linear-algebra.md#diagonal-matrix) $D_{\rm in},D_{\rm out}$ whose entries have [modulus](complex-analysis.md#modulus) one, and set $\mathbf a^{\prime}=D_{\rm in}\mathbf a$, $\mathbf b^{\prime}=D_{\rm out}\mathbf b$. Then $S^{\prime}=D_{\rm out}SD_{\rm in}^{-1}$ and each component has unchanged squared [modulus](complex-analysis.md#modulus). For a [beam splitter scattering matrix](optical-instrument.md#beam-splitter-scattering-matrix), transforming $S$ without transforming input [complex amplitudes](#complex-amplitude) changes the stated physical input.

#### Phasor

↑ **Parent:** [Complex amplitude](#complex-amplitude)

A [phasor](#phasor) is a [complex amplitude](#complex-amplitude) representing a [sinusoid](geometry-and-topology.md#sinusoid) at one specified [angular frequency](lagrangian-mechanics.md#angular-frequency): $a(t)=\operatorname{Re}(\widehat A e^{\mathrm i\omega t})$. Its [modulus](complex-analysis.md#modulus) gives the peak [amplitude](#wave-amplitude) and its [complex argument](complex-analysis.md#argument-complex-analysis) gives the [wave phase](#phase-waves) in this convention. Both may instead use [root mean square](analysis.md#root-mean-square) magnitudes if that normalization is stated.

## Phase (waves)

↑ **Parent:** [Wave](wave.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phase_(waves))

### Phase shift

↑ **Parent:** [Phase (waves)](#phase-waves)

A [phase shift](#phase-shift) is a change in an oscillation's [wave phase](#phase-waves), specified modulo $2\pi$. It can arise from propagation, reflection or an imposed response. With the time convention $e^{-i\omega t}$, a delay $\tau$ multiplies the [complex amplitude](#complex-amplitude) by $e^{i\omega\tau}$. A sign reversal is a $\pi$ [phase shift](#phase-shift).

### Phase factor

↑ **Parent:** [Phase (waves)](#phase-waves)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phase_factor)

A [phase factor](#phase-factor) is a unit-modulus [complex number](complex-analysis.md#complex-number) $e^{i\phi}$. Multiplying a [complex amplitude](#complex-amplitude) by it changes its [wave phase](#phase-waves) by $\phi$ while preserving its squared [modulus](complex-analysis.md#modulus). A common [phase factor](#phase-factor) does not change [light intensity](#light-intensity), while different [phase factors](#phase-factor) of contributions can change their [interference](physical-optics.md#interference-wave-propagation).

### Phase difference

↑ **Parent:** [Phase (waves)](#phase-waves)

The difference of two [wave phases](#phase-waves) at the same place and time, considered modulo $2\pi$. It determines whether two same-frequency [oscillations](#oscillation) reinforce, cancel, or are in [phase quadrature](#phase-quadrature).

### Phase quadrature

↑ **Parent:** [Phase (waves)](#phase-waves)

Two sinusoidal signals are in phase quadrature when their [phase difference](#phase-difference) is a quarter cycle, for example $\cos\phi$ and $\sin\phi$. Their time averages have zero [correlation](variance.md#pearson-correlation-coefficient) over a cycle. In a [plane wave](wave-function.md#plane-wave), this separates fields such as [displacement](classical-mechanics.md#displacement) and its time [derivative](calculus.md#derivative), [velocity](classical-mechanics.md#velocity).

## Wave absorption

↑ **Parent:** [Wave](wave.md)

[Wave absorption](#wave-absorption) transfers [energy](energy.md) from a propagating [wave](wave.md) to other [degrees of freedom](classical-mechanics.md#degree-of-freedom) of a medium. For a [plane wave](wave-function.md#plane-wave) that is a [monochromatic wave](#monochromatic-wave), with amplitude proportional to $e^{i(k'+ik'')z}$ and $k''>0$, its [wave intensity](#intensity-physics) decreases as $I(z)=I(0)e^{-2k''z}$. The intensity absorption coefficient is therefore $2k''$ when this loss is due to absorption. A decreasing transmitted [wave intensity](#intensity-physics) can also result from [wave reflection](#wave-reflection) or [wave scattering](#wave-scattering), which redistribute [energy](energy.md) rather than necessarily converting it into [heat](heat.md).

## Wave reflection

↑ **Parent:** [Wave](wave.md)

[Wave reflection](#wave-reflection) returns part of an incident [wave](wave.md) into the medium from which it arrived, as a consequence of an interface or spatial variation of material properties. An amplitude [reflection coefficient](partial-differential-equation.md#reflection-coefficient) compares the reflected and incident [waves](wave.md); its squared [modulus](complex-analysis.md#modulus) gives their [wave intensity](#intensity-physics) ratio when both use the same medium and normalization. Reflected [energy](energy.md) has not necessarily undergone [wave absorption](#wave-absorption).

## Multipath propagation

↑ **Parent:** [Wave](wave.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multipath_propagation)

## Wave reciprocity

↑ **Parent:** [Wave](wave.md)

In a reciprocal medium, appropriately normalized source and receiver responses can be exchanged: the scalar [Green function](green-s-function.md) satisfies $G(\mathbf r,\mathbf r')=G(\mathbf r',\mathbf r)$. Reciprocity alone does not imply absence of [wave absorption](#wave-absorption).

### Weighted acoustic Green-function reciprocity

↑ **Parent:** [Wave reciprocity](#wave-reciprocity)

For an operator $c^{-2}\partial_t^2-a^{-1}\nabla\cdot(a\nabla)$ with positive stationary coefficients and reciprocal boundary conditions, its delta-normalized [Green function](green-s-function.md) satisfies

$$
a(x)G(x,y;s)=a(y)G(y,x;s).
$$

Multiplying its frequency-domain equation by $a$ and using the bilinear [Green second identity](partial-differential-equation.md#green-second-identity) proves the relation. Both Green functions must use the same outgoing or causal prescription. Exchanging source and receiver preserves time lag, and involves no complex conjugation.

## Time-harmonic wave

↑ **Parent:** [Wave](wave.md)

## Wave scattering

↑ **Parent:** [Wave](wave.md)

### Scattered wave

↑ **Parent:** [Wave scattering](#wave-scattering)

The [scattered wave](#scattered-wave) is the part of the total solution produced by the scatterer relative to the prescribed [incident wave](#incident-wave). It obeys an outgoing radiation condition. For a rough reflecting surface, this convention includes both specular flat-surface reflection and the roughness-dependent correction. Its [coherent field](#coherent-wave-field) is its ensemble mean, which need not equal the full mean intensity.

### Incident wave

↑ **Parent:** [Wave scattering](#wave-scattering)

The [incident wave](#incident-wave) is the prescribed background solution that illuminates a scatterer. It solves the unperturbed [Helmholtz equation](partial-differential-equation.md#helmholtz-equation) in scalar time-harmonic models. The scattered contribution is defined by subtracting this field from the total field; reflected waves from a planar boundary are included unless a separate reference reflection is explicitly removed.

### Differential cross-section for scalar wave scattering

↑ **Parent:** [Wave scattering](#wave-scattering)

If a unit incident [plane wave](wave-function.md#plane-wave) has scattered field $\psi_s=e^{ikR}f_\infty(\widehat{\mathbf r},\widehat{\mathbf r}_0)/R+O(R^{-2})$, the differential wave scattering cross-section is

$$
 \frac{d\sigma}{d\Omega}=|f_\infty(\widehat{\mathbf r},\widehat{\mathbf r}_0)|^2.
$$

It is the far-field limit of $R^2$ times the scattered-to-incident [energy flux](mathematical-physics.md#energy-flux) ratio. The common physical amplitude normalization cancels when the incident and scattered waves are in the same background medium. The formula assumes that the $1/(4\pi)$ Green-function factor, if present, is already included in the [far-field pattern](inverse-problem.md#far-field-pattern).

#### Finite-volume random scattering spectrum

↑ **Parent:** [Differential cross-section for scalar wave scattering](#differential-cross-section-for-scalar-wave-scattering)

In the [Born approximation for scalar wave scattering](inverse-problem.md#born-approximation-for-scalar-wave-scattering), with $n=1+\mu W$ and zero-mean stationary unit-variance $W$, define $S_W(\mathbf q)=\int C(\mathbf s)e^{-i\mathbf q\cdot\mathbf s}d^3s$. The leading [expectation](expected-value.md) of the [differential cross-section for scalar wave scattering](#differential-cross-section-for-scalar-wave-scattering) is

$$
 \langle\sigma_d\rangle=\frac{\mu^2k^4}{4\pi^2}\int C(\mathbf s)|V\cap(V-\mathbf s)|e^{-i\mathbf k_s\cdot\mathbf s}\,d^3s+O(\mu^3),
 \quad\mathbf k_s=k(\widehat{\mathbf r}-\widehat{\mathbf r}_0).
$$

For a regular volume much larger than the covariance range, the overlap is approximately $|V|$, giving $\mu^2k^4|V|S_W(\mathbf k_s)/(4\pi^2)$. [Statistical isotropy](probability-and-statistics.md#statistical-isotropy), beyond [statistical homogeneity](probability-and-statistics.md#statistical-homogeneity), permits the scalar argument $|\mathbf k_s|=2k\sin(\theta/2)$. If the spectrum is defined for the index fluctuation rather than $W$, it already contains $\mu^2$.

### Random medium

↑ **Parent:** [Wave scattering](#wave-scattering)

#### Wave propagation in a random medium

↑ **Parent:** [Random medium](#random-medium)

##### Anderson localization

↑ **Parent:** [Wave propagation in a random medium](#wave-propagation-in-a-random-medium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Anderson_localization)

[Anderson localization](#anderson-localization) is the confinement of [electron](physics.md#electron) [wave functions](wave-function.md), or other [wave](wave.md) modes, by [interference](physical-optics.md#interference-wave-propagation) between repeated [wave scattering](#wave-scattering) paths in static disorder. A [localized eigenstate](#localized-eigenstate) occupies a limited region even in a much larger sample. Disorder can therefore suppress [diffusion](thermodynamics.md#diffusion) without absorbing the [wave](wave.md). In 1958, [Philip Warren Anderson](physicist.md#philip-warren-anderson) studied random site [energies](energy.md) and intersite coupling, finding a regime without transport. His paper develops a theoretical model; it does not report an Anderson laboratory measurement.[Anderson, 1958, pp.1492–1494, Sections I–II](physics-bibliography.md#absence-of-diffusion-in-certain-random-lattices-by-philip-warren-anderson)

The distinction from ordinary [multiple scattering](#multiple-scattering) is the retention of [wave phases](#phase-waves): alternative paths contribute [probability amplitudes](wave-function.md#probability-amplitude) before their squared [modulus](complex-analysis.md#modulus) is taken. Adding path probabilities alone loses the cross terms responsible for [interference](physical-optics.md#interference-wave-propagation). This makes [Anderson localization](#anderson-localization) useful as a warning about transport models: repeated deflections need not produce unlimited [diffusion](thermodynamics.md#diffusion). It also connects [electron](physics.md#electron) transport with [wave propagation in a random medium](#wave-propagation-in-a-random-medium), although the detailed equations and experimental diagnostics differ between [electrons](physics.md#electron), [light](optics.md#light) and [acoustic waves](fluid-mechanics.md#acoustic-wave).

[Philip Warren Anderson](physicist.md#philip-warren-anderson)'s 1977 lecture distinguishes localized magnetic moments from disorder-localized states. It credits [Nevill Francis Mott](physicist.md#nevill-francis-mott) with recognizing the significance of the [mobility edge](#mobility-edge). A [Mott insulator](bloch-s-theorem.md#mott-insulator) instead requires [electron](physics.md#electron) interactions and can exist without disorder.[Local Moments and Localized States, pp.376–377,395–396; inspected institutional mirror [https://www.nevis.columbia.edu/~haas/documents/physics_nobel_lectures/physics71-80-2.pdf](https://www.nevis.columbia.edu/~haas/documents/physics_nobel_lectures/physics71-80-2.pdf)](physics-bibliography.md#local-moments-and-localized-states-by-philip-warren-anderson)

[John Hasbrouck Van Vleck](physicist.md#john-hasbrouck-van-vleck) developed [quantum mechanics](quantum-mechanics.md) explanations of [magnetic susceptibility](statistical-physics.md#magnetic-susceptibility), including its [temperature](temperature.md) dependence; this is a distinct contribution from [Anderson localization](#anderson-localization).[Quantum Mechanics: The Key to Understanding Magnetism, pp.355–356; inspected institutional mirror [https://www.nevis.columbia.edu/~haas/documents/physics_nobel_lectures/physics71-80-2.pdf](https://www.nevis.columbia.edu/~haas/documents/physics_nobel_lectures/physics71-80-2.pdf)](physics-bibliography.md#quantum-mechanics-the-key-to-understanding-magnetism-by-john-hasbrouck-van-vleck)

###### Weak localization

↑ **Parent:** [Anderson localization](#anderson-localization)

Interference of time-reversed multiple-scattering paths can enhance return probability and reduce conductance in a coherent disordered conductor with the appropriate symmetries. Magnetic fields, spin-orbit coupling and dephasing alter or suppress the correction; some symmetry classes exhibit antilocalization. This small-correction regime must be distinguished from strong [Anderson localization](#anderson-localization).

###### Mobility gap

↑ **Parent:** [Anderson localization](#anderson-localization)

An [energy](energy.md) interval with no extended bulk [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) available for transport. It can contain [localized eigenstates](#localized-eigenstate) and have a nonzero [density of states](quantum-ideal-gas-statistics.md#density-of-states); a [mobility gap](#mobility-gap) need not be a [spectral gap](linear-operator-theory.md#spectral-gap).

###### Localized eigenstate

↑ **Parent:** [Anderson localization](#anderson-localization)

A [localized eigenstate](#localized-eigenstate) is an [energy eigenstate](energy-eigenvalue.md#energy-eigenstate) whose spatial weight remains concentrated near some position as the system grows. An exponentially [localized eigenstate](#localized-eigenstate) has a decaying envelope characterized by a [localization length](#localization-length). A small [participation ratio](#participation-ratio) measures concentration in a chosen site basis; it does not by itself establish an exponential tail or a transport law.

An [energy eigenstate](energy-eigenvalue.md#energy-eigenstate) changes only by an overall [wave phase](#phase-waves) under time evolution, whether localized or extended. Its stationary probability distribution alone therefore does not distinguish transport mechanisms. The important distinction concerns spatial extent and how superpositions of [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) carry or retain a disturbance. A wave packet assembled from [localized eigenstates](#localized-eigenstate) with nearby centres can remain confined, whereas extended modes can support propagation.

###### Localization length

↑ **Parent:** [Localized eigenstate](#localized-eigenstate)

The [localization length](#localization-length) $\xi$ measures the decay scale of a [localized eigenstate](#localized-eigenstate)'s [wave amplitude](#wave-amplitude) envelope. Here $a$ is the site spacing and $n_0$ its centre. With this amplitude convention, probability decays on half that scale:

$$
|\psi_n|\sim e^{-|n-n_0|a/\xi},\qquad |\psi_n|^2\sim e^{-2|n-n_0|a/\xi}.
$$

Individual random tails fluctuate; this notation describes their typical envelope, not exact equality at every site. A [localization length](#localization-length) much greater than a finite sample's [length](physics.md#length) makes a state look extended inside that sample. The [participation ratio](#participation-ratio) below is an effective site count, not an independent fitted value of $\xi$.

###### Participation ratio

↑ **Parent:** [Localized eigenstate](#localized-eigenstate)

For an [eigenvector](linear-operator-theory.md#eigenvector) normalized by $\sum_{n=1}^N|\psi_n|^2=1$, the [participation ratio](#participation-ratio) in its site basis is

$$
P=\frac{1}{\sum_{n=1}^N|\psi_n|^4},\qquad 1\leq P\leq N.
$$

It estimates how many sites carry appreciable probability. Equal weight on $K$ sites and zero elsewhere gives $P=K$, irrespective of their [wave phases](#phase-waves). A single occupied site gives $P=1$; uniform probability on all sites gives $P=N$. These are exact constructed examples, not claims about particular [Hamiltonian operators](quantum-system.md#hamiltonian-quantum-mechanics).

To prove the bounds, write $p_n=|\psi_n|^2$. Since $0\leq p_n\leq1$, $\sum_np_n^2\leq\sum_np_n=1$, giving $P\geq1$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $1=(\sum_np_n)^2\leq N\sum_np_n^2$, giving $P\leq N$. Thus the measure has useful limits without assuming an exponential shape. Comparing $P$ as $N$ increases helps distinguish a state filling the sample from one occupying a fixed region, provided [energy](energy.md) selection and disorder statistics are controlled.

###### Mobility edge

↑ **Parent:** [Anderson localization](#anderson-localization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mobility_edge)

A [mobility edge](#mobility-edge) separates localized from extended [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) on the [energy](energy.md) axis. Three-dimensional disordered models can have both. In the infinite one-dimensional [tight-binding model](bloch-s-theorem.md#tight-binding) with independent continuous random site [energies](energy.md), all states are localized for any nonzero disorder, with probability one. This statement excludes specially correlated disorder.[Local Moments and Localized States, pp.395–396, mobility edge and one-dimensional localization; institutional mirror as above](physics-bibliography.md#local-moments-and-localized-states-by-philip-warren-anderson)

A [mobility edge](#mobility-edge) is not a [band gap](bloch-s-theorem.md#band-gap): states can exist on both sides of $E_c$, but differ in spatial extent. For [electrons](physics.md#electron), the location of the [Fermi energy](quantum-ideal-gas-statistics.md#fermi-energy) relative to a [mobility edge](#mobility-edge) matters for low-[temperature](temperature.md) [electrical conductivity](electric-charge.md#electrical-conductivity). A three-dimensional sample need not have an extended interval at every disorder strength. In particular, the finite one-dimensional calculations below neither locate a three-dimensional [mobility edge](#mobility-edge) nor establish a nonzero universal critical disorder.

###### One-dimensional Anderson chain

↑ **Parent:** [Anderson localization](#anderson-localization)

Consider a noninteracting [electron](physics.md#electron) in a finite [tight-binding model](bloch-s-theorem.md#tight-binding) with open ends:

$$
H=-t\sum_{n=1}^{N-1}\bigl(\lvert n\rangle\langle n+1\rvert+\lvert n+1\rangle\langle n\rvert\bigr)+\sum_{n=1}^N\epsilon_n\lvert n\rangle\langle n\rvert,\qquad t>0.
$$

The [vectors](vector-space.md#vector) $\lvert n\rangle$ form an [orthonormal basis](inner-product.md#orthonormal-basis) of site states. The hopping [energy](energy.md) is $t$; it is not the time coordinate. Draw each $\epsilon_n$ independently from the [continuous uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) on $[-W/2,W/2]$ and then hold it fixed. The disorder strength $W/t$ is dimensionless. Open ends mean no hopping bond connects sites $N$ and $1$; equivalently set $\psi_0=\psi_{N+1}=0$. There are no [electron](physics.md#electron) interactions, [phonons](quantum-ideal-gas-statistics.md#phonon) or [wave absorption](#wave-absorption) in this model.

The [eigenvalue equation](linear-operator-theory.md#eigenvalue-equation) in the interior is

$$
-t(\psi_{n-1}+\psi_{n+1})+\epsilon_n\psi_n=E\psi_n.
$$

As a simple local calculation, if a state's peak is at $n_0$, a neighbouring site with $|E-\epsilon_n|\gg t$ receives a small leading contribution $\psi_n\simeq-t\psi_{n_0}/(E-\epsilon_n)$. Several successive large mismatches multiply small factors. This explains why large disorder can restrict spreading, but is not a proof of [Anderson localization](#anderson-localization): near-resonant denominators and alternative [interference](physical-optics.md#interference-wave-propagation) paths prevent treating this expansion as uniformly valid.

For the first original calculation, take $N=80$, $t=1$, $W/t=6$ and the fixed random seed $20261015$. Diagonalizing the resulting real [symmetric matrix](linear-algebra.md#symmetric-matrix) with `numpy.linalg.eigh` and selecting the [eigenvalue](linear-operator-theory.md#eigenvalue) closest to zero gives $E/t\simeq-0.05962$, a probability peak at site $29$, and $P\simeq6.0031$. The selected [eigenvector](linear-operator-theory.md#eigenvector) has total probability one. This is one chosen realization, not a disorder average or a measured specimen.

<a id="anderson-chain-eigenstate"></a>
![](anderson-chain-eigenstate.png)

**[Figure 3](#anderson-chain-eigenstate). One random potential and a concentrated energy eigenstate in a One-dimensional Anderson chain**. Original calculation for $80$ sites and $W/t=6$. The top panel shows all site [energies](energy.md) and the selected [eigenvalue](linear-operator-theory.md#eigenvalue). The lower panels show the same probability on linear and logarithmic scales, compared with a clean central [standing wave](mathematical-physics.md#standing-wave). No fitted [localization length](#localization-length) is claimed.

The clean comparison needs care. With $W=0$, the open chain has [standing waves](mathematical-physics.md#standing-wave)

$$
\psi_n^{(m)}=\sqrt{\frac{2}{N+1}}\sin\frac{m\pi n}{N+1},\qquad E_m=-2t\cos\frac{m\pi}{N+1},\qquad m=1,\ldots,N.
$$

For even $N$, the identity $\sin^4x=(3-4\cos2x+\cos4x)/8$ and finite trigonometric sums give $\sum_n|\psi_n^{(m)}|^4=3/[2(N+1)]$, hence $P=2(N+1)/3$. Thus the clean $80$-site comparison has $P=54$, although it extends across the chain. Extended does not mean uniform probability. For odd $N$, the special central mode $m=(N+1)/2$ has zeros on alternating sites and instead $P=(N+1)/2$; the even-size assumption avoids that exception.

The second original calculation compares $N=40$ and $80$ over $W/t=0,0.5,1,2,3,4,6,8$. For each size, draw $24$ independent site patterns using seed $20261016$, with the size included in the random-seed construction. Scale each fixed pattern across disorder strengths. At every point, average $P$ over the four [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) closest to $E=0$. The solid line is the median across these sample averages; shading spans their $10$th–$90$th percentiles. The selected states can change as $W/t$ varies: lines connect one sample's selections rather than tracking a single mode.

<a id="anderson-participation-disorder"></a>
![](anderson-participation-disorder.png)

**[Figure 4](#anderson-participation-disorder). Participation ratio varies across disorder realizations and finite chain sizes**. Original [One-dimensional Anderson chain](#one-dimensional-anderson-chain) calculations. Faint lines show individual sample averages, solid lines their medians and bands their $10$th–$90$th percentiles. The left panel plots $P$; the right divides by site count $N$. These finite samples illustrate concentration and variability, without a fitted critical disorder.

At $W/t=0$ the two clean values are $27\frac13$ and $54$. At $W/t=8$, the computed median sample averages are approximately $3.17$ and $3.01$. In the latter regime, doubling $N$ hardly changes the typical occupied site count, so $P/N$ falls. At weak disorder the larger chain permits more spatial extent. Neither a single curve nor the overlap of finite-size bands proves the infinite-system statement under [mobility edge](#mobility-edge); a long [localization length](#localization-length) can hide confinement in either size.

###### Semiconductor transport evidence for localization

↑ **Parent:** [Anderson localization](#anderson-localization)

[Nevill Francis Mott](physicist.md#nevill-francis-mott)'s 1977 lecture discusses [silicon](chemical-substance.md#silicon) deposited in a glow discharge. Injected [electrons](physics.md#electron) provided a drift-mobility readout; [electrical conductivity](electric-charge.md#electrical-conductivity) and [temperature](temperature.md) dependence tested localized-state transport and excitation toward a [mobility edge](#mobility-edge). Varying [temperature](temperature.md) distinguishes transport regimes. The lecture gives no contact geometry or timing circuit here, so none is inferred. Its Figure 2 is schematic, not measured data.[Electrons in Glass, pp.404–406, Fig.2 and discussion of glow-discharge-deposited silicon; inspected institutional mirror [https://www.nevis.columbia.edu/~haas/documents/physics_nobel_lectures/physics71-80-2.pdf](https://www.nevis.columbia.edu/~haas/documents/physics_nobel_lectures/physics71-80-2.pdf)](physics-bibliography.md#electrons-in-glass-by-nevill-francis-mott)

This evidence motivates a transport question beyond the closed-chain [eigenvalue problem](linear-operator-theory.md#eigenvalue-problem): how does a prepared charge disturbance move under the conditions of a real sample? The numerical figures above supply neither drift-mobility measurements nor a model of the deposition process. Finite-size concentration alone cannot reproduce an experimental [electrical conductivity](electric-charge.md#electrical-conductivity) curve.

Finite [temperature](temperature.md) permits [phonon](quantum-ideal-gas-statistics.md#phonon)-assisted hopping between [localized eigenstates](#localized-eigenstate) or thermal excitation toward a [mobility edge](#mobility-edge); localized states therefore need not imply zero measured [electrical conductivity](electric-charge.md#electrical-conductivity) at every nonzero [temperature](temperature.md).[Electrons in Glass, pp.405,407, localized-state hopping and thermal excitation](physics-bibliography.md#electrons-in-glass-by-nevill-francis-mott)

Real [dephasing](quantum-information-theory.md#dephasing-channel) destroys the relative [wave phases](#phase-waves) needed for long-path [interference](physical-optics.md#interference-wave-propagation). Observing coherent confinement requires the distance over which those [wave phases](#phase-waves) survive to be long enough to explore the localized region, and the sample to be large enough to resolve it. [Temperature](temperature.md) alone is not an automatic switch: the actual inelastic processes set the relevant scales. Static elastic [wave scattering](#wave-scattering) preserves coherence within each realization. Loss of the ensemble-averaged [coherent field](#coherent-wave-field) through random [wave phases](#phase-waves) is therefore not, by itself, physical [dephasing](quantum-information-theory.md#dephasing-channel) of an individual sample.

##### Uncentered wave-field correlation

↑ **Parent:** [Wave propagation in a random medium](#wave-propagation-in-a-random-medium)

For a complex random [wave amplitude](#wave-amplitude), this two-point [expectation](expected-value.md) retains the [coherent field](#coherent-wave-field) and uses a [complex conjugate](complex-analysis.md#complex-conjugate) on the second amplitude. It is not a normalized [wave-field correlation](#uncentered-wave-field-correlation) coefficient. Subtracting $\mathbb E[E(\mathbf r)]\mathbb E[E(\mathbf r')]^*$ gives the centered [covariance function](stochastic-process.md#covariance-function). At coincident points the uncentered [wave-field correlation](#uncentered-wave-field-correlation) equals the [mean wave intensity](#ensemble-averaged-wave-intensity). Under second-order [stationarity](time-series.md#stationary-process) it depends only on the separation and has a [spectral measure of a stationary random field](time-series.md#spectral-measure-of-a-stationary-random-field). A deterministic field is included by taking a degenerate ensemble.

##### Ensemble-averaged wave intensity

↑ **Parent:** [Wave propagation in a random medium](#wave-propagation-in-a-random-medium)

For a random complex wave amplitude $E$, its mean squared amplitude is $I=\mathbb E[|E|^2]$. Expanding $E=m+(E-m)$, with $m=\mathbb E[E]$, gives

$$
 \mathbb E[|E|^2]=|m|^2+\mathbb E[|E-m|^2].
$$

The mixed terms vanish. Thus the squared [coherent field](#coherent-wave-field) is only one part of the mean intensity; the other is the diffuse contribution. A fixed acoustic or optical normalization converts this squared-amplitude quantity to physical [energy flux](mathematical-physics.md#energy-flux). This ensemble mean differs from the angularly averaged radiative-transfer [mean intensity](astrophysics.md#mean-intensity).

##### Coherent wave field

↑ **Parent:** [Wave propagation in a random medium](#wave-propagation-in-a-random-medium)

In [wave propagation in a random medium](#wave-propagation-in-a-random-medium), the coherent field is the [expectation](expected-value.md) of the complex wave amplitude, $m(\mathbf r)=\mathbb E[E(\mathbf r)]$. The remaining field $E-m$ has zero [expectation](expected-value.md). This is the [coherent and diffuse wave fields](partial-differential-equation.md#coherent-and-diffuse-wave-fields) decomposition. [Statistical homogeneity](probability-and-statistics.md#statistical-homogeneity) of the medium does not make $m$ spatially constant when the incident field is localized: translation symmetry applies to the response together with its incident data. The coherent component can attenuate while the total [ensemble-averaged wave intensity](#ensemble-averaged-wave-intensity) remains substantial.

###### Gaussian coherent-field propagation in the Markov approximation

↑ **Parent:** [Coherent wave field](#coherent-wave-field)

For the linear weak-index [parabolic wave equation](partial-differential-equation.md#parabolic-wave-equation), a [Markov approximation](gaussian-process.md#markov-approximation-for-a-random-medium) with integrated covariance $B(\eta)=\int_{\mathbb R}C(s,\eta)ds$ gives

$$
 m_x=\frac{i}{2k}m_{zz}-\gamma m,\qquad \gamma=\frac{k^2\mu^2B(0)}2.
$$

The drift follows by converting the multiplicative [Stratonovich integral](stochastic-calculus.md#stratonovich-integral) $ik\mu E\circ d\mathcal B$ to an [Itô integral](stochastic-calculus.md#ito-integral) for a [Brownian field](brownian-motion.md#longitudinal-brownian-field-with-transverse-covariance) with transverse covariance $B$. For a [Gaussian beam with one transverse coordinate](physical-optics.md#gaussian-beam-with-one-transverse-coordinate) entering the random region at $x_0$, $m(x,z)=e^{-\gamma(x-x_0)}E_{\mathrm{free}}(x,z)$. The [coherent field](#coherent-wave-field) retains transverse beam structure. The white-noise closure needs short longitudinal correlations and the corresponding separation of propagation scales; Gaussian one-point statistics alone are insufficient.

###### Weak-fluctuation memory equation for the coherent field

↑ **Parent:** [Coherent wave field](#coherent-wave-field)

For a [parabolic wave equation](partial-differential-equation.md#parabolic-wave-equation) with $n=1+\mu W$, a zero-mean stationary real field $W$ of unit variance, and $L_0=i\partial_z^2/(2k)$, finite-correlation perturbation theory gives

$$
\begin{aligned}
 m_x&=L_0m+\frac{ik\mu^2}{2}m\\
 &\quad-k^2\mu^2\int_{x_0}^x\int_{\mathbb R}C(x-s,z-\zeta)G_{x-s}(z-\zeta)m(s,\zeta)\,d\zeta\,ds+O(\mu^3).
\end{aligned}
$$

Here $m$ is the [coherent field](#coherent-wave-field), $C$ is the [autocorrelation function of a random field](gaussian-process.md#autocorrelation-function-of-a-random-field) and $G$ is the one-coordinate [Fresnel propagator](partial-differential-equation.md#fresnel-propagator). Expand the random solution once using the [Duhamel principle](diffusion-equation.md#duhamel-s-principle), multiply by $W$ and average to obtain the memory term. The local phase term comes from the $\mu^2W^2$ term in $n^2$. The expansion is for fixed propagation distances with suitable covariance regularity and moment bounds. A [Markov approximation](gaussian-process.md#markov-approximation-for-a-random-medium) is an additional scale assumption that can turn this integral equation into a local attenuation equation.

###### Quadratic refractive-index shift in the coherent field

↑ **Parent:** [Weak-fluctuation memory equation for the coherent field](#weak-fluctuation-memory-equation-for-the-coherent-field)

If the physical [refractive index](electromagnetic-wave.md#refractive-index) is $n=1+\mu W$, then $n^2-1=2\mu W+\mu^2W^2$. In the [parabolic wave equation](partial-differential-equation.md#parabolic-wave-equation), the last term produces $ik\mu^2\mathbb E[W^2E]/2$ in the mean equation. For unit-variance, finite-correlation fluctuations, $\mathbb E[W^2E]=m+O(\mu)$ in a weak-fluctuation expansion, giving a coherent phase drift $ik\mu^2m/2$ to second order. This term is absent if the model deliberately linearizes $n^2-1$ to $2\mu W$. It is not obtained by squaring ideal [Gaussian white noise](gaussian-process.md#gaussian-white-noise), whose pointwise square is not the finite-variance random variable $W^2$.

### Point scatterer

↑ **Parent:** [Wave scattering](#wave-scattering)

#### Short-distance regularization of a resonant point scatterer

↑ **Parent:** [Point scatterer](#point-scatterer)

An outgoing three-dimensional [Green function](green-s-function.md) behaves as $e^{ikr}/r=1/r+ik+O(r)$. Evaluating a point-coupled discrete-level equation at cutoff distance $\delta$ produces a real shift proportional to $1/\delta$ and an imaginary outgoing-wave term proportional to $ik$. The bare level must depend on the cutoff to keep the measured detuning finite.

### Multiple scattering

↑ **Parent:** [Wave scattering](#wave-scattering)

#### Multiple Coulomb scattering

↑ **Parent:** [Multiple scattering](#multiple-scattering)

Repeated deflection of a [charged particle](electric-charge.md#charged-particle) through [electromagnetic interactions](electromagnetism.md#electromagnetic-interaction) with matter.

## Frequency

↑ **Parent:** [Wave](wave.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frequency)

Frequency is the number of repetitions of a periodic phenomenon per unit time. For a [wave](wave.md) of period $T$, its frequency is $\nu=1/T$, measured in hertz. The [angular frequency](lagrangian-mechanics.md#angular-frequency) is $\omega=2\pi\nu$.

### Frequency ratio

↑ **Parent:** [Frequency](#frequency)

The frequency ratio of two nonzero [frequencies](#frequency) is a dimensionless [ratio](arithmetic.md#ratio). Ordinary and [angular frequencies](lagrangian-mechanics.md#angular-frequency) give the same result because both are converted by the same factor $2\pi$. Rational ratios imply a common period for their sinusoidal motions, while the special ratio two means that one mode completes two cycles during one cycle of the other.

### Radio frequency

↑ **Parent:** [Frequency](#frequency)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radio_frequency)

A radio frequency is a [frequency](#frequency) in the range used for [radio waves](electromagnetic-radiation.md#radio-wave). It describes the rapid [oscillation](#oscillation) of a [radio wave](electromagnetic-radiation.md#radio-wave), which can differ from the rate at which information is transmitted in [radio communication](electrical-engineering.md#radio-communication).

### Hertz

↑ **Parent:** [Frequency](#frequency)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hertz)

The unit of [frequency](#frequency) equal to one cycle per second.

## Doppler effect

↑ **Parent:** [Wave](wave.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Doppler_effect)

The [Doppler effect](#doppler-effect) is a change between emitted and received [frequency](#frequency) caused by motion of the source or receiver. An approaching siren can send more [wave crests](dispersion-relation.md#wave-crest) per second to a [microphone](wave-equation.md#microphone) than the source emits per second; a receding siren sends fewer. The source need not change its own [oscillation](#oscillation). The [Doppler shift](#doppler-effect) is $\Delta f=f_o-f_s$, where $f_s>0$ is emitted [frequency](#frequency) and $f_o>0$ is received [frequency](#frequency), both measured in [hertz](#hertz).

For [acoustic waves](fluid-mechanics.md#acoustic-wave), motion must be specified relative to the material carrying the [wave](wave.md). The [speed of sound](compressible-flow.md#speed-of-sound) is measured in that material's rest [reference frame](mathematical-physics.md#reference-frame). Moving the source changes the spacing of successive [wavefronts](physical-optics.md#wavefront); moving the receiver changes how quickly it crosses those [wavefronts](physical-optics.md#wavefront). These two mechanisms give different exact factors in the [classical Doppler effect for sound](#classical-doppler-effect-for-sound), even for the same closing [relative velocity](classical-mechanics.md#relative-velocity).

This makes a [microphone](wave-equation.md#microphone) a motion probe: a stable tone supplies a repeating clock, and changes in arrival spacing reveal the source's motion toward or away from the receiver. An [acoustic Doppler measurement](#acoustic-doppler-measurement) can test the prediction directly. A passing source also illustrates why geometry matters: its speed can stay constant while the received [frequency](#frequency) changes continuously, as in [Doppler frequency along a trajectory](#doppler-frequency-along-a-trajectory).

The following sound model assumes [linear acoustics](linear-acoustics.md) in uniform stationary material with [isotropy](continuum-mechanics.md#isotropy), constant [speed of sound](compressible-flow.md#speed-of-sound) and negligible [wave dispersion](dispersion-relation.md#wave-dispersion). Source and receiver speeds are below the [speed of sound](compressible-flow.md#speed-of-sound), and there is a single direct propagation path. Air motion requires transforming source and receiver [velocities](classical-mechanics.md#velocity) into the air's rest [reference frame](mathematical-physics.md#reference-frame); a nonuniform flow requires a more general propagation model. At the sonic threshold the simple periodic-arrival picture fails; [moving-point acoustic wavefronts](compressible-flow.md#moving-point-acoustic-wavefronts) and the [Mach cone](compressible-flow.md#mach-cone) describe the relevant geometry, while finite [shock waves](transport-equation.md#shock-wave) require further physics. [Light](optics.md#light) in [vacuum](physics.md#vacuum) instead requires the [relativistic Doppler effect](#relativistic-doppler-effect): the acoustic formula cannot be converted into its exact optical counterpart just by replacing the [speed of sound](compressible-flow.md#speed-of-sound) with the [speed of light](special-relativity.md#speed-of-light).

### Rotational Doppler effect

↑ **Parent:** [Doppler effect](#doppler-effect)

A [frequency](#frequency) change associated with rotation and exchange of [angular momentum](momentum.md#angular-momentum). If an optical element rotates at angular velocity $\Omega$ about a chosen axis and gains [angular momentum](momentum.md#angular-momentum) $\Delta L$ from a [photon](quantum-mechanics.md#photon), its mechanical [energy](energy.md) gain is $\Omega\Delta L$ in the prescribed slow-rotation model. [Energy](energy.md) conservation then gives [photon](quantum-mechanics.md#photon) [frequency](#frequency) change $\Delta\omega=-\Omega\Delta L/\hbar$. The [rotating half-wave plate frequency shift](#rotating-half-wave-plate-frequency-shift) is a spin-polarization example.

#### Rotating half-wave plate frequency shift

↑ **Parent:** [Rotational Doppler effect](#rotational-doppler-effect)

A rotating ideal [half-wave plate](maxwell-equations.md#half-wave-plate) flips circular [polarization](#polarization-waves). The spin change has magnitude $2\hbar$ per [photon](quantum-mechanics.md#photon), so its mechanical [energy](energy.md) exchange produces a [frequency](#frequency) shift of magnitude $2|\Omega|$. For Jones convention $H(\theta)=R(\theta)\operatorname{diag}(1,-1)R(-\theta)$ and $Q=\operatorname{diag}(1,i)$, the combination $QH(\theta)Q=e^{i2\theta\sigma_x}$. Acting on $(1,1)^T/\sqrt2$ gives $e^{i2\theta}$; with time dependence $e^{-i\omega t}$ and $\theta=\Omega t$, the output [frequency](#frequency) is $\omega-2\Omega$. The opposite input eigenpolarization reverses the shift.

### Relativistic Doppler effect

↑ **Parent:** [Doppler effect](#doppler-effect)

The [Lorentz transformation](special-relativity.md#lorentz-transformation) changes the [photon](quantum-mechanics.md#photon) [four-momentum](special-relativity.md#four-momentum) and therefore its frequency, producing the displayed formula for a boost along the first axis. Here the primed ray angle is measured in the emitting frame and $\beta=v/c$. The angle and frequency transforms must be used together: [aberration of light](mathematical-physics.md#relativistic-aberration) changes the direction, and a photon-number angular fraction need not equal the corresponding radiant-energy fraction.

Here $c$ is the [vacuum](physics.md#vacuum) [speed of light](special-relativity.md#speed-of-light), $\gamma$ is the [Lorentz factor](special-relativity.md#lorentz-factor), and the two [frequencies](#frequency) are measured in different inertial [reference frames](mathematical-physics.md#reference-frame). Unlike the [classical Doppler effect for sound](#classical-doppler-effect-for-sound), there is no material rest [reference frame](mathematical-physics.md#reference-frame) for [light](optics.md#light) in [vacuum](physics.md#vacuum). For small radial recession speed $v_r\ll c$, the [wavelength](wave-equation.md#wavelength) shift satisfies $\Delta\lambda/\lambda\simeq v_r/c$. This small-speed limit underlies [Doppler spectroscopy](exoplanet.md#doppler-spectroscopy); it is not an exact sound formula.

#### Frequency ratio of corotating clocks

↑ **Parent:** [Relativistic Doppler effect](#relativistic-doppler-effect)

For a freely propagating [photon](quantum-mechanics.md#photon) between emitters and receivers rotating with the same [angular velocity](rigid-body-dynamics.md#angular-velocity) in flat [spacetime](special-relativity.md#spacetime), $\nu_r/\nu_e=\gamma_r/\gamma_e$, provided the [photon](quantum-mechanics.md#photon) path is unobstructed. At equal radii the ratio is one. Positions and [velocities](classical-mechanics.md#velocity) at the actual emission and reception events must be used.

#### Doppler extrema for a circularly moving source

↑ **Parent:** [Relativistic Doppler effect](#relativistic-doppler-effect)

A source of fixed proper [frequency](#frequency) and [speed](classical-mechanics.md#speed) $v$ on a circle has instantaneous [frequency](#frequency) extrema $\nu_0\sqrt{(1\pm\beta)/(1\mp\beta)}$ for a stationary coplanar receiver outside the circle. The extrema occur when the emission ray is tangent to the source circle, so line-of-sight [speed](classical-mechanics.md#speed) reaches $\pm v$.

#### Transverse Doppler shift and observation time

↑ **Parent:** [Relativistic Doppler effect](#relativistic-doppler-effect)

Let $\theta$ be the angle between the source velocity and the emitted photon's propagation direction in the observer's frame. The [relativistic Doppler effect](#relativistic-doppler-effect) gives $\nu=\nu_0/[\gamma(1-\beta\cos\theta)]$. A ray transverse in that frame has $\lambda=\gamma\lambda_0$, a redshift. A ray transverse in the source frame instead has $\cos\theta=\beta$ by [aberration of light](mathematical-physics.md#relativistic-aberration), and $\lambda=\lambda_0/\gamma$, a blueshift.

The time at which a passing source is closest must also be specified. Put the observer at the origin and the source at $(vt_e,d)$ at emission, with finite transverse offset $d>0$. Reception occurs at

$$
t_r=t_e+\frac{\sqrt{v^2t_e^2+d^2}}c.
$$

Emission at closest approach means $t_e=0$, a transverse observer-frame ray received at $t_r=d/c$, hence a redshift. Reception at closest approach means $t_r=0$, so $t_e=-\gamma d/c$ and the ray has $\cos\theta=\beta$, hence a blueshift. Sending $d$ to zero does not remove the distinction between these two limiting event prescriptions. [MIT 8.286, transverse Doppler shifts, distinction between closest approach at emission and reception](https://web.mit.edu/8.286/www/quiz18/q1rp-euf18.pdf)

#### Moving-mirror Doppler shift

↑ **Parent:** [Relativistic Doppler effect](#relativistic-doppler-effect)

A mirror receding at [velocity](classical-mechanics.md#velocity) $u=\beta c$ from normally incident [light](optics.md#light) produces two applications of the [relativistic Doppler effect](#relativistic-doppler-effect), one into the mirror rest frame and one back to the observer. In that rest frame, reflection preserves [frequency](#frequency). Consequently $\omega_r=\gamma^2(1-\beta)^2\omega_i=\omega_i(1-\beta)/(1+\beta)$. Equivalently, continuity of [wave phase](#phase-waves) on the moving surface $z=ut$ gives $\omega_i-k_i u=\omega_r+k_r u$, with $k_i=\omega_i/c$ and $k_r=\omega_r/c$. For $|u|\ll c$, the fractional [frequency](#frequency) change is $-2u/c$ to first order.

##### Moving-mirror photon interception rate

↑ **Parent:** [Moving-mirror Doppler shift](#moving-mirror-doppler-shift)

For a [photon](quantum-mechanics.md#photon) emitted from the origin and arriving at receding mirror position $x(t)$, its emission time is $t_e=t-x(t)/c$. Thus $dt_e/dt=1-\beta$ and a steady source rate $R$ gives impact rate $R(1-\beta)$ in source-frame coordinate time. This is distinct from the emission rate and from a rate per mirror [proper time](special-relativity.md#proper-time).

#### Kinematic redshift

↑ **Parent:** [Relativistic Doppler effect](#relativistic-doppler-effect)

A kinematic redshift is the [relativistic Doppler effect](#relativistic-doppler-effect) from relative motion of emitter and receiver. With positive radial recession speed $v$, its small-velocity limit is $z_{\rm kin}=v/c+O(v^2/c^2)$. A [peculiar velocity](cosmology.md#peculiar-velocity) gives such a factor in addition to [cosmological redshift](cosmology.md#cosmological-redshift).

### Classical Doppler effect for sound

↑ **Parent:** [Doppler effect](#doppler-effect)

Work in the material's rest [reference frame](mathematical-physics.md#reference-frame), with constant [speed of sound](compressible-flow.md#speed-of-sound) $c>0$. For one-dimensional propagation, choose the positive $x$ direction along the travelling [wave](wave.md) from its emission point toward the receiver. Define $u_s=dx_s/dt$ and $u_o=dx_o/dt$ as the signed source and receiver [velocities](classical-mechanics.md#velocity) along that same axis. Both use the same sign convention: positive $u_s$ moves the source toward the receiver ahead, whereas positive $u_o$ moves that receiver away from the incoming [wave](wave.md). Assume $|u_s|<c$ and $|u_o|<c$, constant [velocities](classical-mechanics.md#velocity), and no source-receiver crossing during the interval considered. Then

$$
f_o=f_s\frac{c-u_o}{c-u_s}.
$$

To derive this, let $T_s=1/f_s$ be the emission [wave period](#wave-period). During $T_s$, one [wave crest](dispersion-relation.md#wave-crest) travels $cT_s$ while the source advances $u_sT_s$. Successive [wavefronts](physical-optics.md#wavefront) along the chosen direction therefore have [wavelength](wave-equation.md#wavelength)

$$
\lambda=(c-u_s)T_s=\frac{c-u_s}{f_s}.
$$

They overtake the receiver at relative speed $c-u_o$, so counting [wave crests](dispersion-relation.md#wave-crest) gives $f_o=(c-u_o)/\lambda$. This separates the source's effect on [wavelength](wave-equation.md#wavelength) from the receiver's effect on crossing rate. Even with a moving source, a stationary receiver obeys $f_o\lambda=c$ because the [wave speed](wave-equation.md#wave-speed) through the material remains $c$.

For a stationary receiver and a source approaching at speed $v$, set $u_o=0$ and $u_s=v$: $f_o=f_sc/(c-v)>f_s$. For recession choose the positive axis along the departing [wave](wave.md) toward the receiver again, so the source has $u_s=-v$: $f_o=f_sc/(c+v)<f_s$. For the deliberately chosen values $c=343\,\mathrm{m\,s^{-1}}$, $v=20\,\mathrm{m\,s^{-1}}$ and $f_s=500\,\mathrm{Hz}$, the two predictions are

$$
f_{\mathrm{approach}}=500\frac{343}{323}\,\mathrm{Hz}\simeq530.96\,\mathrm{Hz},\qquad f_{\mathrm{recede}}=500\frac{343}{363}\,\mathrm{Hz}\simeq472.45\,\mathrm{Hz}.
$$

The corresponding [wavelengths](wave-equation.md#wavelength) are $0.646\,\mathrm m$ and $0.726\,\mathrm m$, compared with $c/f_s=0.686\,\mathrm m$ for a stationary source. These are calculations for chosen parameters, not reported measurements.

<a id="doppler-source-wavefront-spacing"></a>
![](doppler-source-wavefront-spacing.png)

**[Figure 5](#doppler-source-wavefront-spacing). Moving-source wavefront spacing in the classical Doppler effect for sound**. Original [linear acoustics](linear-acoustics.md) model at $t=0$, with a deliberately enlarged speed ratio $v/c=0.4$ for readability. Lengths are measured in $\lambda_0=c/f_s$. Successive [circles](topology.md#circle) are sections of spherical [wavefronts](physical-optics.md#wavefront) emitted one [wave period](#wave-period) apart; their centres stay at the old emission positions. The forward spacing is $0.6\lambda_0$ and the rear spacing $1.4\lambda_0$. These chosen parameters differ from the $20\,\mathrm{m\,s^{-1}}$ worked example.

A receiver approaching a stationary source at $20\,\mathrm{m\,s^{-1}}$ instead has $u_s=0$, $u_o=-20\,\mathrm{m\,s^{-1}}$, giving $f_o=500(363/343)\,\mathrm{Hz}\simeq529.15\,\mathrm{Hz}$. Moving away gives $f_o=500(323/343)\,\mathrm{Hz}\simeq470.85\,\mathrm{Hz}$. The equal closing speeds do not make these equal to the moving-source values. If both source and receiver move together with $u_s=u_o$, however, the numerator and denominator cancel and $f_o=f_s$. For speeds small compared with $c$, the first-order shift is $(f_o-f_s)/f_s\simeq(u_s-u_o)/c$; the difference between moving-source and moving-receiver experiments appears beyond this first order.

### Doppler frequency along a trajectory

↑ **Parent:** [Doppler effect](#doppler-effect)

In the same uniform stationary sound model, let $\tau$ be emission [time](classical-mechanics.md#time-in-physics), $t$ reception [time](classical-mechanics.md#time-in-physics), and $\mathbf x_s(\tau)$ and $\mathbf x_o(t)$ source and receiver positions. The direct-path propagation condition and its direction are

$$
c(t-\tau)=R,\qquad R=|\mathbf x_o(t)-\mathbf x_s(\tau)|>0,\qquad \mathbf n=\frac{\mathbf x_o(t)-\mathbf x_s(\tau)}{R}.
$$

The [unit vector](vector-space.md#unit-vector) $\mathbf n$ points from the source's old emission position to the receiver's reception position. With [velocities](classical-mechanics.md#velocity) $\mathbf v_s=d\mathbf x_s/d\tau$ and $\mathbf v_o=d\mathbf x_o/dt$, taking a [derivative](calculus.md#derivative) of the propagation condition gives

$$
c\left(1-\frac{d\tau}{dt}\right)=\mathbf n\cdot\mathbf v_o-\mathbf n\cdot\mathbf v_s\frac{d\tau}{dt},\qquad f_o(t)=f_s\frac{d\tau}{dt}=f_s\frac{c-\mathbf n\cdot\mathbf v_o(t)}{c-\mathbf n\cdot\mathbf v_s(\tau)}.
$$

Here the [dot products](inner-product.md#dot-product) project onto the actual propagation direction. The last equality counts source [wave phase](#phase-waves) cycles at reception for constant emitted [frequency](#frequency) $f_s$. It assumes both speeds are below $c$, a unique direct arrival and smooth motion; interpreting a measured short-window [frequency spectrum](fourier-analysis.md#frequency-spectrum) additionally requires little [frequency](#frequency) change within that window. The source [velocity](classical-mechanics.md#velocity) must be evaluated at emission, not at reception. This delayed geometry matters when the direction changes.

For an original pass-by model, a source follows $\mathbf x_s(\tau)=(v\tau,0)$ and a stationary receiver is at $(0,b)$ with $b>0$. The source passes its closest position at emission [time](classical-mechanics.md#time-in-physics) $\tau=0$. Then

$$
R=\sqrt{v^2\tau^2+b^2},\qquad t=\tau+R/c,\qquad f_o(t)=f_s\frac{c}{c+v^2\tau/R}.
$$

These parametric equations give received [frequency](#frequency) against reception [time](classical-mechanics.md#time-in-physics). For $\tau<0$ the shift is positive, for $\tau>0$ negative, and the unshifted emission at $\tau=0$ reaches the receiver at $t=b/c$. Thus zero shift occurs after the source's geometric closest passage in the material's [reference frame](mathematical-physics.md#reference-frame). Increasing $b$ spreads the transition over a longer interval even though $v$ is unchanged. Far before and after passage, the [frequency](#frequency) approaches $f_sc/(c-v)$ and $f_sc/(c+v)$ respectively.

<a id="doppler-receiver-frequency-trajectories"></a>
![](doppler-receiver-frequency-trajectories.png)

**[Figure 6](#doppler-receiver-frequency-trajectories). Receiver offset changes the shape of a passing source's Doppler shift**. Original model predictions for $c=343\,\mathrm{m\,s^{-1}}$, $v=20\,\mathrm{m\,s^{-1}}$, $f_s=500\,\mathrm{Hz}$ and receiver offsets $b=2\,\mathrm m$ and $10\,\mathrm m$. The upper panel shows the shared straight source [trajectory](classical-mechanics.md#trajectory) and the two receiver positions; the lower panel uses reception [time](classical-mechanics.md#time-in-physics) $t=\tau+R/c$. Dots at $t=b/c$ mark zero shift. Dashed horizontal limits are the one-dimensional approach and recession values. No curve is measured data.

### Acoustic Doppler measurement

↑ **Parent:** [Doppler effect](#doppler-effect)

UNSW School of Physics documents a [Doppler effect](#doppler-effect) experiment using a buzzer based on [piezoelectricity](quantum-mechanics.md#piezoelectricity), powered by a taped-on $9\,\mathrm V$ [battery](electrical-circuit.md#electric-battery), and a computer's built-in [microphone](wave-equation.md#microphone). Audacity records the [acoustic wave](fluid-mechanics.md#acoustic-wave). First record the stationary source to establish its baseline [frequency](#frequency); then attach it to a bicycle passing the stationary [microphone](wave-equation.md#microphone). The published [spectrogram](fourier-analysis.md#spectrogram) shows a rapid decrease in [frequency](#frequency) during passage.[UNSW, Measuring velocities using the Doppler Shift: Introduction, Figs. 1–2; Circular Motion, Measurements (2)–(3); Linear Motion:Bicycle, Moving Source](physics-bibliography.md#measuring-velocities-using-the-doppler-shift-at-unsw-school-of-physics)

For numerical readout, select an approaching or receding interval, display its [frequency spectrum](fourier-analysis.md#frequency-spectrum) using Plot Spectrum, and read the interpolated Peak [frequency](#frequency). The protocol recommends repeating with slightly different selections to test stability, and working outdoors to reduce reflections and [standing waves](mathematical-physics.md#standing-wave). Longer windows refine [frequency](#frequency) spacing while averaging over more motion. The baseline controls for the source's actual tone; repeated selections expose analysis-window sensitivity.[UNSW, Introduction, final paragraph; Circular Motion, spectrogram resolution discussion; Linear Motion:Bicycle, Plot Spectrum and Peak instructions](physics-bibliography.md#measuring-velocities-using-the-doppler-shift-at-unsw-school-of-physics)

Under nearly collinear constant-speed approach, infer $v=c(1-f_s/f_o)$ from the [classical Doppler effect for sound](#classical-doppler-effect-for-sound). For recession the positive speed is $v=c(f_s/f_o-1)$. These inversions need a specified [speed of sound](compressible-flow.md#speed-of-sound). An offset path changes the projection, as in [Doppler frequency along a trajectory](#doppler-frequency-along-a-trajectory); neither inversion measures the full speed near closest passage. The protocol's controls cannot remove arbitrary [acceleration](classical-mechanics.md#acceleration), background [measurement noise](probability-and-statistics.md#measurement-noise) or unresolved reflected paths. No new measurements are claimed here.

## Wave propagation

↑ **Parent:** [Wave](wave.md)

## ↑ Ancestors (2)

1. [Physics](physics.md)
2. [Codex Wiki](README.md)

## ← Incoming links (59)

- [Alfvénic turbulence](turbulence.md#alfvenic-turbulence)
- [Anderson localization](#anderson-localization)
- [Bending wave of a Keplerian disk](astrophysical-disk.md#bending-wave-of-a-keplerian-disk)
- [Capillary length](surface-tension.md#capillary-length)
- [Capillary wave](surface-tension.md#capillary-wave)
- [Carrier wave](dispersion-relation.md#carrier-wave)
- [Classical Doppler effect for sound](#classical-doppler-effect-for-sound)
- [Cosmological redshift](cosmology.md#cosmological-redshift)
- [Crest and trough](dispersion-relation.md#crest-and-trough)
- [Critical angle for total internal reflection](electromagnetic-wave.md#critical-angle-for-total-internal-reflection)
- [Diffusion limit of the damped heat-transmission equation](wave-equation.md#diffusion-limit-of-the-damped-heat-transmission-equation)
- [Doppler effect](#doppler-effect)
- [Driven-string endpoint power](wave-equation.md#driven-string-endpoint-power)
- [Electron optics](optics.md#electron-optics)
- [Energy flux of a transverse string wave](wave-equation.md#energy-flux-of-a-transverse-string-wave)
- [Equal-density ion-neutral Alfvén dispersion relation](ideal-magnetohydrodynamics.md#equal-density-ion-neutral-alfven-dispersion-relation)
- [Frequency](#frequency)
- [Hubble's law](cosmology.md#hubble-s-law)
- [Interferometer](physical-optics.md#interferometer)
- [John William Strutt, 3rd Baron Rayleigh](physicist.md#john-william-strutt-3rd-baron-rayleigh)
- [Linear mass density](fluid-mechanics.md#linear-mass-density)
- [Local wavelength](wave-equation.md#local-wavelength)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2015/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2022.md#section-a/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-74.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-75.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-75.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-75.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#31a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2.md#section-a/2/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2.md#section-b/b8/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2.md#section-b/b7/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2.md#section-c/c11/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-b/b6/a/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-b/b6/d/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-b/b8/b/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1.md#section-b/b8/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#section-a/a6/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#section-d/d13/solution)
- [Physical oceanography](physics.md#physical-oceanography)
- [Physical optics](physical-optics.md)
- [Polarization (waves)](#polarization-waves)
- [Refraction](optics.md#refraction)
- [Spatial sampling of a wave](wave-equation.md#spatial-sampling-of-a-wave)
- [Standing wave](mathematical-physics.md#standing-wave)
- [TEM travelling-wave voltage-current relation](electrical-engineering.md#tem-travelling-wave-voltage-current-relation)
- [Tension](force.md#tension)
- [Three-wave mixing](optics.md#three-wave-mixing)
- [Total internal reflection](electromagnetic-wave.md#total-internal-reflection)
- [Wave absorption](#wave-absorption)
- [Wave crest](dispersion-relation.md#wave-crest)
- [Wave equation](wave-equation.md)
- [Wave period](#wave-period)
- [Wave reflection](#wave-reflection)
- [Wave turbulence](turbulence.md#wave-turbulence)
