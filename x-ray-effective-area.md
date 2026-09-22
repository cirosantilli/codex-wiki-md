# X-ray effective area

↑ **Parent:** [X-ray astronomy](x-ray-astronomy.md)

[X-ray effective area](x-ray-effective-area.md) is the area that converts an incident [photon](photon.md) arrival rate per unit area into an accepted count rate. For a fixed direction and a sufficiently narrow [energy](energy-split.md) interval, write

$$
A_{\mathrm{eff}}=A_{\mathrm{geom}}T\eta\epsilon_s,\qquad N_s=F A_{\mathrm{eff}}t.
$$

Here $A_{\mathrm{geom}}$ is projected geometric area, $T$ is [transmittance](transmittance.md) through windows or optics, $\eta$ is [quantum efficiency](quantum-efficiency.md), $\epsilon_s$ is the probability that a detected source event passes event selection, and $t$ is live observing time. $N_s$ is an [expected value](expected-value-split.md), not a guarantee of an integer count. Multiplication follows by counting incident [photons](photon.md) over area and time, then applying the successive conditional acceptance probabilities. Live time already excludes intervals when the instrument cannot record events; multiplying by a live-time fraction again would count the same loss twice.

For an invented narrow-band example, choose $A_{\mathrm{geom}}=40\,\mathrm{cm^2}$, $T=0.8$, $\eta=0.75$, and $\epsilon_s=5/6$. Then $A_{\mathrm{eff}}=20\,\mathrm{cm^2}$. A source with $F=0.30\,\mathrm{photons\,cm^{-2}\,s^{-1}}$ observed for $t=100\,\mathrm{s}$ gives $N_s=600$. $F$ here counts [photons](photon.md); converting it into [observed radiative flux](observed-radiative-flux.md) requires their [energies](energy-split.md). If all have [energy](energy-split.md) $E_0$, the corresponding [radiative flux](radiative-flux.md) is $E_0F$.

A broad [spectrum](spectrum-functional-analysis.md) instead requires

$$
N_s=t\int F_E(E)A_{\mathrm{eff}}(E)\,\mathrm{d}E,
$$

where $F_E$ is the differential [photon](photon.md) arrival rate per area and [energy](energy-split.md). A single band-averaged [X-ray effective area](x-ray-effective-area.md) depends on the assumed [spectrum](spectrum-functional-analysis.md). This is why a count rate alone cannot give an assumption-free [radiative flux](radiative-flux.md).

**Table of contents**

- [On-off X-ray photon counting](on-off-x-ray-photon-counting.md)

## ↑ Ancestors (6)

1. [X-ray astronomy](x-ray-astronomy.md)
2. [Observational astronomy](observational-astronomy.md)
3. [Astrophysics](astrophysics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [1962 rocket discovery of cosmic X-ray sources](1962-rocket-discovery-of-cosmic-x-ray-sources.md)
- [Grazing-incidence X-ray optics](grazing-incidence-x-ray-optics.md)
- [On-off X-ray photon counting](on-off-x-ray-photon-counting.md)
- [X-ray effective area](x-ray-effective-area.md)
