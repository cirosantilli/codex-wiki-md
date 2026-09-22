<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [convective chimney](../../../../../convective-chimney.md) is a localized, deeply mixed region within a stratified ocean, formed when surface [buoyancy](../../../../../buoyancy.md) loss allows convection to penetrate far below the surrounding mixed layer. The chimney describes the mixed water column and its circulation; instantaneous downward transfer occurs through many smaller plumes, accompanied by compensating motion and lateral exchange, rather than through one permanently uniform downward pipe. [Open-ocean convection](../../../../../open-ocean-convection.md) occurs in the Labrador and Irminger Seas, the Greenland Sea, the northwestern Mediterranean, and episodically in the open Weddell Sea under a large polynya. Dense-water formation on a continental shelf is related but geometrically distinct from deep open-ocean chimney convection.

Observed Greenland Sea [convective chimneys](../../../../../convective-chimney.md) include compact, approximately circular, weakly stratified cores with temperature and salinity much more uniform vertically than in the ambient ocean. A mapped example was about $20\ \mathrm{km}$ across, extended to about $2500\ \mathrm m$ in winter, and rotated anticyclonically. In summer a fresh, low-density cap and shallower lateral intrusions could isolate the deep core, while winter [buoyancy](../../../../../buoyancy.md) loss removed the cap and renewed deep contact. Such cores could persist through several seasons, so presence of a deep homogeneous core is not proof that vigorous convection is occurring continuously. These particular dimensions and seasonal structure come from [successive hydrographic surveys of Greenland Sea chimneys](https://doi.org/10.1029/2003GL019017).

Formation is favoured by the cyclonic Greenland gyre, which domes density surfaces and can reduce the depth of the stratified barrier. Cold, dry wind outbreaks produce strong sensible, latent and longwave heat loss. Where [frazil ice](../../../../../frazil-ice.md) and pancake ice form in the Odden ice tongue, ice growth removes relatively fresh material while [brine rejection](../../../../../brine-rejection.md) increases the density of the remaining water. Ice advection can keep exposing water for further freezing and separate local brine release from later freshwater return. This combination of preconditioning, cooling and sustained salt input can make a formerly buoyant surface layer dense enough to convect.

Conversely, a fresh surface cap supplied by Arctic freshwater and ice melt strengthens [density stratification](../../../../../density-stratification.md). Warmer atmospheric outbreaks reduce surface heat loss and ice production; circulation changes affecting the cold northwesterly winds and the Odden can reduce the brine source. Atlantic advection supplies both heat and salt, with competing effects on density, so temperature alone is not an adequate diagnostic. The historical decline in Odden ice formation and changes in wind regimes offer a mechanism for less favourable chimney production around the period considered, but ice-driven formation is a physical hypothesis, not evidence that every observed chimney requires ice or that every local change follows a single climate index. The [Greenland Sea salt-flux model](https://doi.org/10.1029/2001JC001099) explicitly includes ice production and advection.

For the [brine rejection](../../../../../brine-rejection.md) mechanism, let $\dot h_i>0$ be ice growth and let $s_w,s_i$ be water and ice salt mass fractions. Newly formed ice removes mass $\rho_i\dot h_i$ per area per time. Compared with removing water at concentration $s_w$, it leaves an excess salt flux in the liquid of

$$
\boxed{F_{\mathrm{salt}}=\rho_i\dot h_i(s_w-s_i)}.
$$

The units are $\mathrm{kg\,m^{-2}\,s^{-1}}$. With the exam's approximation $s=10^{-3}S$ for salinity $S$ in psu, the corresponding mixed-layer salinity tendency is, to first order,

$$
\frac{dS_w}{dt}\simeq\frac{\rho_i}{\rho_wH}\dot h_i(S_w-S_i).
$$

If $\beta_S=(1/\rho_w)(\partial\rho/\partial S)>0$, the surface buoyancy input is negative, with scale $-g\beta_S(\rho_i/\rho_w)\dot h_i(S_w-S_i)$. The enhanced density produces downward saline plumes that deepen mixing if this [buoyancy](../../../../../buoyancy.md) loss overcomes the available [density stratification](../../../../../density-stratification.md). This explains why exporting new ice while retaining its rejected salt can strengthen overturning, whereas later local melt reverses the freshwater effect.

For the numerical comparison, the cover gives the [specific heat capacity](../../../../../specific-heat-capacity.md) of ice, not of seawater. A seawater value must therefore be supplied explicitly. Take $c_{p,w}=4000\ \mathrm{J\,kg^{-1}\,K^{-1}}$ and use the stipulated $\rho_w=1025\ \mathrm{kg\,m^{-3}}$. A $100\ \mathrm m$ column has initial water mass per area

$$
M_0=\rho_wH=102500\ \mathrm{kg\,m^{-2}}.
$$

Cooling it by $1.8\ \mathrm K$ removes

$$
\boxed{Q=M_0c_{p,w}(1.8)=7.38\times10^8\ \mathrm{J\,m^{-2}}}.
$$

The specified thermal density relation gives

$$
\boxed{\Delta\rho_{\mathrm{cool}}=\frac{1.8}{10}=0.18\ \mathrm{kg\,m^{-3}}}.
$$

This assumes the whole column mixes and neglects entrainment and advected heat. Using the supplied ice heat capacity $2100$ for liquid seawater would change $Q$ incorrectly.

At the freezing point the same heat extraction produces a pure-ice mass per area

$$
m_i=\frac{Q}{L_f}=2196.43\ \mathrm{kg\,m^{-2}},\qquad
\boxed{f_i=\frac{m_i}{M_0}=\frac{c_{p,w}(1.8)}{L_f}=0.0214286}.
$$

Here $f_i$ is the fraction of the original water mass removed into ice. With the explicit ice-density approximation $\rho_i=900\ \mathrm{kg\,m^{-3}}$, the resulting ice thickness is

$$
\boxed{h_i=\frac{m_i}{\rho_i}=2.440\ \mathrm m}.
$$

The [water-equivalent thickness](../../../../../water-equivalent-thickness.md) uses a reference water density: with fresh water at $1000\ \mathrm{kg\,m^{-3}}$, it is $m_i/1000=\boxed{2.196\ \mathrm m\simeq2.2\ \mathrm m}$. The depth of the original seawater removed is instead $m_i/1025=\boxed{2.143\ \mathrm m}$. These three quantities are different; $2.2\ \mathrm m$ is not the physical ice thickness for the stated density approximation.

Let the initial salinity be $S_0$. Complete exclusion of salt from the ice leaves all the initial salt in a liquid mass $M_1=M_0-m_i$. [Conservation of salt during freezing](../../../../../conservation-of-salt-during-freezing.md) gives

$$
S_1M_1=S_0M_0,qquad
\boxed{S_1=\frac{S_0}{1-f_i},\qquad
\Delta S=\frac{S_0f_i}{1-f_i}}.
$$

The initial salinity is not printed, so a unique numerical salinity increase requires another explicit assumption. For $S_0=35\ \mathrm{psu}$,

$$
\Delta S=\frac{35(0.0214286)}{0.9785714}=0.7664\ \mathrm{psu},
\qquad \boxed{\Delta\rho_{\mathrm{freeze}}=0.7664\ \mathrm{kg\,m^{-3}}}.
$$

The total density increase after cooling followed by freezing is then about $0.9464\ \mathrm{kg\,m^{-3}}$. The factor $1/(1-f_i)$ is required because salt concentration refers to the remaining liquid mass. Using ice thickness divided by the original water depth as the removed mass fraction would violate this accounting.

For this assumed salinity, the [freezing-to-cooling density efficiency](../../../../../freezing-to-cooling-density-efficiency.md) shows that equal heat extraction at freezing produces about $0.7664/0.18=\boxed{4.26}$ times the density increase of the initial cooling. At low temperature the thermal expansion response is weak, whereas [brine rejection](../../../../../brine-rejection.md) changes salinity efficiently. This supports strong freezing-driven convection where water is already near its freezing point. It does not mean freezing always creates deep chimneys: the initial [density stratification](../../../../../density-stratification.md), freshwater supply, mixing depth and later melting remain decisive. The freezing point itself decreases as salinity rises; keeping it at $-1.8^\circ\mathrm C$ is the exam's approximation. Allowing that small additional cooling and a temperature-dependent equation of state would require a refined heat budget.

Important other sites of freezing-enhanced downward transfer include the Ross and Weddell Antarctic shelves and their coastal polynyas, Adélie Land and Cape Darnley, Arctic shelves such as the Barents and Kara Seas, and the Sea of Okhotsk. On shelves the saline dense water can cascade down a continental slope and feed deeper waters; the same salt-removal balance operates without requiring an isolated open-ocean chimney. A later direct observational example is [bottom-water formation associated with Cape Darnley sea-ice production](https://doi.org/10.1038/ngeo1738).

Atmospheric warming of the Greenland Sea can reduce surface cooling and ice formation, while increased freshwater input can inhibit convection. If these changes weaken the [Atlantic meridional overturning circulation](../../../../../atlantic-meridional-overturning-circulation.md) and its northward heat transport, their ocean-mediated tendency is **relative cooling, or reduced warming, of northwestern Europe compared with otherwise identical atmospheric warming**. This is not a prediction of net European cooling under all emissions scenarios, nor does one chimney determine the whole overturning circulation: other convection regions, winds, freshwater pathways and coupled ocean adjustment also matter. The physical conclusion is the sign of the heat-transport response, not a specified century-scale temperature decrement.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
