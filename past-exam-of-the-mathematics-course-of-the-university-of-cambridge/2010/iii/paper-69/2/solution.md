<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [steric sea level change](../../../../../steric-sea-level-change.md) is caused by a change of water volume at fixed ocean mass. Warming usually lowers seawater [mass density](../../../../../density.md), producing [thermosteric sea level change](../../../../../thermosteric-sea-level-change.md); freshening also lowers density and produces a halosteric contribution. Both depend on the temperature, pressure and [salinity](../../../../../salinity.md) dependence of the equation of state. Regional freshening or warming can therefore change local sea level even when the global ocean mass has not increased.

An [eustatic sea level change](../../../../../eustatic-sea-level-change.md) concerns the ocean water amount or basin capacity. On the coming-century timescale, the principal positive mass contributions are melting mountain [glaciers](../../../../../glacier.md) and [ice caps](../../../../../ice-cap.md), and loss of grounded ice from Greenland and Antarctica, including iceberg discharge. Terrestrial water storage also matters: groundwater depletion transfers water to the ocean, whereas reservoir filling retains it on land. Snowfall accumulation can partly compensate ice loss. Basin changes associated with geology matter over longer periods, and vertical land motion changes locally measured relative sea level. Melting floating [sea ice](../../../../../sea-ice.md) has already largely displaced its eventual meltwater volume; its direct contribution is small compared with transfer of grounded ice into the ocean. Small density and salinity corrections do not alter that distinction.

For scale, a contemporary budget available in 2010 gave the following approximate contributions for 1993–2003, in $\mathrm{mm\,yr^{-1}}$:

$$
\begin{array}{c|r}
\text{Thermal expansion}&1.6\\
\text{Glaciers and ice caps}&0.77\\
\text{Greenland ice sheet}&0.21\\
\text{Antarctic ice sheet}&0.21\\\hline
\text{Sum of these estimates}&2.8\\
\text{Observed global mean rise}&3.1
\end{array}
$$

These are period-specific estimates with appreciable uncertainties, particularly for Antarctica, rather than exact closure of the budget. For comparison, over 1961–2003 the observed rate was about $1.8\,\mathrm{mm\,yr^{-1}}$ and the estimated [thermal expansion](../../../../../thermal-expansion.md) contribution about $0.4\,\mathrm{mm\,yr^{-1}}$. The shorter interval need not define a permanent acceleration by itself, but the magnitudes show that thermal expansion and land-ice loss are both essential.

With continued warming, increasing [ocean heat content](../../../../../ocean-heat-content.md) sustains [thermosteric sea level change](../../../../../thermosteric-sea-level-change.md), including after surface warming slows because the deep ocean equilibrates gradually. Increased [ice ablation](../../../../../ice-ablation.md) generally increases glacier runoff, although small glaciers eventually lose much of their available ice. Surface melt and changes in outlet-glacier flow can increase the ice-sheet contribution; ocean-driven loss of [ice shelves](../../../../../ice-shelf.md) can accelerate discharge of grounded ice. Greater snowfall provides some compensation but cannot be assumed to cancel these losses. Thus, under continued substantial [greenhouse gas](../../../../../greenhouse-gas.md) emissions, **the global rate is likely to rise above its historical few millimetres per year**, with an increasing contribution from the great ice sheets. The precise century-scale increase depends on emissions, ocean heat uptake and [ice sheet dynamics](../../../../../ice-sheet-dynamics.md); a single fixed rate extrapolated from one decade is inadequate.

For the idealized mixed-layer calculation, the stated density response gives

$$
\frac{\partial\rho}{\partial T}=-\frac{1}{5}\,\mathrm{kg\,m^{-3}\,K^{-1}},\qquad \alpha=-\frac1\rho\frac{\partial\rho}{\partial T}=\frac{0.2}{1025}=1.95\times10^{-4}\,\mathrm{K^{-1}}.
$$

At fixed column mass, $\rho H=(\rho+\Delta\rho)(H+\Delta\eta)$, so to first order

$$
\Delta\eta=-\frac{H\Delta\rho}{\rho}=H\alpha\Delta T=200\times1.95\times10^{-4}\times1,\qquad \boxed{\Delta\eta\simeq0.039\,\mathrm m=3.9\,\mathrm{cm}}.
$$

This is only the [thermosteric sea level change](../../../../../thermosteric-sea-level-change.md) from the prescribed layer and warming. The much larger total observed rise since the nineteenth century does not, by itself, prove deeper warming: part of that rise is [eustatic sea level change](../../../../../eustatic-sea-level-change.md). After independently allowing for the mass contribution, a larger remaining steric signal would require warming below $200\,\mathrm m$, a different temperature distribution, or corrections to the simplified equation of state. Direct temperature profiles do independently establish subsurface ocean warming. It reaches depth through winter mixing and [open-ocean convection](../../../../../open-ocean-convection.md), especially in the North Atlantic and parts of the Southern Ocean; through subduction of surface waters into the interior; and through advection and turbulent mixing. Formation and spreading of intermediate and deep waters transmit surface properties far beyond the immediate region of heat uptake. Warm surface water need not simply sink locally: cooling, freshwater effects and [density stratification](../../../../../density-stratification.md) govern the actual pathways.

Using $R=6.371\times10^6\,\mathrm m$, the ocean area is $A_o=0.70(4\pi R^2)=3.57\times10^{14}\,\mathrm{m^2}$. A liquid runoff volume $\Delta V=600\,\mathrm{km^3}=6.00\times10^{11}\,\mathrm{m^3}$ gives

$$
\boxed{\dot\eta_{\rm runoff}=\frac{\Delta V}{A_o}=1.68\times10^{-3}\,\mathrm{m\,yr^{-1}}\simeq1.7\,\mathrm{mm\,yr^{-1}}}.
$$

This is the contribution from that input, before allowing for other exchanges in the [global ocean freshwater budget](../../../../../global-ocean-freshwater-budget.md).

For the sea-ice dilution estimate, the ocean volume is $V_o=A_o(4000\,\mathrm m)=1.428\times10^{18}\,\mathrm{m^3}$. Let its initial mean [salinity](../../../../../salinity.md) be $S_0$; the question does not specify it, so use $S_0\simeq35$ psu for a numerical estimate. Interpret the $600\,\mathrm{km^3}$ as liquid freshwater-equivalent melt, with $\rho_f\simeq1000\,\mathrm{kg\,m^{-3}}$. Salt mass remains fixed while liquid water mass increases, giving

$$
S_1=\frac{S_0\rho_wV_o}{\rho_wV_o+\rho_f\Delta V},\qquad \Delta S\simeq-S_0\frac{\rho_f\Delta V}{\rho_wV_o}.
$$

Consequently

$$
\boxed{\dot S\simeq-1.43\times10^{-5}\,\mathrm{psu\,yr^{-1}}\approx-1.5\times10^{-5}\,\mathrm{psu\,yr^{-1}}}.
$$

Approximating the densities as equal gives $-1.47\times10^{-5}$ psu per year. If the quoted volume instead denotes literal solid-ice volume, use $\rho_i\Delta V$ for the added mass; with $\rho_i=917\,\mathrm{kg\,m^{-3}}$ the result is $-1.32\times10^{-5}$ psu per year. Either convention gives the same order of magnitude. Floating-ice melt can change mean ocean [salinity](../../../../../salinity.md) even though its direct sea-level effect is small: displaced volume and dissolved salt concentration are different budgets.

An observed net freshening is a statement about the sum of all freshwater exchanges, not a separate measurement of every positive contribution. Let $M$ be liquid ocean mass, $R$ net freshwater runoff from land, $I$ net global sea-ice melt minus formation, and $P-E$ net precipitation minus evaporation, all expressed as masses per unit time. The [global ocean freshwater budget](../../../../../global-ocean-freshwater-budget.md) and salt conservation give

$$
\dot M=R+I+P-E,\qquad \frac{\dot S}{S}=-\frac{R+I+P-E}{M}.
$$

The runoff term must include non-ice river input as well, or those other exchanges must already have been netted out. If the measured freshening equals that predicted from $I$ alone, positive runoff is still possible provided

$$
\boxed{R+P-E=0}
$$

or an equivalent compensating term exists in the complete budget. For instance, excess evaporation can remove water at the same rate at which land-ice runoff supplies it; compensating net ice formation elsewhere must also be included if $I$ was initially only the Arctic contribution. Gross seasonal melt cannot be compared with an annual global trend without subtracting refreezing. Such compensation also means that the runoff-only sea-level increment need not equal the total retained increment. If runoff is additional, sea-ice melt is already net and global, and every other freshwater term is zero, the two contributions must add: under those stronger assumptions the alleged equality would be inconsistent. **The apparent paradox is resolved by closing the complete freshwater and salt budgets.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
