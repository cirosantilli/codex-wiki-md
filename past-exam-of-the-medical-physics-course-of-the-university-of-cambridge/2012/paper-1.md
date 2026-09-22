# Paper 1

↑ **Parent:** [2012](../2012.md)

Source: [Cambridge examination PDF, physical pages 477–478; printed paper 230](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1).

Biology and clinical applications are deferred in this draft. The generic mathematical, detector and wave-physics parts below are included.

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

TODO: Biology deferred at the user's request: the cancer-treatment account, clinical dose choices, treatment planning and clinical interpretation of the numerical model.

For the specified energy-loss model, multiply $dE/dx=-k/E$ by $2E$ and integrate from the entrance:

$$
\frac{d(E^2)}{dx}=-2k,\qquad
\boxed{E(x)^2=E_0^2-2kx.}
$$

The positive [stopping power](../../particle-detection.md#stopping-power) is $S=-dE/dx=k/E$. The model reaches zero [kinetic energy](../../energy.md#kinetic-energy) at

$$
\boxed{R=\frac{E_0^2}{2k}=\frac{200^2}{2(770)}\,\mathrm{cm}=25.97\,\mathrm{cm}.}
$$

At the entrance,

$$
\boxed{S(0)=\frac{770}{200}=3.85\,\mathrm{MeV\,cm^{-1}}.}
$$

Half a centimeter before the formal endpoint, $E^2=2k(0.5\,\mathrm{cm})=770\,\mathrm{MeV^2}$, so

$$
\boxed{E=27.75\,\mathrm{MeV},\qquad S=27.75\,\mathrm{MeV\,cm^{-1}}.}
$$

The signed derivatives are the negatives of the quoted [stopping powers](../../particle-detection.md#stopping-power). This [inverse-energy stopping-power model](../../particle-detection.md#inverse-energy-stopping-power-model) deposits [energy](../../energy.md) more strongly toward the endpoint. Its divergent endpoint derivative is integrable, giving finite total deposited [energy](../../energy.md) $E_0$; a real stopping curve includes finite [energy](../../energy.md) spread, range straggling, scattering and a more accurate low-energy stopping law. These numbers are consequences of the supplied ideal equation.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

TODO: Biology deferred at the user's request: clinical contrast interpretation, applications, and the head-injury MRI-versus-CT comparison.

The generic physics of [magnetic resonance imaging](../../nuclear-magnetic-resonance.md#magnetic-resonance-imaging) combines a main static magnet, radiofrequency transmit and receive coils, controlled [magnetic field gradients](../../magnetic-field.md#magnetic-field-gradient), signal electronics and reconstruction. A transverse radiofrequency pulse excites [nuclear spins](../../atomic-nucleus.md#nuclear-spin) near their Larmor [frequency](../../wave.md#frequency), $\omega_0=\gamma B_0$. The evolving transverse magnetization induces a received signal; [phase](../../wave.md#phase-waves) coherence and relaxation determine its time dependence.

Gradients encode [position](../../classical-mechanics.md#position) into [phase](../../wave.md#phase-waves). In a simplified homogeneous receive-sensitivity model,

$$
s(t)=\int\rho(\mathbf r)e^{-2\pi i\mathbf k(t)\cdot\mathbf r}\,d^3\mathbf r,
\qquad \mathbf k(t)=\frac{\gamma}{2\pi}\int^t\mathbf G(t')\,dt'.
$$

Here $\mathbf k$ is in cycles per unit length and $\gamma$ is in radians per second per tesla. Echo sign changes, pulse sequence timing and receive sensitivity belong in a more complete signal model. Sampling this [MRI k-space](../../nuclear-magnetic-resonance.md#magnetic-resonance-k-space) and reconstructing its data produces an image; the measured samples are not already real-space pixel values.

The physical signal depends on [spin](../../angular-momentum-operator.md#spin) density, longitudinal recovery and transverse dephasing. Timing changes their weighting. Static field inhomogeneity adds reversible dephasing beyond intrinsic [transverse relaxation](../../density-matrix.md#transverse-relaxation), motivating echo techniques and distinguishing $T_2^*$ from $T_2$. Those are physical signal mechanisms; their biological interpretation remains deferred.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

TODO: Biology deferred at the user's request: clinical registration applications and their validation requirements.

Generic [image registration](../../inverse-problem.md#image-registration) estimates a coordinate transformation aligning corresponding features in two images. A rigid transform permits translation and rotation, an affine transform additionally permits linear deformation, and a nonrigid model permits spatially varying displacement. The transformation class expresses assumptions about what changes between the acquisitions.

One can minimize a discrepancy between $I_1(T(\mathbf x))$ and $I_2(\mathbf x)$, using interpolated image values and an explicit [optimization](../../mathematical-optimization.md) procedure. Squared intensity differences suit some comparable acquisitions; [mutual information](../../information-theory.md#mutual-information) can compare statistical dependence when image contrasts differ. Landmarks, feature descriptors or additional geometric constraints provide other information. Smoothness or other [regularization](../../statistical-learning.md#regularization) controls overly flexible transformations. A favorable objective value does not by itself prove correct feature correspondence.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

TODO: Biology deferred at the user's request: biological radiation effects and clinical risk assessment.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

In [pulse-echo ultrasound](../../fluid-mechanics.md#pulse-echo-ultrasound), a transducer emits a pulse and records returning echoes. For a straight round-trip path in a medium of assumed [sound speed](../../compressible-flow.md#speed-of-sound) $c$, an echo delay $t$ gives depth $z=ct/2$. [Reflections](../../linear-algebra.md#reflection-mathematics) depend on acoustic-impedance changes, while attenuation, scattering and propagation geometry affect the received amplitude.

An [A-mode ultrasound scan](../../fluid-mechanics.md#a-mode-ultrasound-scan) displays echo amplitude against inferred depth along one beam. A [B-mode ultrasound scan](../../fluid-mechanics.md#b-mode-ultrasound-scan) maps received amplitude to brightness and assembles many beam directions or translated beam lines into a spatial image. An [M-mode ultrasound scan](../../fluid-mechanics.md#m-mode-ultrasound-scan) repeats one beam line and displays its depth profile versus time, making motion along that line visible. Thus the display axes and acquisition pattern differ even when the pulse-echo principle is shared.

For a pulse lasting $\tau_p$, a simple axial-separation estimate is $c\tau_p/2$. Lateral resolution depends on aperture, wavelength, focusing and depth. Shorter pulses and broader bandwidth can improve axial resolution; an assumed [sound speed](../../compressible-flow.md#speed-of-sound) or a multiple-reflection path can instead misplace an echo. Brightness is not a direct universal map of composition.

[Doppler ultrasound](../../fluid-mechanics.md#doppler-ultrasound) uses [frequency](../../wave.md#frequency) or pulse-to-pulse [phase](../../wave.md#phase-waves) changes from moving scatterers. In a simple backscatter geometry, $\Delta f\simeq2f_0v\cos\theta/c$. Inferring [speed](../../classical-mechanics.md#speed) requires the beam-to-motion angle; pulsed sampling can alias frequencies, and an unknown angle leaves a velocity-projection ambiguity. This describes generic acoustic acquisition rather than a clinical diagnosis.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

TODO: Biology deferred at the user's request: biological tracer behavior and clinical PET applications.

The generic physics of [positron emission tomography](../../inverse-problem.md#positron-emission-tomography) uses [electron-positron annihilation](../../relativistic-quantum-field.md#electron-positron-annihilation). A slowly moving electron-positron pair predominantly produces two nearly opposite [photons](../../quantum-mechanics.md#photon) with [energy](../../energy.md) close to $m_ec^2=511\,\mathrm{keV}$ each. A ring of detectors records approximately simultaneous interactions; a coincidence identifies a [coincidence line of response](../../inverse-problem.md#coincidence-line-of-response) along which an annihilation could have occurred. Finite [Positron](../../physics.md#positron) travel before annihilation and nonzero pair [momentum](../../momentum.md) limit how directly this line identifies the original emission location.

Many such measurements constrain an emission distribution through a [tomography](../../inverse-problem.md#tomography) model. Attenuation, scattered coincidences, unrelated random coincidences, finite detector resolution and dead time alter the observed counts and require [calibration](../../differential-geometry.md#calibration-differential-geometry) or modeling. With useful time-of-flight information, the arrival-time difference further localizes [position](../../classical-mechanics.md#position) along the line: a timing uncertainty $\delta t$ corresponds to a [position](../../classical-mechanics.md#position) scale $c\delta t/2$. The coincidence data therefore provide spatial constraints, rather than each event directly supplying a complete three-dimensional image point.

## ↑ Ancestors (11)

1. [2012](../2012.md)
2. [Past exam of the medical physics course of the University of Cambridge](../../past-exam-of-the-medical-physics-course-of-the-university-of-cambridge.md)
3. [Medical Physics course of the University of Cambridge](../../university-of-cambridge.md#medical-physics-course-of-the-university-of-cambridge)
4. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
