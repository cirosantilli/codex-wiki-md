# LIGO displacement readout and control

↑ **Parent:** [LIGO differential strain measurement](ligo-differential-strain-measurement.md)

An ideal single-round-trip [Michelson interferometer](michelson-interferometer.md) converts differential [length](length.md) into [phase difference](phase-difference.md) $\delta\phi=4\pi\Delta L/\lambda$. If its dark-port [power](power.md) scale is $P_0$ and its static phase offset is $\phi_0$, then

$$
P_{\rm out}=P_0\sin^2\!\left(\frac{\phi_0+\delta\phi}{2}\right),\qquad
\delta P=\frac{P_0}{2}\sin\phi_0\,\delta\phi+O(\delta\phi^2).
$$

Exactly at a dark fringe, $\phi_0=0$, [power](power.md) is quadratic in small [displacement](displacement.md) and loses its sign. A deliberate offset supplies an optical reference field: interference with the small signal field produces a linear term. Equivalently, $|E_{\rm ref}+E_{\rm sig}|^2$ contains $2\operatorname{Re}(E_{\rm ref}^*E_{\rm sig})$. The [photodetector](photodetector.md) measures [power](power.md), not a signed [displacement](displacement.md) directly.

Advanced [LIGO](ligo.md) uses this DC homodyne principle with a small differential arm offset and an output mode cleaner. Its [feedback control](closed-loop-control.md) maintains optical resonance and alignment, using actuation distributed over the suspension stages.[2.3 Gravitational wave readout; 4.4.2 Quadruple pendulum design; 4.8 Interferometer sensing and control](advanced-ligo-by-j-aasi-and-others.md) The simple formula above omits resonant storage: arm and recycling cavities give a frequency-dependent optical gain and delay, so no constant pass-count multiplier describes the entire observing band.

To see why a locked detector can still measure a disturbance, use a linear [feedback control](closed-loop-control.md) model. Let $x_{\rm ext}$ be the external differential [displacement](displacement.md), $d_{\rm err}$ the residual readout, $d_{\rm ctrl}$ the recorded control command, $C(f)$ the sensing response and $A(f)$ the actuation response. With the convention $x_{\rm res}=x_{\rm ext}-A d_{\rm ctrl}$, reconstruction gives

$$
\widetilde x_{\rm ext}=C^{-1}\widetilde d_{\rm err}+A\widetilde d_{\rm ctrl},\qquad
\widetilde h_D=\widetilde x_{\rm ext}/L.
$$

Here tildes denote [Fourier transforms](fourier-transform-split.md); $C$ has readout units per metre and $A$ metres per command unit. Feedback suppresses residual motion but records the compensating command. Omitting that command would suppress the reconstructed low-frequency signal too. In the actual [GW150914](gw150914.md) experiment, a modulated auxiliary [laser](laser-split.md) exerted calibrated [radiation pressure](radiation-pressure.md) on a mirror to measure the response; periodic excitations monitored calibration.[II Control loop, equations (1)–(4); IV Photon calibrator; VII Time-dependent systematic errors](calibration-of-the-advanced-ligo-detectors-for-the-discovery-of-the-binary-black-hole-merger-gw150914-by-b-p-abbott-and-others.md)

<a id="image-from-differential-arm-length-to-optical-power-and-reconstructed-gravitational-wave-strain"></a>
![](ligo-differential-strain-readout-control.png)

**[Figure 1](#image-from-differential-arm-length-to-optical-power-and-reconstructed-gravitational-wave-strain). From differential arm length to optical power and reconstructed gravitational wave strain**. Original functional schematic, not a scale drawing. Upper panel: instrument components. Lower panel: ideal linear feedback reconstruction from residual error and applied control.

## ↑ Ancestors (7)

1. [LIGO differential strain measurement](ligo-differential-strain-measurement.md)
2. [GW150914](gw150914.md)
3. [Gravitational wave](gravitational-wave-split.md)
4. [General relativity](general-relativity-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
