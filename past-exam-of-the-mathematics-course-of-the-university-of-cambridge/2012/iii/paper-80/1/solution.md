<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [oil spill under sea ice](../../../../../oil-spill-under-sea-ice.md) first reaches the underside through [buoyancy](../../../../../buoyancy.md). Oil droplets and gas bubbles rise relative to the surrounding water; their collective [buoyancy](../../../../../buoyancy.md) drives an entraining [buoyant plume](../../../../../buoyant-plume.md), while ocean currents bend the plume and carry small droplets away. Droplet size matters: small droplets rise slowly and can be dispersed or partly dissolved before arriving, whereas coalescence produces faster-rising drops. Gas expansion, dissolution and the ambient [density stratification](../../../../../density-stratification.md) change the plume on its ascent. Consequently the arrival footprint can be displaced from the well, and the oil arrival rate at the ice need not equal the discharge rate at the seabed.

The combinations of cover and motion give four distinct collection geometries. Each must then be combined with the four age-and-relief cases below; this accounts for all sixteen combinations without treating age as a substitute for geometry.

- Under continuous [fast ice](../../../../../fast-ice.md), the receiving underside stays near the source. Oil accumulates locally, spreads laterally along the ice–water interface and can fill successively higher buoyant traps. Currents can still transport it beneath the stationary cover.
- Under continuous moving [sea ice](../../../../../sea-ice.md), different parts of the underside cross the arrival footprint. Oil adhering to, or trapped beneath, an [ice floe](../../../../../ice-floe.md) is exported with it; oil remaining mobile relative to the ice is also transported by currents. The balance of arrival and the fresh underside passing the source determines whether deposition is continuous.
- With broken but anchored [fast ice](../../../../../fast-ice.md), oil can collect beneath separate stationary pieces, escape around their edges into leads, or encounter another piece downstream. The exposed water allows evaporation and wave-driven dispersion that are restricted beneath an unbroken cover. Here “fast” means anchored pieces, rather than freely drifting fragments.
- With broken moving [ice floes](../../../../../ice-floe.md), there is both intermittent capture by passing floes and intermittent direct surfacing in the gaps. Collisions, overturning and changing leads redistribute oil between undersides, floe edges and open water; the contaminated floes can travel far from the discharge.

For each of these four geometries, the age-and-relief combinations have the following effects.

- Smooth [first-year sea ice](../../../../../first-year-sea-ice.md) supports a thin spreading lens. Its saline pore network can later provide a route into the ice when connected brine channels open; a cold, poorly connected network can initially exclude oil.
- Deformed [first-year sea ice](../../../../../first-year-sea-ice.md) has upward recesses, ridge keels and rubble interstices that partition the lens into reservoirs. Locally much thicker oil can be stored, and liquid-filled interstices can provide routes into a ridge. The available connected storage volume matters more than the flat-interface lens thickness.
- Smooth [multi-year sea ice](../../../../../multi-year-sea-ice.md) still obeys the flat-interface capillary balance wherever the receiving surface is flat. Its previous drainage and melt history changes pore salinity and connected pathways, so its incorporation behaviour need not match saline young ice.
- Deformed [multi-year sea ice](../../../../../multi-year-sea-ice.md) combines old ridge and melt topography with a repeatedly modified pore structure. Oil can be retained in deep underside pockets and redistributed when the floe melts, cracks or overturns. Neither age class is invariably more permeable: temperature, liquid fraction and connectivity control the [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md).

Thus deformation increases local storage in either age class; motion changes residence time and export in either geometry; and gaps permit direct surfacing in either stationary or moving ice. These distinctions remain important even when two covers have the same mean thickness.

During growth, new [sea ice](../../../../../sea-ice.md) can form around the edges of a lens or at available water-contacting surfaces and enclose oil between successive layers. Oil interrupts direct ice–water contact and changes thermal resistance, so incorporation is not simply freezing a pure oil layer. Oil droplets can be caught in a growing skeletal layer, and connected brine channels allow upward migration when [buoyancy](../../../../../buoyancy.md) overcomes capillary entry resistance. In spring, warming increases the liquid fraction and opens pathways; meltwater and brine circulation can redistribute oil internally. Oil can then reach the surface and [melt ponds](../../../../../melt-pond.md), darken the ice, or be released to open water when the enclosing ice disappears. Thick ridge pockets may survive longer than flat lenses. The coupling between brine drainage, warming and oil migration is documented by [field observations of oil entrainment in first-year ice](https://doi.org/10.3189/S0022143000014477).

A shorter freezing season gives less time for encapsulation and long-term storage. Less [multi-year sea ice](../../../../../multi-year-sea-ice.md), greater open-water exposure and earlier breakup shift more of the spill into surface slicks and mobile fragments. Earlier warming can release stored oil sooner, while reduced cover permits more wave mixing and evaporation. This does not guarantee rapid removal: a plume may still encounter [fast ice](../../../../../fast-ice.md) or deformed reservoirs, and oil-induced darkening promotes [ice-albedo feedback](../../../../../ice-albedo-feedback.md). These changes alter exposure, transport and recovery opportunities rather than making every warming effect favourable.

For the [oil lens capillary balance](../../../../../oil-lens-capillary-balance.md), distinguish the three interfacial tensions $\gamma_{io}$, $\gamma_{ow}$ and $\gamma_{iw}$, where the subscripts denote ice, oil and water. Replacing an ice–water area by an ice–oil and oil–water pair costs the effective interfacial energy

$$
\Gamma=\gamma_{io}+\gamma_{ow}-\gamma_{iw}.
$$

For a broad, shallow, non-wetting lens of volume $\mathcal V=Ah$, neglect the small edge region. The interfacial energy is $\Gamma A$. Because oil is lighter than water, moving it downward through a depth $h$ costs buoyancy potential energy $\frac12(\rho_w-\rho_o)gAh^2$. At fixed $\mathcal V$ their sum is

$$
E(h)=\mathcal V\left(\frac{\Gamma}{h}+\frac12(\rho_w-\rho_o)gh\right).
$$

Setting $E'(h)=0$ gives

$$
\boxed{h^2=\frac{2\Gamma}{(\rho_w-\rho_o)g}}.
$$

The second derivative is positive when $\Gamma>0$. Equivalently, if $\vartheta$ is the contact angle measured through the oil, the contact-line balance gives $\gamma_{iw}-\gamma_{io}=\gamma_{ow}\cos\vartheta$, so $\Gamma=\gamma_{ow}(1-\cos\vartheta)$. These are the interfacial quantities required, rather than $\gamma_{io}$ alone. If $\Gamma\leq0$, complete wetting replaces this finite-lens balance; if the ice is rough, pocket geometry replaces the flat-lens approximation. [oil–ice–water interfacial experiments](https://doi.org/10.1002/cjce.5450540110) give the corresponding contact-angle description.

The printed numerical premise is defective. A crude-oil density near $0.85\ \mathrm{g\,cm^{-3}}$ means $850\ \mathrm{kg\,m^{-3}}$, rather than the printed $0.85\ \mathrm{kg\,m^{-3}}$. Moreover, the specified oil–ice tension does not specify $\Gamma$. Even if $1.5\ \mathrm{N\,m^{-1}}$ were assumed to be $\Gamma$, taking $\rho_w=1025\ \mathrm{kg\,m^{-3}}$ would give $h=1.73\ \mathrm{cm}$ with the literal density and $h=4.18\ \mathrm{cm}$ with the plausible density repair. Neither calculation proves the claimed bound. With $\rho_o=850\ \mathrm{kg\,m^{-3}}$, the exact condition is

$$
\boxed{h<1\ \mathrm{cm}\quad\Longleftrightarrow\quad
0<\Gamma<0.08584\ \mathrm{N\,m^{-1}}}.
$$

For an explicitly defined, illustrative effective tension $\Gamma=0.050\ \mathrm{N\,m^{-1}}$, the same formula gives **$h=7.63\ \mathrm{mm}$**. This is a consistent sub-centimetre example, not a uniquely recoverable correction of the printed interfacial data.

For [ice-floe oil painting fraction](../../../../../ice-floe-oil-painting-fraction.md), let $Q$ be the oil volume arriving per day and assume complete retention in a layer of specified thickness $h$ on the passing underside. In time $\Delta t$, a plume of width $d$ sweeps a strip of area $dV\Delta t$, apart from the initial end correction. Coating that strip needs $hdV\Delta t$ of oil. The circular plume area cannot replace the swept width: $AVh$ has dimensions of volume times length per time. Therefore

$$
\boxed{V_c=\frac{Q}{dh},\qquad
p=\min\left(1,\frac{Q}{dVh}\right)}.
$$

Deposition becomes discontinuous when $V>V_c$. For $d=100\ \mathrm m$ and $V=10^4\ \mathrm{m\,day^{-1}}$, the four results are

$$
\begin{array}{c|c|c|c}
Q\ (\mathrm{m^3\,day^{-1}})&h\ (\mathrm m)&V_c\ (\mathrm{m\,day^{-1}})&100p\ (\%)\\ \hline
200&0.01&200&\boxed{2}\\
200&0.10&20&\boxed{0.2}\\
2000&0.01&2000&\boxed{20}\\
2000&0.10&200&\boxed{2}
\end{array}
$$

These percentages refer to the swept, $d$-wide corridor. The percentage of a whole floe of unspecified width is not determined. They are volume-equivalent coverage fractions at the stipulated local thickness; real deposition may instead give a thinner continuous smear, and losses reduce the retained fraction. Rough pockets store more oil per painted area, explaining their smaller coverage at fixed $Q$. The oil is exported as a patchy record of the floe's passage, so later melting can release many dispersed patches rather than a single stationary slick. Low areal coverage is compatible with substantial oil mass and locally thick contamination.

Preparedness should follow those transport stages. Before release, install well-control and subsea capping capability, winter-operable access, warmed pumping equipment, oil storage, under-ice survey capability and drifting position beacons; map currents, [sea ice](../../../../../sea-ice.md) motion and underside traps. Once a blowout starts, stopping or collecting oil near the source limits all later exposure. Survey the actual plume landfall with subsea vehicles and suitable acoustic or optical sensors, track both water and ice trajectories, and sample to distinguish an oil layer from ordinary ice roughness.

Under stable [fast ice](../../../../../fast-ice.md), targeted access holes and suction collectors can recover accessible reservoirs before encapsulation, provided the underside survey identifies their position and connectivity. Under moving [ice floes](../../../../../ice-floe.md), collectors must follow or intercept the contaminated floes; fixed surface booms cannot recover oil sealed beneath an intact slab. In broken ice and leads, use ice-capable skimmers and containment where relative ice and water motion allow it. Controlled burning is an option only for an accessible surface layer of sufficient thickness; dispersants concern exposed or subsea droplets with adequate mixing, not a sealed lens. During spring release, return to tracked pockets and floes, collect oil reaching leads and [melt ponds](../../../../../melt-pond.md), and prepare coastal interception along the forecast export route.

The research questions are specific: detection accuracy against natural underside roughness; droplet-size and plume-landfall prediction; capillary entry into saline pores; trapping capacities and remobilization thresholds of ridges; oil-dependent growth, viscosity and pumping rates at low temperature; timing of spring channel opening; and recovery, burning or dispersion efficiency and environmental effects under realistic ice and mixing conditions. A plan must quantify recoverable mass and operating windows rather than assume any one technique works in all ice states. [Arctic response-gap research](https://www.bsee.gov/research-record/osrr-1022-estimating-oil-spill-response-gap-us-arctic-ocean) explicitly treats weather, ice, access and technique limitations.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
