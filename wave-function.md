# Wave function

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wave_function)

A [wavefunction](wave-function.md) is the position representation of a [pure state](quantum-theory.md#pure-state). In the one-dimensional model used here, $\psi(x,t)$ takes values in the [complex numbers](complex-analysis.md#complex-number), and the [Born rule](#born-rule) gives

$$
\rho(x,t)=|\psi(x,t)|^2,\qquad \Pr(a<x<b)=\int_a^b\rho(x,t)\,dx.
$$

The [probability density](#probability-density) $\rho$ has units of inverse length; the [wavefunction](wave-function.md) has units of inverse square root of length. A value of $\rho$ at a point is not itself a probability: probabilities come from an [integral](integral.md) over a region. For the [infinite square well](quantum-mechanics.md#infinite-square-well) [ground state](quantum-mechanics.md#ground-state), $\rho(L/2)=2/L$, whereas the probability of the exact single point $L/2$ is zero. The interesting question is how much probability a finite interval contains.

Two [wavefunctions](wave-function.md) differing only by a [global phase](quantum-system.md#global-phase) represent the same [pure state](quantum-theory.md#pure-state). Relative [quantum phases](quantum-system.md#quantum-phase) between components of a [quantum superposition](quantum-system.md#quantum-superposition) affect [matter-wave interference](#matter-wave-interference), so retaining the full [complex number](complex-analysis.md#complex-number) amplitude is essential. This scalar description covers a particle without active [spin](angular-momentum-operator.md#spin) degrees of freedom; a general [electron](physics.md#electron) [wavefunction](wave-function.md) can have two [spin](angular-momentum-operator.md#spin) components, with the position [probability density](#probability-density) obtained by adding the squared [modulus](complex-analysis.md#modulus) of each component.

**Table of contents**

- [Single-valued wavefunction](#single-valued-wavefunction)
- [Momentum representation in quantum mechanics](#momentum-representation-in-quantum-mechanics)
- [Top-hat wavefunction](#top-hat-wavefunction)
  - [Momentum variance of a discontinuous top hat](#momentum-variance-of-a-discontinuous-top-hat)
- [Position representation in quantum mechanics](#position-representation-in-quantum-mechanics)
- [Node of a wavefunction](#node-of-a-wavefunction)
  - [Kinetic-energy estimate from wavefunction nodes](#kinetic-energy-estimate-from-wavefunction-nodes)
- [Wavefunction normalization](#wavefunction-normalization)
- [Matter wave](#matter-wave)
  - [Matter-wave coherence](#matter-wave-coherence)
  - [de Broglie phase harmony](#de-broglie-phase-harmony)
  - [Relativistic matter-wave velocities](#relativistic-matter-wave-velocities)
  - [Thomson electron transmission diffraction experiment](#thomson-electron-transmission-diffraction-experiment)
  - [Matter-wave interference](#matter-wave-interference)
  - [de Broglie wavelength](#de-broglie-wavelength)
    - [Free-particle momentum convention](#free-particle-momentum-convention)
    - [Electron accelerating-voltage wavelength](#electron-accelerating-voltage-wavelength)
  - [Neutron interferometer](#neutron-interferometer)
    - [Colella–Overhauser–Werner experiment](#colella-overhauser-werner-experiment)
- [Plane wave](#plane-wave)
- [Probability amplitude](#probability-amplitude)
  - [Born rule](#born-rule)
    - [Born statistical scattering interpretation](#born-statistical-scattering-interpretation)
      - [Angular scattering probability from complex amplitudes](#angular-scattering-probability-from-complex-amplitudes)
      - [Two-channel scattering with flux normalization](#two-channel-scattering-with-flux-normalization)
    - [Two-level quantum return probability](#two-level-quantum-return-probability)
    - [Two-level observable transition probability](#two-level-observable-transition-probability)
    - [Wigner's theorem](#wigner-s-theorem)
      - [Projective unitary representation](#projective-unitary-representation)
    - [Energy measurement](#energy-measurement)
- [Normalizable wavefunction](#normalizable-wavefunction)
- [Probability density](#probability-density)
  - [Radial probability density](#radial-probability-density)
- [Probability current](#probability-current)
  - [Probability current of a two-dimensional Dirac particle](#probability-current-of-a-two-dimensional-dirac-particle)
  - [Probability continuity equation](#probability-continuity-equation)
    - [Conservation of quantum probability](#conservation-of-quantum-probability)
- [Gaussian wave packet](#gaussian-wave-packet)
  - [Gaussian covariance in a harmonic potential](#gaussian-covariance-in-a-harmonic-potential)
  - [Free Gaussian wave packet evolution](#free-gaussian-wave-packet-evolution)
  - [Gaussian evolution in an inverted harmonic oscillator](#gaussian-evolution-in-an-inverted-harmonic-oscillator)

## Single-valued wavefunction

↑ **Parent:** [Wave function](wave-function.md)

An ordinary scalar [wavefunction](wave-function.md) assigns one complex amplitude to each physical configuration. In [polar coordinates](multivariable-calculus.md#polar-coordinates) without an additional twisted boundary condition, the points $(r,\phi)$ and $(r,\phi+2\pi)$ are identical, so the angular factor must be periodic. An angular [eigenfunction](linear-operator-theory.md#eigenfunction) $e^{im\phi}$ therefore requires integer $m$. This scalar orbital condition does not rule out half-integer intrinsic [spin](angular-momentum-operator.md#spin).

## Momentum representation in quantum mechanics

↑ **Parent:** [Wave function](wave-function.md)

The [Fourier transform](fourier-transform.md) in the title represents a one-dimensional state in the [wavevector](elasticity-physics.md#wavevector) basis. Its [probability density](#probability-density) is $|\phi(k)|^2$, normalized by $\int|\phi(k)|^2dk=1$ when $\int|\psi(x)|^2dx=1$. For physical [momentum](momentum.md) $p=\hbar k$, the density per unit momentum is $|\phi(p/\hbar)|^2/\hbar$. A confined stationary [energy eigenstate](energy-eigenvalue.md#energy-eigenstate) need not be a [momentum eigenstate](energy-eigenvalue.md#momentum-eigenstate).

## Top-hat wavefunction

↑ **Parent:** [Wave function](wave-function.md)

A [top-hat wavefunction](#top-hat-wavefunction) is constant on an interval and zero elsewhere. It has a uniform [position](classical-mechanics.md#position) [distribution](distribution-theory.md#distribution-mathematical-analysis) and a [sinc function](fourier-transform.md#sinc-function) [momentum](momentum.md) [amplitude](wave.md#wave-amplitude). Its discontinuous edges place it outside the finite-kinetic-energy domain of the free [Hamiltonian](hamiltonian-mechanics.md#hamiltonian). Smooth-edged localized packets can approximate its [position](classical-mechanics.md#position) profile while having different [momentum](momentum.md) tails.

### Momentum variance of a discontinuous top hat

↑ **Parent:** [Top-hat wavefunction](#top-hat-wavefunction)

The [momentum](momentum.md) density of a [top-hat wavefunction](#top-hat-wavefunction) decays as an oscillatory $1/p^2$ envelope. Its [momentum](momentum.md) second moment therefore diverges, although the [probability density](#probability-density) itself is normalizable. The central diffraction-lobe width is not the [standard deviation](variance.md#standard-deviation). Even the first moment requires care: the symmetric [principal value](complex-analysis.md#cauchy-principal-value) is zero, but the absolute first moment diverges logarithmically.

## Position representation in quantum mechanics

↑ **Parent:** [Wave function](wave-function.md)

The [wavefunction](wave-function.md) is the [probability amplitude](#probability-amplitude) of a [quantum state](quantum-system.md#quantum-state) in the generalized position [basis](vector-space.md#basis). For a scalar particle on a line, the [position operator](quantum-mechanics.md#position-operator) multiplies by $x$ and the [momentum operator](quantum-mechanics.md#momentum-operator) acts as $-i\hbar\,d/dx$ on their appropriate domains. This makes the [canonical commutation relation](quantum-mechanics.md#canonical-commutation-relation) $[x,p]=i\hbar$ explicit.

## Node of a wavefunction

↑ **Parent:** [Wave function](wave-function.md)

A position or set of positions where a [wavefunction](wave-function.md) vanishes. Its [Born rule](#born-rule) position [probability density](#probability-density) is also zero there. For a one-dimensional bound state, counting interior nodes distinguishes successive [energy eigenfunctions](energy-eigenvalue.md#energy-eigenfunction); hard-wall endpoint zeros are usually counted separately.

### Kinetic-energy estimate from wavefunction nodes

↑ **Parent:** [Node of a wavefunction](#node-of-a-wavefunction)

A [wavefunction](wave-function.md) with extent $a$ and many nearly equally spaced internal [nodes of a wavefunction](#node-of-a-wavefunction) has local [wavevector](elasticity-physics.md#wavevector) $k\sim\pi n/a$. Thus $\langle K\rangle=\hbar^2\int|\psi'|^2/(2m\int|\psi|^2)$ scales as $\hbar^2n^2/(ma^2)$. Exact coefficients require the envelope and [boundary conditions](differential-equation.md#boundary-condition). An order-one node-count offset is needed for low states: a nodeless localized state still has positive [kinetic energy](energy.md#kinetic-energy) by the [Heisenberg uncertainty principle](quantum-theory.md#heisenberg-uncertainty-relation).

## Wavefunction normalization

↑ **Parent:** [Wave function](wave-function.md)

Wavefunction normalization makes the total [Born rule](#born-rule) probability equal to one. In an [orthonormal basis](inner-product.md#orthonormal-basis) of [energy eigenstates](energy-eigenvalue.md#energy-eigenstate), $\psi=\sum_n c_n\phi_n$ is normalized precisely when $\sum_n|c_n|^2=1$.

For a proposed [infinite square well](quantum-mechanics.md#infinite-square-well) mode $A\sin(n\pi x/L)$, the [integral](integral.md) of its squared [modulus](complex-analysis.md#modulus) is $|A|^2L/2$. Thus [wavefunction normalization](#wavefunction-normalization) requires $|A|=\sqrt{2/L}$; choosing $A$ real and positive fixes a convenient [global phase](quantum-system.md#global-phase). For the equal [quantum superposition](quantum-system.md#quantum-superposition) $(\phi_1+\phi_2)/\sqrt2$, [orthogonality](inner-product.md#orthogonal-vectors) makes the integrated cross term zero, leaving $1/2+1/2=1$. The cross term can nevertheless be nonzero locally: normalization constrains total probability, not the shape of its [probability density](#probability-density).

## Matter wave

↑ **Parent:** [Wave function](wave-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matter_wave)

A matter wave is the quantum wave associated with a material particle. Its phase can interfere after coherent paths recombine.

In the position representation, a [matter wave](#matter-wave) is described by a [wavefunction](wave-function.md): a [complex number](complex-analysis.md#complex-number) [probability amplitude](#probability-amplitude), with detection probabilities given by the [Born rule](#born-rule). A localized [wave packet](dispersion-relation.md#wave-packet) combines different [momenta](momentum.md); its envelope can move while its individual [quantum phase](quantum-system.md#quantum-phase) crests move at another speed. Neither curve is a literal mechanical oscillation of material along a particle's path. The [de Broglie phase harmony](#de-broglie-phase-harmony) explains the historical route to $\lambda=h/p$; the [relativistic matter-wave velocities](#relativistic-matter-wave-velocities) distinguish the two speeds. The [Davisson–Germer experiment](quantum-scattering.md#davisson-germer-experiment) and the [Thomson electron transmission diffraction experiment](#thomson-electron-transmission-diffraction-experiment) connect that spatial [quantum phase](quantum-system.md#quantum-phase) to measured [electron diffraction](quantum-scattering.md#electron-diffraction).

### Matter-wave coherence

↑ **Parent:** [Matter wave](#matter-wave)

### de Broglie phase harmony

↑ **Parent:** [Matter wave](#matter-wave)

In the 1923 note _Waves and Quanta_, [Louis de Broglie](physicist.md#louis-de-broglie) proposed a periodic process associated with [rest energy](special-relativity.md#rest-energy), remaining in phase with a wave along the moving particle's path. He distinguished the internal [frequency](wave.md#frequency) slowed by [time dilation](special-relativity.md#time-dilation) from the wave [frequency](wave.md#frequency) based on total [energy](energy.md).[Nature 112, p. 540, 13 October 1923, opening paragraph](physics-bibliography.md#waves-and-quanta-by-louis-de-broglie) The proposal developed into his 1924 thesis.[Nobel Lectures, Physics 1922–1941; Louis de Broglie, Biographical, printed p. 257: 1924 thesis and doctoral degree](physics-bibliography.md#nobel-lectures-physics-1922-1941/louis-de-broglie-biographical) In the 1929 lecture _The wave nature of the electron_, he reconstructed the argument using a [Lorentz transformation](special-relativity.md#lorentz-transformation).[Nobel Lectures, Physics 1922–1941; 12 December 1929, printed pp. 247–249: rest-frame periodicity, Lorentz transformation and momentum](physics-bibliography.md#nobel-lectures-physics-1922-1941/the-wave-nature-of-the-electron-by-louis-de-broglie)

Here is that [quantum phase](quantum-system.md#quantum-phase) argument in modern notation. Set $\omega_0=mc^2/\hbar$ in the [rest frame](mathematical-physics.md#rest-frame). A [Lorentz transformation](special-relativity.md#lorentz-transformation) to a frame where the particle has [velocity](classical-mechanics.md#velocity) $v$ gives

$$
t'=\gamma\left(t-\frac{vx}{c^2}\right),\qquad
\gamma=\frac{1}{\sqrt{1-v^2/c^2}},\qquad
\phi=\omega_0t'=\frac{Et-px}{\hbar},\qquad
E=\gamma mc^2,\quad p=\gamma mv.
$$

Along $x=vt$, [proper time](special-relativity.md#proper-time) is $\tau=t/\gamma$, so

$$
\phi(vt,t)=\frac{(E-pv)t}{\hbar}
=\frac{mc^2t}{\gamma\hbar}=\omega_0\tau.
$$

This is the harmony: evaluating the spatial wave at the moving particle gives the slower clock phase. At fixed $x$, its [angular frequency](lagrangian-mechanics.md#angular-frequency) is instead $E/\hbar=\gamma\omega_0$. Since $k=p/\hbar$, the [de Broglie wavelength](#de-broglie-wavelength) follows as $\lambda=2\pi/k=h/p$. The proposed clock was a theoretical construction, not an observed mechanical vibration.

### Relativistic matter-wave velocities

↑ **Parent:** [Matter wave](#matter-wave)

For a one-dimensional [free particle](quantum-mechanics.md#free-particle) with $m>0$ and $p>0$, take the positive total [energy](energy.md) from the [relativistic energy-momentum relation](special-relativity.md#energy-momentum-relation):

$$
E(p)=\sqrt{m^2c^4+p^2c^2},\qquad
\omega=E/\hbar,\qquad k=p/\hbar.
$$

A fixed [plane wave](#plane-wave) [quantum phase](quantum-system.md#quantum-phase) obeys $kx-\omega t=\text{constant}$. Its [phase velocity](dispersion-relation.md#phase-velocity) is therefore

$$
v_{\mathrm{ph}}=\frac{\omega}{k}=\frac{E}{p}=\frac{c^2}{v}>c.
$$

For a narrow [wave packet](dispersion-relation.md#wave-packet) centered at $p_0$, expand its [dispersion relation](dispersion-relation.md) as $E(p)\simeq E(p_0)+E'(p_0)(p-p_0)$. In the [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) [integral](integral.md) building the [wave packet](dispersion-relation.md#wave-packet), the envelope then depends on $x-E'(p_0)t$. Thus its [group velocity](dispersion-relation.md#group-velocity) is

$$
v_{\mathrm g}=\frac{d\omega}{dk}=\frac{dE}{dp}=\frac{pc^2}{E}=v<c,\qquad
v_{\mathrm{ph}}v_{\mathrm g}=c^2.
$$

The superluminal [phase velocity](dispersion-relation.md#phase-velocity) follows a repeating phase marker; it does not describe a localized signal or superluminal transport of [energy](energy.md). Higher derivatives of the [dispersion relation](dispersion-relation.md) produce [wave packet](dispersion-relation.md#wave-packet) spreading, so the translated-envelope argument is a narrow-band approximation. For $v=0.6c$, the [Lorentz factor](special-relativity.md#lorentz-factor) is $1.25$, $p=0.75mc$ and $E=1.25mc^2$: the [group velocity](dispersion-relation.md#group-velocity) is $0.6c$ while the [phase velocity](dispersion-relation.md#phase-velocity) is $5c/3$.

<a id="image-a-matter-wave-s-phase-velocity-and-group-velocity-are-different-slopes"></a>
![](matter-wave-phase-and-group-velocity.png)

**[Figure 1](#image-a-matter-wave-s-phase-velocity-and-group-velocity-are-different-slopes). A matter wave's phase velocity and group velocity are different slopes**. [Source](matter-wave-phase-and-group-velocity.py). Original one-dimensional [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) model with $m=c=\hbar=1$, central [momentum](momentum.md) $p_0=0.75$ and [Gaussian function](calculus.md#gaussian-function) momentum amplitude $a(p)\propto\exp[-(p-p_0)^2/(4\sigma_p^2)]$, $\sigma_p=0.055$. The blue curve is the real part of $\Psi(x,t)=\int a(p)e^{i(px-E(p)t)}\,dp$ and the orange curves bound its amplitude. Dashed lines mark $v_{\mathrm g}t$; dotted lines track one phase of the central [plane wave](#plane-wave), $x=Et/p$. The right panel compares the secant and tangent slopes. This scalar model illustrates the [dispersion relation](dispersion-relation.md), without representing [electron](physics.md#electron) [spin](angular-momentum-operator.md#spin) or measured particle paths.

The total-[energy](energy.md) convention matters. Define $\psi=e^{imc^2t/\hbar}\Psi$ to remove the common [rest energy](special-relativity.md#rest-energy) from a [wavefunction](wave-function.md) $\Psi$ with total-[energy](energy.md) time dependence. Then

$$
K=E-mc^2\simeq\frac{p^2}{2m},\qquad
\omega_{\mathrm{NR}}=K/\hbar,\qquad
\frac{\omega_{\mathrm{NR}}}{k}\simeq\frac{p}{2m},\qquad
\frac{d\omega_{\mathrm{NR}}}{dk}\simeq\frac{p}{m}.
$$

This is exactly the [free-particle momentum convention](#free-particle-momentum-convention) used by the [Schrödinger equation](mathematical-physics.md#schrodinger-equation) here. Removing a common time-dependent [global phase](quantum-system.md#global-phase) changes the reported [phase velocity](dispersion-relation.md#phase-velocity), while leaving the [de Broglie wavelength](#de-broglie-wavelength), relative spatial [quantum phases](quantum-system.md#quantum-phase) and [group velocity](dispersion-relation.md#group-velocity) unchanged. Adding $mc^2$ again to a total [energy](energy.md) would count the [rest energy](special-relativity.md#rest-energy) twice.

### Thomson electron transmission diffraction experiment

↑ **Parent:** [Matter wave](#matter-wave)

Alongside the 1927 [Davisson–Germer experiment](quantum-scattering.md#davisson-germer-experiment), [George Paget Thomson](physicist.md#george-paget-thomson) developed an independent transmission test. [Alexander Reid](physicist.md#alexander-reid) first used celluloid; Thomson used thin metal films. A narrow [electron](physics.md#electron) beam crossed a film about $10^{-6}\,\mathrm{cm}$ thick, reaching a [photographic plate](optical-instrument.md#photographic-plate) perpendicular to the beam. Rings appeared. Accelerating [voltages](random-walk.md#voltage) of $20$–$60\,\mathrm{kV}$ set the [de Broglie wavelengths](#de-broglie-wavelength); metal structures known from [X-ray diffraction](quantum-scattering.md#x-ray-diffraction) allowed quantitative comparison. A downstream [magnetic field](magnetic-field.md) deflected ring-forming [electrons](physics.md#electron) like those passing through holes, identifying the carriers as [electrons](physics.md#electron) rather than [X-rays](electromagnetic-radiation.md#x-ray). Celluloid's uncertain structure limited its quantitative interpretation.[Nobel Lectures, Physics 1922–1941; Electronic waves, delivered 7 June 1938, printed pp. 398–400: films, plate, voltage range, metal comparison and magnetic control](physics-bibliography.md#nobel-lectures-physics-1922-1941/electronic-waves-by-george-paget-thomson)

The [Davisson–Germer experiment](quantum-scattering.md#davisson-germer-experiment) uses crystal reflection and angular [electric current](electric-charge.md#electric-current) scans; this transmission camera records a spatial pattern behind the specimen. Both probe [interference](physical-optics.md#interference-wave-propagation) in [electron diffraction](quantum-scattering.md#electron-diffraction), with different specimen preparations and readouts. A developed [photographic plate](optical-instrument.md#photographic-plate) records accumulated detections, not a direct image of the [wavefunction](wave-function.md).

Why rings? In an ideal film containing many small [crystals](thermodynamics.md#crystal) with uniformly distributed orientations, a family of [lattice planes](physical-chemistry.md#lattice-plane) with spacing $d$ can satisfy [Bragg's law](quantum-scattering.md#bragg-s-law) at every azimuth about the incident beam. First-order [elastic scattering](quantum-scattering.md#elastic-scattering) then forms a cone of opening half-angle $2\theta$, where $2d\sin\theta=\lambda$. A flat detector a distance $L$ downstream cuts this cone in a circle:

$$
R=L\tan(2\theta)
=L\tan\!\left[2\arcsin\!\left(\frac{\lambda}{2d}\right)\right]
\simeq\frac{L\lambda}{d}.
$$

The last expression requires small [scattering angles](quantum-scattering.md#scattering-angle). It explains a useful control: hold the specimen and camera distance fixed, increase accelerating [voltage](random-walk.md#voltage), and the ring radii should shrink with the [electron accelerating-voltage wavelength](#electron-accelerating-voltage-wavelength). It predicts positions, not intensities: preferred crystal orientations, film thickness and repeated [quantum scattering](quantum-scattering.md) can alter a real pattern.

For a chosen example, take $L=0.200\,\mathrm m$ and $d=0.200\,\mathrm{nm}$. The exact relativistic [electron accelerating-voltage wavelength](#electron-accelerating-voltage-wavelength) gives $\lambda=8.589\,\mathrm{pm}$ at $20\,\mathrm{kV}$ and $4.176\,\mathrm{pm}$ at $80\,\mathrm{kV}$. The corresponding exact ring radii are $8.594\,\mathrm{mm}$ and $4.176\,\mathrm{mm}$. These are calculated examples with chosen spacings and camera distance, not Thomson's measurements. The higher [voltage](random-walk.md#voltage) lies outside the range quoted from his lecture, deliberately illustrating a prediction rather than reconstructing his data.

<a id="image-calculated-electron-diffraction-rings-shrink-as-accelerating-voltage-increases"></a>
![](electron-transmission-diffraction-rings.png)

**[Figure 2](#image-calculated-electron-diffraction-rings-shrink-as-accelerating-voltage-increases). Calculated electron diffraction rings shrink as accelerating voltage increases**. [Source](electron-transmission-diffraction-rings.py). Original transmission geometry and calculated first-order ring positions for chosen plane spacings $0.200\,\mathrm{nm}$ and $0.140\,\mathrm{nm}$ at camera distance $L=0.200\,\mathrm m$. Both detector views have identical scales. Exact relativistic [de Broglie wavelengths](#de-broglie-wavelength) and $R=L\tan(2\theta)$ determine the radii; ring brightness and width are drawing choices. The geometry sketch exaggerates the [scattering angles](quantum-scattering.md#scattering-angle). No experimental data or borrowed diffraction photograph is plotted.

### Matter-wave interference

↑ **Parent:** [Matter wave](#matter-wave)

Matter-wave interference occurs when coherent spatial branches of a particle's [wavefunction](wave-function.md) recombine and their relative [quantum phase](quantum-system.md#quantum-phase) changes the detection probabilities.

### de Broglie wavelength

↑ **Parent:** [Matter wave](#matter-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/de_Broglie_wavelength)

The [de Broglie wavelength](#de-broglie-wavelength) is the distance over which a [matter wave](#matter-wave) accumulates one full spatial [quantum phase](quantum-system.md#quantum-phase) cycle in its propagation direction:

$$
\lambda=\frac{h}{|\mathbf p|}=\frac{2\pi}{|\mathbf k|},\qquad \mathbf p=\hbar\mathbf k,\qquad \hbar=\frac{h}{2\pi}.
$$

Here $h$ is the [Planck constant](quantum-mechanics.md#planck-constant), $\mathbf p$ is the [momentum](momentum.md), and $\mathbf k$ is the angular [wavevector](elasticity-physics.md#wavevector). The scalar $p$ in $\lambda=h/p$ means the positive [momentum](momentum.md) magnitude, not a signed component. Reversing a [momentum](momentum.md) reverses the [wavevector](elasticity-physics.md#wavevector) without making the [wavelength](wave-equation.md#wavelength) negative. At zero [momentum](momentum.md) there is no finite spatial phase period: the limiting [wavelength](wave-equation.md#wavelength) diverges.

This relation makes microscopic [diffraction](quantum-scattering.md#diffraction) accessible with particles: increasing the [momentum](momentum.md) shortens the [wavelength](wave-equation.md#wavelength) until it is comparable with the spacings in a [crystal scattering](quantum-scattering.md#crystal-scattering) problem. The [electron accelerating-voltage wavelength](#electron-accelerating-voltage-wavelength) gives a practical way to tune this scale, while the [Davisson–Germer experiment](quantum-scattering.md#davisson-germer-experiment) tests it by comparing [electron diffraction](quantum-scattering.md#electron-diffraction) directions with independently known crystal geometry. The same relation applies to neutral particles in a [neutron interferometer](#neutron-interferometer); [electric charge](electric-charge.md) is not a requirement for a [matter wave](#matter-wave).

The [wavelength](wave-equation.md#wavelength) belongs to the [wavefunction](wave-function.md), not to a sinusoidal path of a particle. A [free-particle momentum convention](#free-particle-momentum-convention) makes the distinction especially clear: a [plane wave](#plane-wave) has a rotating complex [quantum phase](quantum-system.md#quantum-phase) but a constant [probability density](#probability-density). A localized [wave packet](dispersion-relation.md#wave-packet) contains a range of [momenta](momentum.md) and therefore generally has a range of [wavelengths](wave-equation.md#wavelength), rather than one exact spatial period.

#### Free-particle momentum convention

↑ **Parent:** [de Broglie wavelength](#de-broglie-wavelength)

For a [free particle](quantum-mechanics.md#free-particle) of [mass](classical-mechanics.md#mass) $m>0$ in [nonrelativistic quantum mechanics](quantum-mechanics.md#nonrelativistic-quantum-mechanics), choose the [potential energy](energy.md#potential-energy) zero and write

$$
\psi(\mathbf r,t)=A\exp\!\left[\frac{i}{\hbar}(\mathbf p\cdot\mathbf r-Et)\right],\qquad E=\frac{|\mathbf p|^2}{2m},\qquad \omega=\frac{E}{\hbar}.
$$

Applying the [momentum operator](quantum-mechanics.md#momentum-operator) $-i\hbar\nabla$ returns $\mathbf p\psi$; this fixes the sign convention. The [angular frequency](lagrangian-mechanics.md#angular-frequency) is measured relative to this chosen [energy](energy.md) zero. Adding a constant [energy](energy.md) changes only a time-dependent [global phase](quantum-system.md#global-phase), leaving the spatial [de Broglie wavelength](#de-broglie-wavelength) unchanged. No rest-energy term is included in this [nonrelativistic quantum mechanics](quantum-mechanics.md#nonrelativistic-quantum-mechanics) convention.

The [plane wave](#plane-wave) has $|\psi|^2=|A|^2$ and [probability current](#probability-current) $\mathbf j=(\mathbf p/m)|A|^2$. Its real part can be drawn as a [sine](geometry-and-topology.md#sine) or [cosine](geometry-and-topology.md#cosine), but that graph is a component of a [probability amplitude](#probability-amplitude), not a transverse displacement. On infinite space this is a generalized [momentum eigenstate](energy-eigenvalue.md#momentum-eigenstate), not a state satisfying [wavefunction normalization](#wavefunction-normalization). A narrow [wave packet](dispersion-relation.md#wave-packet) instead moves with [group velocity](dispersion-relation.md#group-velocity) $\nabla_{\mathbf k}\omega=\mathbf p/m$; the [phase velocity](dispersion-relation.md#phase-velocity) $\omega/|\mathbf k|=|\mathbf p|/(2m)$ is not its transport speed.

The equality of [canonical momentum](hamiltonian-mechanics.md#canonical-momentum) and [kinetic momentum](quantum-theory.md#kinetic-momentum) here assumes a field-free region with the [magnetic vector potential](electromagnetism.md#magnetic-vector-potential) chosen zero. For a charged particle in a [magnetic field](magnetic-field.md), the [kinetic momentum](quantum-theory.md#kinetic-momentum) is $\boldsymbol\Pi=\mathbf p-q\mathbf A$. An arbitrary canonical phase gradient must not then be substituted into $m\mathbf v$; the [free particle](quantum-mechanics.md#free-particle) formula needs its stated assumptions.

#### Electron accelerating-voltage wavelength

↑ **Parent:** [de Broglie wavelength](#de-broglie-wavelength)

Let an [electron](physics.md#electron) start with negligible [kinetic energy](energy.md#kinetic-energy) and move through an increase $U>0$ in [electric potential](electric-field.md#electric-potential). Its [electric charge](electric-charge.md) is $q=-e$, where $e>0$ is the [elementary charge](electric-charge.md#elementary-charge), so the decrease in [potential energy](energy.md#potential-energy) is $eU$. In a field-free region after acceleration,

$$
K=eU,\qquad |\mathbf p|=\sqrt{2m_e eU},\qquad \lambda=\frac{h}{\sqrt{2m_e eU}}\simeq\frac{1.2264\,\mathrm{nm}}{\sqrt{U/(1\,\mathrm V)}}.
$$

This is an [electron](physics.md#electron) formula, not a universal conversion from [voltage](random-walk.md#voltage) to [wavelength](wave-equation.md#wavelength). It assumes negligible initial [kinetic energy](energy.md#kinetic-energy), negligible losses, and $eU\ll m_ec^2$, where $c$ is the [speed of light](special-relativity.md#speed-of-light). It describes the [de Broglie wavelength](#de-broglie-wavelength) outside the crystal; the [potential energy](energy.md#potential-energy) inside a material can change the local [kinetic momentum](quantum-theory.md#kinetic-momentum).

For $U=54\,\mathrm V$, take $h=6.62607015\times10^{-34}\,\mathrm{J\,s}$, $e=1.602176634\times10^{-19}\,\mathrm C$, and $m_e\simeq9.1093837\times10^{-31}\,\mathrm{kg}$. The rounded [electron](physics.md#electron) [mass](classical-mechanics.md#mass) is consistent with the 2022 recommended constants.[CODATA electron mass: numerical value and 2022 adjustment label](physics-bibliography.md#codata-value-electron-mass-by-national-institute-of-standards-and-technology)

$$
K=8.65175\times10^{-18}\,\mathrm J=54\,\mathrm{eV},\qquad
|\mathbf p|\simeq3.97019\times10^{-24}\,\mathrm{kg\,m\,s^{-1}},\qquad
\lambda\simeq1.66895\times10^{-10}\,\mathrm m=0.166895\,\mathrm{nm}.
$$

The [electronvolt](electronegativity.md#electronvolt) is an [energy](energy.md) unit: $54\,\mathrm{eV}$ must be converted to [joules](physics.md#joule) before combining it with $m_e$ in SI units. [Dimensional analysis](mathematical-physics.md#dimensional-analysis) checks both steps:

$$
[eU]=\mathrm{C\,V}=\mathrm J,\qquad [\sqrt{2m_e eU}]=\sqrt{\mathrm{kg\,J}}=\mathrm{kg\,m\,s^{-1}},\qquad [h/p]=\frac{\mathrm{J\,s}}{\mathrm{kg\,m\,s^{-1}}}=\mathrm m.
$$

The resulting [velocity](classical-mechanics.md#velocity) is about $4.3584\times10^6\,\mathrm{m\,s^{-1}}$, or $0.01454c$, so the nonrelativistic assumption is consistent. For a larger accelerating [voltage](random-walk.md#voltage), the [relativistic energy-momentum relation](special-relativity.md#energy-momentum-relation) gives $pc=\sqrt{K(K+2m_ec^2)}$, with $K=eU$, while $\lambda=h/p$ still holds. At $54\,\mathrm V$ the relativistic [wavelength](wave-equation.md#wavelength) is shorter by about $0.00264\%$.

Explicitly, the exact [special relativity](special-relativity.md) formula and its [nonrelativistic quantum mechanics](quantum-mechanics.md#nonrelativistic-quantum-mechanics) limit are

$$
\lambda_{\mathrm{rel}}(U)
=\frac{hc}{\sqrt{eU(eU+2m_ec^2)}}
=\frac{h}{\sqrt{2m_e eU}}\left(1+\frac{eU}{2m_ec^2}\right)^{-1/2}
\underset{eU\ll m_ec^2}{\simeq}\frac{h}{\sqrt{2m_e eU}}.
$$

Here $K=eU$ is the gained [kinetic energy](energy.md#kinetic-energy); the total [energy](energy.md) is $E=m_ec^2+K$. At $80\,\mathrm{kV}$, the [nonrelativistic quantum mechanics](quantum-mechanics.md#nonrelativistic-quantum-mechanics) expression gives $4.336\,\mathrm{pm}$, about $3.84\%$ larger than the exact $4.176\,\mathrm{pm}$. This difference matters when using [electron diffraction](quantum-scattering.md#electron-diffraction) ring positions to infer [lattice plane](physical-chemistry.md#lattice-plane) spacings.

<a id="image-de-broglie-wavelength-versus-momentum-and-electron-accelerating-voltage"></a>
![](de-broglie-wavelength-momentum-voltage.png)

**[Figure 3](#image-de-broglie-wavelength-versus-momentum-and-electron-accelerating-voltage). de Broglie wavelength versus momentum and electron accelerating voltage**. [Source](de-broglie-wavelength-momentum-voltage.py). Original formula plots. Left: $\lambda=h/p$, with $p$ the [momentum](momentum.md) magnitude. Right: the nonrelativistic [electron accelerating-voltage wavelength](#electron-accelerating-voltage-wavelength) for $10$–$500\,\mathrm V$ and negligible starting [kinetic energy](energy.md#kinetic-energy). Labels mark calculated examples, including $54\,\mathrm V$; no points represent experimental measurements. Quadrupling $U$ doubles $p$ and halves $\lambda$.

### Neutron interferometer

↑ **Parent:** [Matter wave](#matter-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neutron_interferometer)

A neutron interferometer coherently splits and recombines neutron matter waves, allowing path-dependent phases to be measured through the output intensity.

<h4 id="colella-overhauser-werner-experiment">Colella–Overhauser–Werner experiment</h4>

↑ **Parent:** [Neutron interferometer](#neutron-interferometer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Colella–Overhauser–Werner_experiment)

The Colella–Overhauser–Werner experiment observed the relative phase acquired by neutron paths at different heights in the Earth's gravitational field.

[https://doi.org/10.1103/PhysRevLett.34.1472](https://doi.org/10.1103/PhysRevLett.34.1472)

## Plane wave

↑ **Parent:** [Wave function](wave-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Plane_wave)

A plane wave has constant amplitude and a phase linear in space and time. It is a [momentum eigenstate](energy-eigenvalue.md#momentum-eigenstate) and is not spatially normalizable.

## Probability amplitude

↑ **Parent:** [Wave function](wave-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probability_amplitude)

A probability amplitude is a [complex number](complex-analysis.md#complex-number) that describes the contribution of a [pure state](quantum-theory.md#pure-state) to a specified measurement outcome. For a normalized [quantum state](quantum-system.md#quantum-state) $|\psi\rangle$ and a rank-one outcome associated with a normalized vector $|j\rangle$, it is the [inner product](inner-product.md) $a_j=\langle j|\psi\rangle$. The [Born rule](#born-rule) gives the corresponding [probability](probability-theory.md#probability) $p_j=|a_j|^2=a_j^*a_j$, using the [complex conjugate](complex-analysis.md#complex-conjugate). Thus an amplitude can be negative or complex, while a [probability](probability-theory.md#probability) is real and nonnegative. A [wavefunction](wave-function.md) is the analogous position amplitude: its squared [modulus](complex-analysis.md#modulus) gives a [probability density](#probability-density), which must be integrated over a region to obtain a [probability](probability-theory.md#probability). [Zwiebach, MIT 8.04, lecture 6, section 2, pp. 3–4](https://ocw.mit.edu/courses/8-04-quantum-physics-i-spring-2016/d87c768c4e1181fde8d4366112169719_MIT8_04S16_LecNotes6.pdf).

The extra information is the [quantum phase](quantum-system.md#quantum-phase). If $a=re^{i\theta}$, its [modulus](complex-analysis.md#modulus) $r$ fixes $|a|^2=r^2$, but its angle $\theta$ controls how it adds to another contribution. In the [complex plane](complex-analysis.md#complex-plane), picture amplitudes as arrows: add the arrows, then square the resulting length. For coherent contributions $A$ and $B$ to the same outcome,

$$
|A+B|^2=|A|^2+|B|^2+2\operatorname{Re}(A^*B).
$$

The last term is [interference](physical-optics.md#interference-wave-propagation). Adding [probabilities](probability-theory.md#probability) first loses it. Contributions with different relative [quantum phases](quantum-system.md#quantum-phase) can reinforce or cancel even when their individual squared [moduli](complex-analysis.md#modulus) are fixed.

For the [qubit](quantum-system.md#qubit) [quantum superposition](quantum-system.md#quantum-superposition) $|\psi_\phi\rangle=(\sqrt3/2)|0\rangle+(e^{i\phi}/2)|1\rangle$, project onto the plus vector of the [Hadamard basis](quantum-theory.md#hadamard-basis). By linearity, the two contributions combine as

$$
\langle+|\psi_\phi\rangle
=\underbrace{\frac{\sqrt3}{2\sqrt2}}_{A}
+\underbrace{\frac{e^{i\phi}}{2\sqrt2}}_{B}.
$$

Here $|A|^2=3/8$ and $|B|^2=1/8$, while the [interference](physical-optics.md#interference-wave-propagation) term is $(\sqrt3/4)\cos\phi$. At $\phi=0$, the arrows align and the plus [probability](probability-theory.md#probability) is $1/2+\sqrt3/4\simeq0.9330127$. At $\phi=\pi$, they oppose and that [probability](probability-theory.md#probability) is $1/2-\sqrt3/4\simeq0.0669873$; cancellation is incomplete because the lengths differ. At $\phi=\pi/2$, the arrows are perpendicular and the cross term vanishes. The minus amplitude uses $A-B$, reversing the cross term. These are alternate [projective measurements](quantum-measurement.md#projective-measurement) on identically prepared copies, rather than a sequence of measurements on one copy.

<a id="image-relative-quantum-phase-redistributes-hadamard-basis-probabilities-a-diagonal-mixture-stays-at-one-half"></a>
![](quantum-relative-phase-interference.png)

**[Figure 4](#image-relative-quantum-phase-redistributes-hadamard-basis-probabilities-a-diagonal-mixture-stays-at-one-half). Relative quantum phase redistributes Hadamard-basis probabilities; a diagonal mixture stays at one half**.

A [global phase](quantum-system.md#global-phase) multiplies every contribution by the same factor $e^{i\gamma}$, giving

$$
|\langle j|e^{i\gamma}\psi\rangle|^2
=|e^{i\gamma}\langle j|\psi\rangle|^2
=|\langle j|\psi\rangle|^2.
$$

It therefore changes no outcome [probability](probability-theory.md#probability). Changing a relative [quantum phase](quantum-system.md#quantum-phase) can change the angle between contributions and hence their [interference](physical-optics.md#interference-wave-propagation). Keeping amplitudes until the last step makes [quantum circuits](quantum-circuit.md) and [matter-wave interference](#matter-wave-interference) calculable; discarding their angles prematurely discards physically testable information. The [Born rule](#born-rule) example compares two measurement bases explicitly.

### Born rule

↑ **Parent:** [Probability amplitude](#probability-amplitude)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Born_rule)

The Born rule connects a [quantum state](quantum-system.md#quantum-state) to measurement [probabilities](probability-theory.md#probability). Let $\{|j\rangle\}$ be a complete [orthonormal basis](inner-product.md#orthonormal-basis), finite or countably infinite, for a [Hilbert space](hilbert-space.md), and let

$$
|\psi\rangle=\sum_j a_j|j\rangle,
\qquad
a_j=\langle j|\psi\rangle,
\qquad
\langle\psi|\psi\rangle=1.
$$

An ideal measurement distinguishing these basis vectors returns label $j$ with [probability](probability-theory.md#probability)

$$
p_j=|a_j|^2=|\langle j|\psi\rangle|^2.
$$

This assignment is a physical measurement rule. Its compatibility with total [probability](probability-theory.md#probability) one follows from [orthonormality](inner-product.md#orthonormal-set) and normalization:

$$
\sum_jp_j=\sum_j|a_j|^2
=\sum_{j,k}a_j^*a_k\langle j|k\rangle
=\langle\psi|\psi\rangle=1.
$$

The [probabilities](probability-theory.md#probability) are the squared [moduli](complex-analysis.md#modulus), not the amplitudes themselves or the squares $a_j^2$. [Watrous, IBM Quantum Learning, Quantum information, Measuring quantum states](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/single-systems/quantum-information).

If the basis is an [eigenbasis](linear-operator-theory.md#eigenbasis) of an [observable](quantum-system.md#observable), the reported numerical value is its [eigenvalue](linear-operator-theory.md#eigenvalue). Several vectors can share one [eigenvalue](linear-operator-theory.md#eigenvalue); the [probability](probability-theory.md#probability) of that value is then the sum over the corresponding basis labels. More generally, a [projective measurement](quantum-measurement.md#projective-measurement) with [orthogonal projections](hilbert-space.md#orthogonal-projection) $P_r$ assigns

$$
p_r=\langle\psi|P_r|\psi\rangle=\|P_r|\psi\rangle\|^2,
\qquad
p_r=\operatorname{Tr}(\rho P_r)
$$

for a [pure state](quantum-theory.md#pure-state) and a general [density matrix](density-matrix.md) $\rho$, respectively. This also covers [mixed states](density-matrix.md#mixed-state) and degenerate [eigenspaces](linear-operator-theory.md#eigenspace). The [Born rule](#born-rule) determines outcome statistics; the ideal conditional state change is specified separately by the [Lüders rule](quantum-measurement.md#luders-rule). See [projective measurement](quantum-measurement.md#projective-measurement) for that formulation and its assumptions. [Watrous, IBM Quantum Learning, Mathematical formulations of measurements, Projective measurements](https://quantum.cloud.ibm.com/learning/en/courses/general-formulation-of-quantum-information/general-measurements/formulations-of-measurements).

For a worked example, take the normalized [qubit](quantum-system.md#qubit) [quantum state](quantum-system.md#quantum-state)

$$
|\psi_\phi\rangle=\frac{\sqrt3}{2}|0\rangle+\frac{e^{i\phi}}2|1\rangle.
$$

The squared [moduli](complex-analysis.md#modulus) add to $3/4+1/4=1$. A [computational-basis measurement](quantum-theory.md#quantum-measurement-in-the-computational-basis), equivalently a measurement of the $Z$ [Pauli matrix](algebra.md#pauli-matrices), has

$$
p_0=\left|\frac{\sqrt3}{2}\right|^2=\frac34,
\qquad
p_1=\left|\frac{e^{i\phi}}2\right|^2=\frac14.
$$

These [probabilities](probability-theory.md#probability) do not depend on the relative [quantum phase](quantum-system.md#quantum-phase) $\phi$. Now choose the [Hadamard basis](quantum-theory.md#hadamard-basis)

$$
|\pm\rangle=\frac{|0\rangle\pm|1\rangle}{\sqrt2},
$$

whose vectors are [eigenstates](energy-eigenvalue.md#eigenstate) of the $X$ [Pauli matrix](algebra.md#pauli-matrices), also used by the [Pauli X gate](quantum-theory.md#pauli-x-gate). The new [probability amplitudes](#probability-amplitude) and [probabilities](probability-theory.md#probability) are

$$
b_\pm=\langle\pm|\psi_\phi\rangle
=\frac{\sqrt3\pm e^{i\phi}}{2\sqrt2},
\qquad
p_\pm=|b_\pm|^2
=\frac12\pm\frac{\sqrt3}{4}\cos\phi.
$$

Both [probabilities](probability-theory.md#probability) are nonnegative and their sum is one. The relative [quantum phase](quantum-system.md#quantum-phase) becomes visible because the two [probability amplitudes](#probability-amplitude) add before their squared [modulus](complex-analysis.md#modulus) is taken:
- At $\phi=0$, $p_+=(2+\sqrt3)/4\simeq0.9330127$ and $p_-\simeq0.0669873$.
- At $\phi=\pi/2$, $p_+=p_-=1/2$.
- At $\phi=\pi$, $p_+\simeq0.0669873$ and $p_-\simeq0.9330127$.

<a id="image-the-same-qubit-preparation-has-phase-independent-z-probabilities-and-phase-sensitive-x-probabilities"></a>
![](born-rule-basis-probabilities.png)

**[Figure 5](#image-the-same-qubit-preparation-has-phase-independent-z-probabilities-and-phase-sensitive-x-probabilities). The same qubit preparation has phase-independent Z probabilities and phase-sensitive X probabilities**.

A [Hadamard gate](quantum-theory.md#hadamard-gate) followed by a [computational-basis measurement](quantum-theory.md#quantum-measurement-in-the-computational-basis) realizes these $X$ statistics, since $H|\pm\rangle=|0\rangle,|1\rangle$, respectively. Compare the two bases using fresh, identically prepared copies: a preceding measurement may change the state. The [quantum superposition](quantum-system.md#quantum-superposition) section shows why replacing the preparation by the [mixed state](density-matrix.md#mixed-state) $\operatorname{diag}(3/4,1/4)$ keeps the $Z$ statistics but gives $p_+=p_-=1/2$ for every $\phi$.

The usefulness of the [Born rule](#born-rule) is this conversion from [linear algebra](linear-algebra.md) to experimental predictions: calculate overlaps in the basis actually measured, then take squared [moduli](complex-analysis.md#modulus). Its appealing geometry is that changing basis redistributes probability while preserving total squared [norm](normed-vector-space.md#norm). The same rule relates an [energy eigenstate](energy-eigenvalue.md#energy-eigenstate) expansion to an [energy measurement](#energy-measurement) and a position [wavefunction](wave-function.md) to a [probability density](#probability-density).

Born's 1926 paper on [quantum scattering](quantum-scattering.md) interpreted the outgoing-wave coefficients in terms of the [probabilities](probability-theory.md#probability) of collision outcomes; a corrective footnote specified proportionality to the square of the amplitude. This is a historical scattering formulation, rather than the general [density matrix](density-matrix.md) formula above. [Born, Zur Quantenmechanik der Stoßvorgänge, Zeitschrift für Physik 37, 863–867, 1926](physics-bibliography.md#zur-quantenmechanik-der-stossvorgange-by-max-born); [English translation of Born's paper, p. 3 and footnote 1](https://www.neo-classical-physics.info/uploads/3/0/6/5/3065888/born_-_qm_for_collisions_i.pdf).

#### Born statistical scattering interpretation

↑ **Parent:** [Born rule](#born-rule)

The scattering interpretation connects an incoming preparation to the relative frequency of outgoing directions and final atomic states. [Max Born](physicist.md#max-born)'s 1926 paper treats a distant incoming [electron](physics.md#electron) and a [chemical atom](physics.md#atom-physics), expands the outgoing [wavefunction](wave-function.md) into final atomic states, and imposes [conservation of energy](mathematical-physics.md#conservation-of-energy). Its translated correction footnote specifies the square of the coefficient; the modern [complex modulus](complex-analysis.md#complex-modulus) notation below is ours.[Zur Quantenmechanik der Stoßvorgänge, 1926, pp. 863–867; inspected in D. H. Delphenich's translation, pp. 2–4, especially p. 3 equation (1) and footnote 1: squared coefficient](physics-bibliography.md#zur-quantenmechanik-der-stossvorgange-by-max-born)

In his 11 December 1954 lecture, [Max Born](physicist.md#max-born) recalled the difficulty of interpreting bound [electrons](physics.md#electron) alone. He instead described an incident [electron](physics.md#electron) wave generating an outgoing spherical wave, with direction-dependent squared amplitude determining relative scattering probabilities. Distinct final atomic states describe excitation with corresponding [electron](physics.md#electron) [energy](energy.md) loss. This is a retrospective account of an interpretation, rather than the report of a new apparatus.[The statistical interpretation of quantum mechanics, lecture delivered 11 December 1954, printed pp. 261–262; inspected through the transcription at [https://studyres.com/doc/8624145/the-statistical-interpretation-of-quantum-mechanics,](https://studyres.com/doc/8624145/the-statistical-interpretation-of-quantum-mechanics,) paragraphs from the bound-electron difficulty through inelastic scattering](physics-bibliography.md#the-statistical-interpretation-of-quantum-mechanics-by-max-born)

The distinction from the modern [Born rule](#born-rule) matters. The historical question was which collision outcome occurs: a direction of motion and a final atomic state. The general [projective measurement](quantum-measurement.md#projective-measurement) formula applies to arbitrary [observables](quantum-system.md#observable), including degenerate outcomes and [mixed states](density-matrix.md#mixed-state); a [positive operator-valued measure](quantum-measurement.md#positive-operator-valued-measure) describes still more general detector statistics. Those formulations should not be read back as the explicit contents of the short 1926 scattering paper. Nor does the scattering interpretation itself supply a rule for the conditional [post-measurement state](quantum-measurement.md#post-measurement-state).

Actual experimental settings are described in the [Davisson–Germer experiment](quantum-scattering.md#davisson-germer-experiment) and the [Franck-Hertz experiment](energy-eigenvalue.md#franck-hertz-experiment). The former scans collected [electric current](electric-charge.md#electric-current) as an [electron](physics.md#electron) beam scatters from prepared [nickel](chemical-substance.md#nickel); changing direction, accelerating [voltage](random-walk.md#voltage) and surface preparation probes [electron diffraction](quantum-scattering.md#electron-diffraction). The latter uses acceleration through mercury vapor and a retarding collector to infer discrete [energy](energy.md) losses from current minima, with vapor density and retarding settings as controls. Angular resolution and surface backgrounds limit the first inference; initial [energy](energy.md) spread and collision positions limit the second. These linked experiments supply the preparation, apparatus and readout; the examples below are original calculations, not Born's measured data.

##### Angular scattering probability from complex amplitudes

↑ **Parent:** [Born statistical scattering interpretation](#born-statistical-scattering-interpretation)

Take [nonrelativistic quantum mechanics](quantum-mechanics.md#nonrelativistic-quantum-mechanics), a short-range interaction, a fixed heavy target, and a common projectile [mass](classical-mechanics.md#mass) $m$. An incoming [plane wave](#plane-wave) in atomic state $a$ has unit coefficient. In an open [scattering channel](quantum-scattering.md#scattering-channel) $i$, the target finishes in a normalized atomic state $\chi_i$, and the projectile has positive [velocity](classical-mechanics.md#velocity) magnitude $v_i=\hbar k_i/m$. At large distance,

$$
\Psi\sim e^{ik_a z}\chi_a+\sum_{i\,\mathrm{open}}f_{ia}(\Omega)\frac{e^{ik_i r}}r\chi_i,\qquad
\frac{\hbar^2k_i^2}{2m}+\varepsilon_i=\frac{\hbar^2k_a^2}{2m}+\varepsilon_a.
$$

Here $\Omega$ denotes direction, $d\Omega$ is a [solid angle](euclidean-geometry.md#solid-angle) element, and $\varepsilon_i$ is an internal atomic [energy](energy.md). Different $\chi_i$ are [orthogonal](inner-product.md#orthogonal-vectors). The [scattering amplitude](quantum-scattering.md#scattering-amplitude) $f_{ia}$ has units of length. A closed [scattering channel](quantum-scattering.md#scattering-channel) has no propagating outgoing [probability current](#probability-current) at this total [energy](energy.md).

The incoming [probability current](#probability-current) density is $j_{\mathrm{in}}=v_a$. The outgoing radial [probability current](#probability-current) density in channel $i$ is $j_{r,i}\sim v_i|f_{ia}|^2/r^2$. Multiplying by the area $r^2d\Omega$ and dividing by $j_{\mathrm{in}}$ gives the [differential scattering cross-section](quantum-scattering.md#differential-scattering-cross-section):

$$
\frac{d\sigma_i}{d\Omega}=\frac{v_i}{v_a}|f_{ia}(\Omega)|^2.
$$

The $r^{-2}$ dilution cancels the detector's area growth. The [velocity](classical-mechanics.md#velocity) ratio remains: a squared wave coefficient alone is not generally a flux fraction. A [differential scattering cross-section](quantum-scattering.md#differential-scattering-cross-section) has units of area per [solid angle](euclidean-geometry.md#solid-angle), rather than being a normalized directional [probability density](#probability-density). For selected scattering events in acceptance $D$, an ideal detector with equal efficiency in all retained channels instead gives

$$
\Pr(i,\Omega\in D\mid\text{selected scattering})
=\frac{\displaystyle\int_D(v_i/v_a)|f_{ia}|^2\,d\Omega}
{\displaystyle\sum_j\int_{\mathrm{selection}}(v_j/v_a)|f_{ja}|^2\,d\Omega}.
$$

The denominator specifies the event selection; it need not equal one square unit of area. Absolute rates require incident flux, target number and detector efficiency in addition to these relative weights. The next finite-mode model normalizes outgoing [probability current](#probability-current) to one incoming event and predicts event fractions directly.

##### Two-channel scattering with flux normalization

↑ **Parent:** [Born statistical scattering interpretation](#born-statistical-scattering-interpretation)

Consider one chosen model at a fixed total [energy](energy.md), with two open [scattering channels](quantum-scattering.md#scattering-channel), no absorption and no omitted outgoing modes. Channel 1 leaves the target unchanged; channel 2 excites it. Let $v_1=v>0$ and $v_2=v/2$. For the same projectile [mass](classical-mechanics.md#mass), [conservation of energy](mathematical-physics.md#conservation-of-energy) then requires a target excitation $\Delta=3mv^2/8$. These are hypothetical parameters, not a fit to a particular atom. Each incoming or outgoing mode is normalized to unit [probability current](#probability-current); the outgoing modes will have the angular profiles specified below.

Choose the [S-matrix](quantum-scattering.md#s-matrix)

$$
S=\frac15\begin{pmatrix}3&4i\\4i&3\end{pmatrix},\qquad
S^\dagger S=\frac1{25}\begin{pmatrix}25&12i-12i\\-12i+12i&25\end{pmatrix}=I.
$$

This phenomenological [unitary matrix](linear-operator-theory.md#unitary-matrix) specifies the channel conversion; it is not derived here from an interaction [potential energy](energy.md#potential-energy). For incidence in channel 1, its first column gives the outgoing flux amplitudes

$$
b=S\begin{pmatrix}1\\0\end{pmatrix}
=\begin{pmatrix}3/5\\4i/5\end{pmatrix},\qquad
P_1=\frac9{25},\quad P_2=\frac{16}{25}.
$$

To recover ordinary wave coefficients relative to an incident coefficient one, undo the [velocity](classical-mechanics.md#velocity) normalization:

$$
c_i=\sqrt{\frac{v_1}{v_i}}b_i,\qquad
c_1=\frac35,\quad c_2=\frac{4i\sqrt2}{5},\qquad
\sum_i\frac{v_i}{v_1}|c_i|^2=\frac9{25}+\frac12\frac{32}{25}=1.
$$

Thus $|c_2|^2=32/25>1$ is allowed: channel 2 travels more slowly. Its outgoing [probability current](#probability-current) fraction is $16/25$, not $32/25$. Renormalizing the unweighted squares would give $9/41$ and $32/41$, the wrong [probabilities](probability-theory.md#probability). More generally the ordinary coefficient map is $A=V^{-1/2}SV^{1/2}$, with $V=\operatorname{diag}(v,v/2)$; it obeys $A^\dagger VA=V$. The conserved quantity is the squared coefficient [norm](normed-vector-space.md#norm) weighted by [velocity](classical-mechanics.md#velocity), which represents [probability current](#probability-current).

Now specify an original angular realization of these two outgoing modes, with [scattering angle](quantum-scattering.md#scattering-angle) $\theta$ and no azimuth dependence:

$$
g_1(\theta)=\sqrt{\frac3{16\pi}}(1+i\cos\theta),\qquad
g_2(\theta)=\frac1{\sqrt{4\pi}},\qquad
\int|g_1|^2d\Omega=\int|g_2|^2d\Omega=1.
$$

The first normalization follows from $2\pi\int_{-1}^1(1+u^2)\,du=16\pi/3$, where $u=\cos\theta$. These angular profiles define the modes of this model; they are not asserted to follow from Born's approximation or an atomic [potential energy](energy.md#potential-energy). The joint directional [probability densities](#probability-density) are

$$
\frac{dP_1}{d\Omega}=\frac9{25}\frac3{16\pi}(1+\cos^2\theta),\qquad
\frac{dP_2}{d\Omega}=\frac{16}{25}\frac1{4\pi}.
$$

<a id="image-complex-angular-amplitudes-become-channel-resolved-scattering-intensity"></a>
![](born-scattering-complex-amplitude-angular-intensity.png)

**[Figure 6](#image-complex-angular-amplitudes-become-channel-resolved-scattering-intensity). Complex angular amplitudes become channel-resolved scattering intensity**. [Source](born-scattering-complex-amplitude-angular-intensity.py). Original two-channel model. Left: arrows in the [complex plane](complex-analysis.md#complex-plane) show $h(\theta)=1+i\cos\theta$, the angular factor of $g_1$. Right: the joint directional [probability densities](#probability-density) $P_i|g_i|^2$, per [solid angle](euclidean-geometry.md#solid-angle), retain the channel flux weights $9/25$ and $16/25$. The shaded interval is the cone $0\leq\theta\leq60^\circ$; its [probability](probability-theory.md#probability) requires the measure $2\pi\sin\theta\,d\theta$, not the area under a curve against degrees. These are chosen amplitudes, not historical measurements.

Suppose a detector accepts the cone $D:0\leq\theta\leq\pi/3$, with full azimuth and unit efficiency. Its angular fractions within the channels are

$$
F_1=\frac38\int_{1/2}^1(1+u^2)\,du=\frac{19}{64},\qquad
F_2=\frac12\int_{1/2}^1du=\frac14.
$$

Multiplying the angular fractions by the outgoing flux weights gives

$$
\Pr(1,D)=\frac9{25}\frac{19}{64}=\frac{171}{1600},\qquad
\Pr(2,D)=\frac{16}{25}\frac14=\frac{256}{1600}.
$$

For $1600$ independent incident events, the [expected values](expected-value.md) are therefore $171$ and $256$ accepted detections, compared with $576$ and $1024$ over all directions. The remaining expected $1173$ events fall outside the cone. The chosen incident number makes the expectations integers; actual counts fluctuate. Conditional on a detection inside the cone, the channel [probabilities](probability-theory.md#probability) are $171/427$ and $256/427$, rather than $9/25$ and $16/25$. Angular acceptance changes the observed channel proportions even with equal detector efficiencies.

<a id="image-velocity-weighting-and-angular-acceptance-determine-expected-channel-counts"></a>
![](born-scattering-channel-counts-weighted-flux.png)

**[Figure 7](#image-velocity-weighting-and-angular-acceptance-determine-expected-channel-counts). Velocity weighting and angular acceptance determine expected channel counts**. [Source](born-scattering-channel-counts-weighted-flux.py). Original model with $1600$ incident events. Left: raw squared wave coefficients $9/25$ and $32/25$ become conserved outgoing flux fractions $9/25$ and $16/25$ after multiplying by $v_i/v_1$. Right: all-direction expectations $576$ and $1024$ become $171$ and $256$ inside the $60^\circ$ cone. Bars show calculated [expected values](expected-value.md), not a generated sample or experimental counts.

The final atomic states are [orthogonal](inner-product.md#orthogonal-vectors), so ignoring the atomic readout adds the two channel intensities; it does not produce $|b_1g_1+b_2g_2|^2$. Coherent paths that reach the same final state can instead interfere, as the existing [probability amplitude](#probability-amplitude) and [quantum superposition](quantum-system.md#quantum-superposition) examples demonstrate. The distinction is physical distinguishability of final states, not whether the detector operator chooses to display their labels. Flux normalization and angular integration make the scattering interpretation useful: they turn complex outgoing waves into conserved event weights and then into the statistics of a specified detector.

#### Two-level quantum return probability

↑ **Parent:** [Born rule](#born-rule)

A normalized [quantum state](quantum-system.md#quantum-state) $\chi=\sqrt q\,\psi_1+e^{i\eta}\sqrt{1-q}\,\psi_2$ in two orthonormal [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) returns to its original one-dimensional measurement subspace with probability

$$
|\langle\chi,e^{-iHt/\hbar}\chi\rangle|^2=q^2+(1-q)^2+2q(1-q)\cos((E_1-E_2)t/\hbar).
$$

This follows by applying [unitary time evolution](quantum-system.md#unitary-time-evolution) to each [energy eigenstate](energy-eigenvalue.md#energy-eigenstate), then the [Born rule](#born-rule). The relative phase $\eta$ cancels from the return amplitude. Degenerate energies make the probability identically one.

#### Two-level observable transition probability

↑ **Parent:** [Born rule](#born-rule)

For two orthonormal [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) $\psi_1,\psi_2$, let an [observable](quantum-system.md#observable) have distinct nondegenerate [eigenstates](energy-eigenvalue.md#eigenstate) $\phi_\pm=(\psi_1\pm\psi_2)/\sqrt2$. Starting in $\phi_-$, [unitary time evolution](quantum-system.md#unitary-time-evolution) gives $(e^{-iE_1t/\hbar}\psi_1-e^{-iE_2t/\hbar}\psi_2)/\sqrt2$. Its [probability amplitude](#probability-amplitude) along $\phi_+$ is $(e^{-iE_1t/\hbar}-e^{-iE_2t/\hbar})/2$. The [Born rule](#born-rule) therefore gives the stated transition probability. The energy difference determines the oscillation frequency, while a common energy shift has no effect.

<h4 id="wigner-s-theorem">Wigner's theorem</h4>

↑ **Parent:** [Born rule](#born-rule)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wigner's_theorem)

Every bijection of pure-state rays that preserves transition probabilities is induced by either a unitary or an antiunitary operator on the Hilbert space.

##### Projective unitary representation

↑ **Parent:** [Wigner's theorem](#wigner-s-theorem)

Because state vectors differing by a [quantum phase](quantum-system.md#quantum-phase) represent the same ray, a unitary realization of a group action need only satisfy

$$
U(g_1)U(g_2)=e^{i\phi(g_1,g_2)}U(g_1g_2).
$$

A [projective unitary representation](#projective-unitary-representation) is a [projective representation](representation-theory.md#projective-representation) whose chosen representatives are unitary operators. The phase factors disappear on rays.

#### Energy measurement

↑ **Parent:** [Born rule](#born-rule)

An ideal energy measurement returns an eigenvalue of the Hamiltonian with probability equal to the squared norm of the state's projection onto its eigenspace. After obtaining a nondegenerate energy, the state is the corresponding energy eigenstate.

## Normalizable wavefunction

↑ **Parent:** [Wave function](wave-function.md)

A wavefunction is normalizable when the integral of its squared modulus is finite, so multiplication by a constant can make its total probability one.

## Probability density

↑ **Parent:** [Wave function](wave-function.md)

A probability density is a nonnegative [function](function.md) whose [integral](integral.md) over an event gives its probability.

### Radial probability density

↑ **Parent:** [Probability density](#probability-density)

The [radial probability density](#radial-probability-density) $P(r)$ is defined so that $P(r)\,dr$ is the probability of finding a particle between radii $r$ and $r+dr$. The spherical volume element gives $P(r)=r^2\int|\psi(r,\Omega)|^2d\Omega$. For a spherically symmetric [wavefunction](wave-function.md), $P(r)=4\pi r^2|\psi(r)|^2$; for $\psi=R(r)Y_l^m(\Omega)$ with normalized [spherical harmonics](analysis.md#spherical-harmonic), $P(r)=r^2|R(r)|^2$. Its maximum need not coincide with the maximum of the density per unit volume: a hydrogenic $1s$ state has its largest spatial density at the origin but its most probable radius at $a_0/Z$.

## Probability current

↑ **Parent:** [Wave function](wave-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probability_current)

For a nonrelativistic particle of mass $m$, the probability current is

$$
J=-\frac{i\hbar}{2m}
\left(\psi^*\nabla\psi-\psi\nabla\psi^*\right).
$$

### Probability current of a two-dimensional Dirac particle

↑ **Parent:** [Probability current](#probability-current)

For a Hermitian local mass coefficient and $H=c\boldsymbol\sigma\cdot\mathbf p+V\sigma_z$, the density and current obey $\partial_t(\Psi^\dagger\Psi)+\nabla\cdot(c\Psi^\dagger\boldsymbol\sigma\Psi)=0$. A normalized $\sigma_x=-1$ interface [spinor](algebra-over-a-field.md#spinor) carries $j_x=-c\rho$ and $j_y=0$.

### Probability continuity equation

↑ **Parent:** [Probability current](#probability-current)

For a [wavefunction](wave-function.md) satisfying the [Schrödinger equation](mathematical-physics.md#schrodinger-equation) with a real potential,

$$
\frac{\partial|\psi|^2}{\partial t}+\nabla\cdot J=0.
$$

This [continuity equation](mathematical-physics.md#continuity-equation) expresses local conservation of probability.

#### Conservation of quantum probability

↑ **Parent:** [Probability continuity equation](#probability-continuity-equation)

If the [probability current](#probability-current) of a [normalizable wavefunction](#normalizable-wavefunction) vanishes at spatial infinity, integrating the [probability continuity equation](#probability-continuity-equation) over all space shows that the total probability $\int |\psi|^2$ is constant in time.

## Gaussian wave packet

↑ **Parent:** [Wave function](wave-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_wave_packet)

A Gaussian wave packet is a [wavefunction](wave-function.md) whose spatial amplitude is a [Gaussian function](calculus.md#gaussian-function). Free quantum evolution preserves its Gaussian form while changing its complex width and spreading its [probability density](#probability-density).

### Gaussian covariance in a harmonic potential

↑ **Parent:** [Gaussian wave packet](#gaussian-wave-packet)

Under a [quantum harmonic oscillator](quantum-harmonic-oscillator.md) Hamiltonian, the [Heisenberg equations of motion](quantum-system.md#heisenberg-equation-of-motion) give

$$
x(t)=x(0)\cos\omega t+\frac{p(0)}{m\omega}\sin\omega t,\qquad p(t)=p(0)\cos\omega t-m\omega x(0)\sin\omega t.
$$

Subtract the [expectation values](quantum-system.md#expectation-value), square the first equation, and use the symmetrized [covariance](variance.md#covariance) $C_0=\langle\{x-\langle x\rangle,p-\langle p\rangle\}\rangle/2$. This yields

$$
\sigma_x(t)^2=\sigma_x(0)^2\cos^2\omega t+\frac{\sigma_p(0)^2}{m^2\omega^2}\sin^2\omega t+\frac{2C_0}{m\omega}\sin\omega t\cos\omega t.
$$

These moment equations hold for any state with finite second moments; a quadratic Hamiltonian additionally preserves [Gaussian wave packets](#gaussian-wave-packet). A [coherent state](quantum-theory.md#coherent-state) has $\sigma_x(0)^2=\hbar/(2m\omega)$, $\sigma_p(0)^2=m\hbar\omega/2$, and $C_0=0$, so its width stays fixed while its center follows the classical orbit. A [squeezed coherent state](quantum-harmonic-oscillator.md#squeezed-coherent-state) generally has a width that oscillates at $2\omega$.

### Free Gaussian wave packet evolution

↑ **Parent:** [Gaussian wave packet](#gaussian-wave-packet)

Let the initial [Gaussian wave packet](#gaussian-wave-packet) be

$$
\psi(x,0)=(2\pi\sigma_0^2)^{-1/4}\exp\left[-\frac{(x-x_0)^2}{4\sigma_0^2}+\frac{ip_0(x-x_0)}\hbar\right].
$$

Fourier transforming, multiplying each momentum amplitude by $e^{-ip^2t/(2m\hbar)}$ and evaluating the [Gaussian integral](integral.md#gaussian-integral) gives

$$
\psi(x,t)=\frac{(2\pi\sigma_0^2)^{-1/4}}{\sqrt{1+i\eta}}\exp\left[-\frac{(x-x_0-p_0t/m)^2}{4\sigma_0^2(1+i\eta)}+\frac{ip_0(x-x_0)}\hbar-\frac{ip_0^2t}{2m\hbar}\right],\qquad \eta=\frac{\hbar t}{2m\sigma_0^2}.
$$

Its [probability density](#probability-density) is a normalized Gaussian with center $x_0+p_0t/m$ and width $\sigma_x=\sigma_0\sqrt{1+\eta^2}$; the momentum width remains $\sigma_p=\hbar/(2\sigma_0)$. Its symmetrized position-momentum [covariance](variance.md#covariance) is $C_{xp}=t\sigma_p^2/m$, so

$$
\sigma_x\sigma_p=\frac\hbar2\sqrt{1+\eta^2},\qquad \sigma_x^2\sigma_p^2-C_{xp}^2=\frac{\hbar^2}4.
$$

Thus free spreading preserves equality in the [Robertson-Schrödinger uncertainty relation](quantum-theory.md#robertson-schrodinger-uncertainty-relation) while producing a nonzero quadratic position-dependent phase and a product $\sigma_x\sigma_p$ larger than $\hbar/2$. More generally, $\sigma_x(t)^2=\sigma_x(0)^2+2tC_{xp}(0)/m+t^2\sigma_p(0)^2/m^2$, so an initially correlated Gaussian can first contract.

### Gaussian evolution in an inverted harmonic oscillator

↑ **Parent:** [Gaussian wave packet](#gaussian-wave-packet)

For the [Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics) $H=(p^2-x^2)/2$, a [Gaussian wave packet](#gaussian-wave-packet) $Ae^{-Bx^2}$ satisfies $\dot A=-i\hbar AB$ and $\dot B=-i/(2\hbar)-2i\hbar B^2$. The displayed solution is normalizable for real $\phi$ exactly when $\sin(2\phi)>0$; its [second moments of a complex Gaussian wave packet](quantum-mechanics.md#second-moments-of-a-complex-gaussian-wave-packet) are

$$
\langle x^2\rangle=\frac{\hbar[\cosh(2t)+\cos(2\phi)]}{2\sin(2\phi)},\qquad
\langle p^2\rangle=\frac{\hbar[\cosh(2t)-\cos(2\phi)]}{2\sin(2\phi)}.
$$

Both grow as $\hbar e^{2t}/[4\sin(2\phi)]$, while their difference and hence the mean [energy](energy.md) remain constant.

## ↑ Ancestors (4)

1. [Quantum mechanics](quantum-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (25)

- [Aharonov-Bohm effect](topological-quantum-matter.md#aharonov-bohm-effect)
- [Anderson localization](wave.md#anderson-localization)
- [Ground-state overlap after sudden expansion of a square well](quantum-mechanics.md#ground-state-overlap-after-sudden-expansion-of-a-square-well)
- [Hartree equations](quantum-mechanics.md#hartree-equations)
- [Nobel Prize in Physics in 1954](nobel-prize-in-physics.md#nobel-prize-in-physics-in-1954)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2.md#19d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1.md#15g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2.md#16g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-59.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-62.md#4/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2019/paper-2.md#section-a-ii/15/i/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2019/paper-2.md#section-a-ii/15/ii/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-1.md#section-b/b6/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1.md#section-d/d13/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1.md#section-a/a1/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2014/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2017.md#1/a/solution)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2018.md#2/c/solution)
- [Phase shift of a delta-shell potential](quantum-scattering.md#phase-shift-of-a-delta-shell-potential)
- [Psi-epistemic model](foundations-of-quantum-mechanics.md#psi-epistemic-model)
- [Quantum propagator](quantum-system.md#quantum-propagator)
- [Spin-triplet p-wave pairing](statistical-physics.md#spin-triplet-p-wave-pairing)
- [Wannier-Mott exciton](quantum-mechanics.md#wannier-mott-exciton)
