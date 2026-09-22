# Double heterostructure laser

↑ **Parent:** [Double heterostructure](double-heterostructure.md)

A [double heterostructure laser](double-heterostructure-laser.md) electrically pumps its central layer for [stimulated emission](stimulated-emission.md). [Band offsets](band-offset.md) confine [charge carriers](charge-carrier.md); [refractive index](refractive-index.md) contrast confines the optical [normal mode](normal-mode.md).[§II, Fig. 1, p. 768](nobel-lecture-the-double-heterostructure-concept-and-its-applications-in-physics-electronics-and-technology-by-zhores-ivanovich-alferov.md)

<a id="image-chosen-type-i-band-alignment-carrier-injection-and-optical-readout"></a>
![](semiconductor-heterostructure-band-injection.png)

**[Figure 5](#image-chosen-type-i-band-alignment-carrier-injection-and-optical-readout). Chosen type-I band alignment: carrier injection and optical readout**. [Source](semiconductor-heterostructure-band-injection.py). Original schematic using stipulated [energy](energy-split.md) units. The upper panel plots electron [energy band](energy-band.md) edges across the layers; the lower panel separates electrical pumping from the emerging [light](light.md). Flat segments omit [band bending](band-bending.md). The curves do not reproduce a historical device.

For an original bookkeeping model, let $R$ be the injected pair rate per unit area, $d$ the active-layer thickness, $N$ its excess pair [number density](number-density.md), $\tau$ a recombination lifetime, and $\tau_e$ an escape time. Before appreciable [stimulated emission](stimulated-emission.md), suppose

$$
\frac{dN}{dt}=\frac{R}{d}-\frac{N}{\tau}-\frac{N}{\tau_e},\qquad
N_{\rm ss}=\frac{R\tau}{d}\frac{1}{1+\tau/\tau_e}.
$$

Choose two otherwise identical devices with $\tau_e=\tau$ and $\tau_e=9\tau$. The resulting [steady state](steady-state.md) populations are $R\tau/(2d)$ and $9R\tau/(10d)$: improved confinement raises the population by a factor $1.8$ at fixed injection. This linear model assumes equal excess [electron](electron.md) and [electron hole](electron-hole.md) densities, fixed lifetimes, and no [laser gain clamping](laser-gain-clamping.md).

Optical confinement enters separately. For a chosen optical [normal mode](normal-mode.md), define $0<\Gamma\leq1$ as its gain-overlap factor with the active layer. With material [optical gain](optical-gain.md) $g$, internal loss $\alpha_i$, and mirror loss $\alpha_m$, a simple [laser threshold](laser-threshold.md) condition is

$$
\Gamma g=\alpha_i+\alpha_m.
$$

For stipulated losses $\alpha_i+\alpha_m=3$ in inverse-length units, $\Gamma=1/2$ requires $g=6$, whereas $\Gamma=3/4$ requires $g=4$. This calculation varies optical overlap only; the preceding population calculation varies carrier escape only. Their combination explains the usefulness of controlling both the [energy band](energy-band.md) profile and the optical [normal mode](normal-mode.md).

[Herbert Kroemer](herbert-kroemer.md) proposed the [double heterostructure laser](double-heterostructure-laser.md) in 1963; he did not participate in its 1970 experimental realization.[§IV, p. 787](nobel-lecture-quasielectric-fields-and-band-offsets-teaching-electrons-new-tricks-by-herbert-kroemer.md) [Zhores I. Alferov](zhores-ivanovich-alferov.md) describes his group's independent 1963 proposal and later experimental program.[§II, pp. 768–770](nobel-lecture-the-double-heterostructure-concept-and-its-applications-in-physics-electronics-and-technology-by-zhores-ivanovich-alferov.md)

**Table of contents**

- [Continuous double heterostructure laser experiment](continuous-double-heterostructure-laser-experiment.md)

## ↑ Ancestors (5)

1. [Double heterostructure](double-heterostructure.md)
2. [Semiconductor heterostructure](semiconductor-heterostructure.md)
3. [Semiconductor](semiconductor-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Continuous double heterostructure laser experiment](continuous-double-heterostructure-laser-experiment.md)
- [Double heterostructure laser](double-heterostructure-laser.md)
- [Finite-well confinement in a semiconductor heterostructure](finite-well-confinement-in-a-semiconductor-heterostructure.md)
