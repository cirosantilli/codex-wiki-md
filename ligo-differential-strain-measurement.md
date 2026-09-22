# LIGO differential strain measurement

↑ **Parent:** [GW150914](gw150914.md)

Each [LIGO](ligo.md) instrument is a [Michelson interferometer](michelson-interferometer.md) with approximately $4\,\mathrm{km}$ arms containing [Fabry–Pérot interferometers](fabry-perot-interferometer.md). A stabilized $1064\,\mathrm{nm}$ [laser](laser-split.md) illuminates suspended $40\,\mathrm{kg}$ fused-silica mirrors in [vacuum](vacuum.md). Four-stage suspensions and active isolation suppress ground motion; low-loss materials reduce [thermal noise](thermal-noise.md). Power recycling increases circulating [power](power.md); signal recycling shapes the response to the [gravitational wave](gravitational-wave-split.md).[Sections 2–2.3, Table 1; 4.4 Test mass suspensions, Fig. 8; 4.5 Seismic isolation](advanced-ligo-by-j-aasi-and-others.md)

Why measure two perpendicular arms? In the long-[wavelength](wavelength.md) limit, take a [gravitational wave](gravitational-wave-split.md) with [plus polarization](plus-polarization.md) normally incident on ideal perpendicular arms. Its [transverse-traceless tensor](transverse-traceless-tensor.md) has $h_{xx}=h_+$ and $h_{yy}=-h_+$. Expanding each proper length to first order gives

$$
\frac{\delta L_x}{L}=\frac{h_+}{2},\qquad
\frac{\delta L_y}{L}=-\frac{h_+}{2},\qquad
\Delta L=\delta L_x-\delta L_y=Lh_+.
$$

Here $h_+$ is dimensionless, whereas $\Delta L$ is a [length](length.md). A stipulated $h_+=10^{-21}$ and $L=4000\,\mathrm m$ imply $\Delta L=4\times10^{-18}\,\mathrm m$, with individual arm changes of opposite sign and magnitude $2\times10^{-18}\,\mathrm m$. These are equivalent differential arm-length changes, not a photograph of mirrors moving against a rigid external ruler. The observable compares returning light phases; [coordinate systems](coordinate-system.md) can distribute the description between mirror coordinates and light propagation.

For unit arm directions $\mathbf u,\mathbf v$, define the detector [tensor](tensor.md) $D^{ij}=(u^iu^j-v^iv^j)/2$. If $e^+_{ij},e^\times_{ij}$ are the transverse polarization tensors, then

$$
h_D=D^{ij}h^{\rm TT}_{ij}=F_+h_++F_\times h_\times,\qquad
F_A=D^{ij}e^A_{ij}.
$$

The dimensionless factors $F_A$ encode sky direction and the polarization basis. Thus even identical sources can have different observed [amplitudes](wave-amplitude.md) and [wave phases](phase-waves.md). Motion changing both arms equally cancels in this ideal differential observable, although real asymmetries can couple common disturbances into it.

Suspension supplies an inertial reference above its resonances. For example, a single ideal [harmonic oscillator](simple-harmonic-motion.md) with support motion $y$ obeys $\ddot x+\omega_0^2(x-y)=0$. Its response at [angular frequency](angular-frequency.md) $\omega$ is $x/y=\omega_0^2/(\omega_0^2-\omega^2)$, which decreases in magnitude as $(\omega_0/\omega)^2$ well above resonance. The mirror follows slow support drift but approximately free motion in the high-frequency limit. Real multistage suspensions also require damping and alignment control; resonant frequencies are not regions of good isolation.

[Rainer Weiss](rainer-weiss.md)'s 1972 report proposed suspended masses, multiple-pass optical delay lines, and a servo holding an interference fringe. Its noise analysis separately treats photon-counting fluctuations, [laser](laser-split.md) frequency instability, mechanical [thermal noise](thermal-noise.md), [radiation pressure](radiation-pressure.md) and ground motion. Those delay lines should be distinguished from the resonant arm cavities of Advanced [LIGO](ligo.md).[Typeset transcription of 1972 report, sections 4–5.5, Fig. 1; original scan is linked from DCC record P720002](electromagnetically-coupled-broadband-gravitational-antenna-by-rainer-weiss.md)

**Table of contents**

- [LIGO displacement readout and control](ligo-displacement-readout-and-control.md)

## ↑ Ancestors (6)

1. [GW150914](gw150914.md)
2. [Gravitational wave](gravitational-wave-split.md)
3. [General relativity](general-relativity-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
