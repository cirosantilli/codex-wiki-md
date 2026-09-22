# Group velocity

↑ **Parent:** [Phase velocity and group velocity](phase-velocity-and-group-velocity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_velocity)

The [group velocity](group-velocity.md) of a differentiable, real [dispersion relation](dispersion-relation.md) branch is

$$
\mathbf c_g=\nabla_{\mathbf k}\omega(\mathbf k_0),\qquad c_g=\frac{d\omega}{dk}(k_0)\ \text{in one dimension}.
$$

It describes the leading translation of a narrow-band [wave packet](wave-packet.md) centred on [wavevector](wavevector.md) $\mathbf k_0$, assuming a linear model, a locally uniform medium and negligible loss. Narrow-band means that the appreciably excited [wavevectors](wavevector.md) occupy a small neighbourhood on which one smooth branch can be linearized. Write its complex wavefield as

$$
\psi(\mathbf x,t)=\int a(\mathbf q)e^{i[(\mathbf k_0+\mathbf q)\cdot\mathbf x-\omega(\mathbf k_0+\mathbf q)t]}\,d\mathbf q.
$$

The [Taylor expansion](taylor-expansion.md) $\omega(\mathbf k_0+\mathbf q)\simeq\omega_0+\mathbf c_g\cdot\mathbf q$ gives

$$
\psi(\mathbf x,t)\simeq e^{i(\mathbf k_0\cdot\mathbf x-\omega_0t)}A(\mathbf x-\mathbf c_gt),\qquad A(\mathbf y)=\int a(\mathbf q)e^{i\mathbf q\cdot\mathbf y}\,d\mathbf q.
$$

Thus the rapid [wave phase](phase-waves.md) follows the [phase velocity](phase-velocity.md), while the slowly varying [wave envelope](envelope-waves.md) follows the [group velocity](group-velocity.md). This [Fourier analysis](fourier-analysis-split.md) argument is an outline of the approximation, rather than a statement that every [wave packet](wave-packet.md) translates rigidly forever. In one dimension a useful short-time condition is $|\omega''(k_0)|t(\Delta k)^2\ll1$, where $\Delta k$ is the characteristic spectral width; neglected higher derivatives must also remain small. Curvature of the [dispersion relation](dispersion-relation.md) eventually changes the [wave envelope](envelope-waves.md).[equations 9.9–9.16](pulse-propagation-by-richard-fitzpatrick.md)

Two nearby [plane waves](plane-wave.md) make the derivative visible without an integral. For equal [wave amplitudes](wave-amplitude.md) $a$, define $\bar k=(k_1+k_2)/2$, $\bar\omega=(\omega_1+\omega_2)/2$, $\Delta k=k_2-k_1$ and $\Delta\omega=\omega_2-\omega_1$. The [superposition principle](superposition-principle.md) gives the exact identity

$$
a\cos(k_1x-\omega_1t)+a\cos(k_2x-\omega_2t)=2a\cos\!\left(\frac{\Delta k\,x-\Delta\omega\,t}{2}\right)\cos(\bar kx-\bar\omega t).
$$

The periodic [wave envelope](envelope-waves.md) has speed $\Delta\omega/\Delta k$, approaching [group velocity](group-velocity.md) as the two [wavenumbers](wavenumber.md) coalesce, while the carrier [wave phase](phase-waves.md) has speed $\bar\omega/\bar k$. Two tones alone form an infinite beat train, not a localized [wave packet](wave-packet.md). The figure shows an exact two-tone [surface gravity wave](surface-gravity-wave.md) model with dimensionless $\omega=\sqrt{k}$: $k_1=0.9$, $k_2=1.1$. Its carrier [phase velocity](phase-velocity.md) is approximately $0.99875$, its finite-difference envelope velocity approximately $0.50063$, and $\omega'(1)=0.5$ is the limiting [group velocity](group-velocity.md). The marked carrier phase line need not coincide exactly with a maximum of the full modulated wave.

<a id="image-exact-analytical-two-tone-gravity-wave-model-carrier-phase-advances-through-a-slower-periodic-envelope"></a>
![](phase-group-dispersion-beats.png)

**[Figure 13](#image-exact-analytical-two-tone-gravity-wave-model-carrier-phase-advances-through-a-slower-periodic-envelope). Exact analytical two-tone gravity-wave model: carrier phase advances through a slower periodic envelope**.

The deep-water [surface gravity wave](surface-gravity-wave.md) therefore has $c_g=c_p/2$, whereas the deep-water [capillary wave](capillary-wave.md) limit has $c_g=3c_p/2$: crests can drift either forward or backward relative to a [wave envelope](envelope-waves.md). For finite-depth [surface gravity waves](surface-gravity-wave.md), differentiating the [dispersion relation](dispersion-relation.md) gives

$$
c_g=\frac{c_p}{2}\left(1+\frac{2kh}{\sinh(2kh)}\right),\qquad k>0.
$$

Here $\sinh$ is the [hyperbolic sine](hyperbolic-sine.md). The shallow-water limit has $c_g\simeq c_p\simeq\sqrt{gh}$; the deep-water limit has $c_g\simeq c_p/2$.[equations 6.8–6.11](free-surface-water-waves-13-012-hydrodynamics-for-ocean-engineers-reading-5-by-a-h-techet.md)

In the wave tank, produce a finite train with a smooth turn-on and turn-off and time the same [wave envelope](envelope-waves.md) feature at two probes separated by distance $L$; its transit estimate is $L/\Delta t$. Independently follow [wave crests](wave-crest.md) through that train. Techet's 2003 lab asks students to observe a deep-water train's foremost crest disappearing as the group moves forward, and to compare deep- and shallow-water cases. The interpretation is that a [wave crest](wave-crest.md) overtakes the slower [wave envelope](envelope-waves.md), dwindling at its front while other crests become visible at its rear. This is a qualitative expected observation in the teaching protocol, not a published set of measured curves.[Waves, phase speed, and group speed (13.012 Hydrodynamics for Ocean Engineers, Laboratory 1) by A. H. Techet](waves-phase-speed-and-group-speed-13-012-hydrodynamics-for-ocean-engineers-laboratory-1-by-a-h-techet.md)

A useful controlled version keeps the paddle [wave amplitude](wave-amplitude.md) small, records $h$ and $\lambda$, and checks both $ka\ll1$ and $a/h\ll1$. Compare runs with $kh\gg1$ and $kh\ll1$, rather than assuming every ripple tank is shallow relative to every [wavelength](wavelength.md). Increase train duration at fixed central [frequency](frequency.md) to narrow its spectrum, and check that the envelope transit estimate stabilizes. Calibrate both probes, sample fast enough to resolve the carrier, and compare records before reflected waves return; an absorbing beach reduces this contamination. A current changes laboratory velocities, large [wave amplitudes](wave-amplitude.md) introduce nonlinear effects, and very short [wavelengths](wavelength.md) require [surface tension](surface-tension.md). Strong [damping](damping.md) or noticeable reshaping makes the chosen threshold or peak an unreliable marker of simple [group velocity](group-velocity.md). These are proposed controls and model limits, not claims that the cited lab measured every correction.

Three velocities should consequently be kept separate. The [group velocity](group-velocity.md) predicts narrow-band [wave envelope](envelope-waves.md) motion. An energy-transport velocity is [energy flux](energy-flux.md) divided by [energy density](energy-density.md), using the appropriate time average; it agrees with [group velocity](group-velocity.md) in standard lossless linear wave models when all stored [energy](energy.md) is included.[Mathematical Methods in Nanophotonics, MIT 18.369, Spring 2016 — lectures 18–19 by Steven G. Johnson](mathematical-methods-in-nanophotonics-mit-18-369-spring-2016-lectures-18-19-by-steven-g-johnson.md) A signal-front velocity concerns the earliest response to a new disturbance and requires a causal model over its full spectrum. A strictly band-limited [wave packet](wave-packet.md) has no sharply bounded onset, and a mathematical two-tone envelope cannot test front arrival. In strongly absorbing or broadband propagation, a single [group velocity](group-velocity.md) need not describe the observed peak, energy transport, or first detectable response. A complex $\omega$ or $k$ also prevents interpreting its derivative as an ordinary real transport velocity without further analysis.

In particular, an unusually large or negative [group velocity](group-velocity.md) from pulse reshaping does not establish superluminal information transmission. For the causal dielectric model analysed by Fitzpatrick, the field ahead of the front vanishes for $t<x/c$, even when its [phase velocity](phase-velocity.md) exceeds the vacuum [speed of light](speed-of-light.md) $c$. That result concerns the electromagnetic model's [causality](causality.md); the ideal water-wave diagrams above contain no relativistic signal-front claim.[equations 871–873](wave-front-propagation-by-richard-fitzpatrick.md)

Finally, zero [wavenumber](wavenumber.md) requires care: the positive-frequency [wave equation](wave-equation-split.md) branch $c|k|$ is not differentiable at $k=0$, so it has no unique [group velocity](group-velocity.md) there, although its one-sided values are $\pm c$. A smooth gapped branch such as the [Klein-Gordon equation](klein-gordon-equation.md) instead has $\omega'(0)=0$ despite undefined [phase velocity](phase-velocity.md) at $k=0$. The same signed branch must be used in both derivatives and ratios; a negative [group velocity](group-velocity.md) means an envelope moving in the negative coordinate direction, not a negative elapsed time. The practical value of [group velocity](group-velocity.md) is precisely this translation between a local slope on a [dispersion diagram](dispersion-diagram.md) and a measurable packet transit, with its assumptions made explicit.

The [Gaussian envelope in a Klein-Gordon medium](gaussian-envelope-in-a-klein-gordon-medium.md) supplies a quantitative next step: the first [derivative](derivative.md) translates the [wave envelope](envelope-waves.md), the second [derivative](derivative.md) spreads it, and higher [derivatives](derivative.md) limit that approximation. At finite spectral width, a peak's measured speed need not equal the [group velocity](group-velocity.md) at the central [wavenumber](wavenumber.md). Neither a peak nor a fixed fraction of its height generally identifies [front velocity](front-velocity.md).

## ↑ Ancestors (8)

1. [Phase velocity and group velocity](phase-velocity-and-group-velocity.md)
2. [Dispersion relation](dispersion-relation.md)
3. [Wave equation](wave-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (175)

- [Absolute hydrodynamic instability](absolute-hydrodynamic-instability.md)
- [Absolute wavenumber](absolute-wavenumber.md)
- [Acoustic eikonal equation in a shear flow](acoustic-eikonal-equation-in-a-shear-flow.md)
- [Acoustic phonon branch](acoustic-phonon-branch.md)
- [Anisotropic absolute-instability threshold for positive diffusion](anisotropic-absolute-instability-threshold-for-positive-diffusion.md)
- [Bending wave of a Keplerian disk](bending-wave-of-a-keplerian-disk.md)
- [Birefringent walk-off](birefringent-walk-off.md)
- [Bloch oscillation](bloch-oscillation.md)
- [Boundary-forced internal gravity wave](boundary-forced-internal-gravity-wave.md)
- [Capillary length](capillary-length.md)
- [Causal envelope of stationary internal waves](causal-envelope-of-stationary-internal-waves.md)
- [Causal pressure adjustment by internal waves](causal-pressure-adjustment-by-internal-waves.md)
- [Circular mountain-wave ray in linear shear](circular-mountain-wave-ray-in-linear-shear.md)
- [Conduit equation](conduit-equation.md)
- [Critical-height approach of a stationary wave in linear shear](critical-height-approach-of-a-stationary-wave-in-linear-shear.md)
- [Dispersion diagram](dispersion-diagram.md)
- [Dispersion relation](dispersion-relation.md)
- [Dispersive swell source inversion](dispersive-swell-source-inversion.md)
- [Displacement pseudomomentum of an internal gravity wave](displacement-pseudomomentum-of-an-internal-gravity-wave.md)
- [Eikonal equation for a variable-speed wave](eikonal-equation-for-a-variable-speed-wave.md)
- [Elastic energy velocity](elastic-energy-velocity.md)
- [Elastic wave surface](elastic-wave-surface.md)
- [Electron hole](electron-hole.md)
- [First arrival of a stationary internal wavefront at a layer boundary](first-arrival-of-a-stationary-internal-wavefront-at-a-layer-boundary.md)
- [Free-particle momentum convention](free-particle-momentum-convention.md)
- [Front velocity](front-velocity.md)
- [Gaussian envelope in a Klein-Gordon medium](gaussian-envelope-in-a-klein-gordon-medium.md)
- [Geometrical optics](geometrical-optics.md)
- [Gravity-capillary wave](gravity-capillary-wave.md)
- [Group refractive index](group-refractive-index.md)
- [Group velocity](group-velocity.md)
- [Group-velocity minimum of a flexural-gravity wave](group-velocity-minimum-of-a-flexural-gravity-wave.md)
- [Group-velocity minimum of a high-contrast Love wave](group-velocity-minimum-of-a-high-contrast-love-wave.md)
- [Harmonic heating response of quasi-geostrophic flow](harmonic-heating-response-of-quasi-geostrophic-flow.md)
- [Information velocity](information-velocity.md)
- [Internal-wave envelope radiation condition](internal-wave-envelope-radiation-condition.md)
- [Internal-wave polarization](internal-wave-polarization.md)
- [Internal-wave ray tracing](internal-wave-ray-tracing.md)
- [Klein-Gordon packet velocities](klein-gordon-packet-velocities.md)
- [Long-wave transport along a depth step](long-wave-transport-along-a-depth-step.md)
- [Nondispersive wave](nondispersive-wave.md)
- [Opposite propagation directions in the annular displacement equation](opposite-propagation-directions-in-the-annular-displacement-equation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-43/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-47/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-48/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-49/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-54/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-58/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-72/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-72/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-74/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-74/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-75/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-78/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-78/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-73/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-73/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-73/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-75/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-75/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-75/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-76/5/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/37e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-80/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/37c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-77/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-82/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-2/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/37c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/37c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4/33a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-77/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-77/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-77/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/37b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-81/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-81/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/17a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/38a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-77/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-79/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/38a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-71/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-71/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-71/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-71/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/39b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/38b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-52/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-65/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-72/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-72/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-72/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-73/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-40/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-73/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-76/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/36b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3/37b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-74/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-74/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-79/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-321/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-330/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-330/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-330/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-331/3/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-331/3/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-333/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-336/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/18d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/33c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/38b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/38b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/38b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-331/3/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/35a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/40c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-333/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-333/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-333/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-345/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/34b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/38a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/38a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/38a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-333/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-333/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-345/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/39b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-321/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-333/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-345/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-321/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-341/section-b/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-345/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-345/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-336/1/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-333/3/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-342/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-345/2/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-345/2/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-345/1/b/solution.md)
- [Phase-group orthogonality for degree-zero dispersion](phase-group-orthogonality-for-degree-zero-dispersion.md)
- [Phase speed](phase-speed.md)
- [Phase velocity](phase-velocity.md)
- [Plane internal gravity wave](plane-internal-gravity-wave.md)
- [Quasi-geostrophic wave pseudomomentum](quasi-geostrophic-wave-pseudomomentum.md)
- [Ray tracing](ray-tracing.md)
- [Reflection of a Rossby wave at a meridional wall](reflection-of-a-rossby-wave-at-a-meridional-wall.md)
- [Refraction of a stationary internal-wave causal envelope](refraction-of-a-stationary-internal-wave-causal-envelope.md)
- [Right-triangle geometry of internal-wave velocities](right-triangle-geometry-of-internal-wave-velocities.md)
- [Rigid-base approximation to Love waves](rigid-base-approximation-to-love-waves.md)
- [Rigid-lid resonance of stationary topographic internal waves](rigid-lid-resonance-of-stationary-topographic-internal-waves.md)
- [Rossby-gravity waves](rossby-gravity-waves.md)
- [Rossby wave in a log-pressure atmosphere](rossby-wave-in-a-log-pressure-atmosphere.md)
- [Shallow-water Rossby-wave dispersion relation](shallow-water-rossby-wave-dispersion-relation.md)
- [Simple turning point of a variable-speed wave](simple-turning-point-of-a-variable-speed-wave.md)
- [Slowly modulated internal-wave boundary forcing](slowly-modulated-internal-wave-boundary-forcing.md)
- [Slowness](slowness.md)
- [Stationary internal-wave WKB solution](stationary-internal-wave-wkb-solution.md)
- [Stationary Rossby-wave ray envelope](stationary-rossby-wave-ray-envelope.md)
- [Stationary square-root-dispersion wake](stationary-square-root-dispersion-wake.md)
- [Surface-gravity-wave energy](surface-gravity-wave-energy.md)
- [Variational group velocity of a Taylor-Goldstein mode](variational-group-velocity-of-a-taylor-goldstein-mode.md)
- [Viscous attenuation of an internal gravity wave](viscous-attenuation-of-an-internal-gravity-wave.md)
- [Wave action (fluid dynamics)](wave-action-fluid-dynamics.md)
- [Wave-action transport for a variable-speed wave](wave-action-transport-for-a-variable-speed-wave.md)
- [Wave dispersion](wave-dispersion.md)
- [Wave packet](wave-packet.md)
- [Wave speed](wave-speed.md)
- [Wavefront](wavefront.md)
- [Waveguide phase and group velocities](waveguide-phase-and-group-velocities.md)
- [Wavelength](wavelength.md)
- [Wavenumber](wavenumber.md)
