<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $h_i,h_s$ denote ice and snow thickness, let $z$ increase downwards, and count external atmospheric fluxes as positive into the surface. The [Maykut-Untersteiner model](../../../../../maykut-untersteiner-model.md) is a time-dependent column model, rather than a single thickness formula: [heat conduction](../../../../../thermal-conduction.md), heat storage, internal absorption of sunlight and moving freezing/melting boundaries must be solved together. In an ice-following description its energy equation can be written

$$
\rho_i\frac{D e_i(T,S)}{Dt}=\partial_z\big(k_i(T,S)\partial_zT\big)-\partial_z I(z,t),\qquad \rho_s c_s\frac{DT_s}{Dt}=\partial_z\big(k_s\partial_zT_s\big),
$$

where $e_i$ is specific [enthalpy](../../../../../enthalpy.md), $S$ is the prescribed ice [salinity](../../../../../salinity.md), and $I$ is the downward penetrating shortwave flux. The material derivative includes coordinate motion if a moving numerical grid is used. A common attenuation form is $I=I_0e^{-\kappa z}$ within a homogeneous ice layer, with the origin taken at that layer's top. The corresponding source is $\kappa I$. Snow-covered cases have much less penetration; absorbed surface radiation must not also be counted as internal heating.

The liquid brine fraction contributes [latent heat](../../../../../latent-heat.md) to the effective [specific heat capacity](../../../../../specific-heat-capacity.md): for the illustrative liquidus approximation $\phi_b\simeq-\mu S/T$ with Celsius $T<0$ in the mixed-phase range $0<\phi_b<1$, $c_{\rm eff}=\partial_Te_i\simeq c_0+L_f\mu S/T^2$. The precise ice conductivity and heat capacity are [salinity](../../../../../salinity.md)- and temperature-dependent. This is why the full transient temperature profile need not be linear. At the snow-ice interface impose continuity of temperature and conductive [heat flux](../../../../../heat-flux-density.md); at the ice bottom impose the seawater freezing temperature $T_f$.

Write $I_0=i_0(1-\alpha)F_{\rm SW}$ and define the atmospheric input absorbed at the surface by

$$
Q_A=(1-i_0)(1-\alpha)F_{\rm SW}+F_{{\rm LW},\downarrow}-\varepsilon\sigma T_{\rm surf,K}^4+F_H+F_E.
$$

Here $\alpha$ is the surface [albedo](../../../../../albedo.md), $\sigma$ is the [Stefan-Boltzmann constant](../../../../../stefan-boltzmann-constant.md), and $F_H,F_E$ are signed sensible and latent turbulent [heat fluxes](../../../../../heat-flux-density.md). With upward conductive flux $q_c=k\partial_zT$, the cold, nonmelting surface satisfies $Q_A+q_{c,s}=0$. Once the surface reaches its melting temperature, constrain it there and use excess energy for ablation:

$$
L_s\dot m_s=Q_A+q_{c,s}\ge0.
$$

The mass-loss rate $\dot m_s$ first removes [snow](../../../../../snow.md) at thickness rate $\dot m_s/\rho_s$; after the snow is gone it removes ice at rate $m_i=\dot m_s/\rho_i$. [Snow](../../../../../snow.md) thickness also changes through prescribed snowfall and any separately represented compaction or sublimation.

At the bottom, the [Stefan condition](../../../../../stefan-condition.md) equates latent heat released by growth to upward conductive removal minus upward [ocean heat flux](../../../../../ocean-heat-flux.md) $F_o$:

$$
\boxed{\rho_iL_b g_b=q_{c,b}-F_o,\qquad \dot h_i=g_b-m_i.}
$$

Here $g_b$ is positive for basal freezing and negative for basal melting, and $L_b$ is the appropriate effective latent heat. These equations, the incident fluxes and snowfall determine the seasonal thickness trajectory. [Annual sea-ice thermodynamic equilibrium](../../../../../annual-sea-ice-thermodynamic-equilibrium.md) means a periodic temperature field and $h_i(t+\mathcal T)=h_i(t)$, so

$$
\boxed{\int_0^{\mathcal T}(g_b-m_i)\,dt=0.}
$$

With constant $L_b$, this is equivalently $\int(q_{c,b}-F_o-\rho_iL_bm_i)\,dt=0$. An “equilibrium thickness” must refer to the mean or a specified phase of this seasonal cycle.

A useful winter reduction neglects heat storage and solar penetration and treats each conductivity as constant. The two layers act as thermal resistances in series:

$$
\boxed{q_c\simeq\frac{T_f-T_{\rm surf}}{h_i/k_i+h_s/k_s},\qquad \rho_iL_b\dot h_i\simeq\frac{T_f-T_{\rm surf}}{h_i/k_i+h_s/k_s}-F_o.}
$$

This displays the dependence on snow and ice thickness, but is not a replacement for the full seasonally forced [Maykut-Untersteiner model](../../../../../maykut-untersteiner-model.md).

Increasing [ocean heat flux](../../../../../ocean-heat-flux.md) subtracts directly from basal growth and increases bottom ablation. On a stable perennial branch it lowers annual equilibrium thickness, and sufficiently large input can eliminate a year-round ice cover. With zero oceanic input, removing this heat sink can allow much thicker thermodynamic ice; it does not remove the seasonal surface energy balance.

Additional annual snowfall has competing effects. Larger $h_s/k_s$ suppresses winter [heat conduction](../../../../../thermal-conduction.md) and basal growth, favoring thinner ice. But persistent bright [snow](../../../../../snow.md) raises [albedo](../../../../../albedo.md), consumes energy when it melts and delays exposure of dark bare ice, suppressing summer ice ablation. The original column calculations show near compensation for moderate snowfall and substantial thickening when much more snow survives into summer. Thus **annual equilibrium thickness need not decrease with snowfall**, even though greater snow thickness at fixed winter temperatures always reduces the conductive growth rate. The balance also depends on snowfall timing and the treatment of snow-to-ice conversion. These seasonal responses are illustrated by [the original model calculations](https://frouingroup.ucsd.edu/Most_recent_figs/Refs/Maykut-Unitersteiner_1971.pdf).

Reducing [surface albedo](../../../../../surface-albedo.md) increases absorbed shortwave radiation. It promotes surface ablation, internal heating and, where sunlight reaches the ocean, basal ablation; the [ice-albedo feedback](../../../../../ice-albedo-feedback.md) reinforces the reduction in equilibrium ice thickness. Increasing [albedo](../../../../../albedo.md) has the opposite effect. This sensitivity is strongest when sunlight is available and dark surfaces are exposed, rather than during polar night.

For the observed bottom melt, use $\rho_i\simeq917\ \mathrm{kg\,m^{-3}}$, $L_f\simeq3.34\times10^5\ \mathrm{J\,kg^{-1}}$ and approximately 122 days. The [basal melt heat flux](../../../../../basal-melt-heat-flux.md) equivalent is

$$
\boxed{\overline F_{\rm melt}=\frac{\rho_iL_f\Delta h}{\Delta t}\simeq\frac{917(3.34\times10^5)(2)}{122(86400)}\simeq58\ \mathrm{W\,m^{-2}}\approx60\ \mathrm{W\,m^{-2}}.}
$$

The integrated latent heat is about $6.1\times10^8\ \mathrm{J\,m^{-2}}$. This is energy used for melting, not automatically the complete ocean-to-ice heat input: the basal balance gives $F_o=\rho_iL_b(-g_b)+q_{c,b}$, with sensible heat and salinity corrections if needed.

A likely major source is solar heating of an unusually large open-water fraction. Dark water absorbs much more sunlight than snow-covered ice, and warm water transfers that stored heat to floe bottoms by mixing and lateral transport. Thin or ponded ice also transmits more sunlight. Wind-driven divergence and export expose additional water, while advection of warm Pacific or Atlantic water and mixing of subsurface heat can contribute regionally. The supplied melt amount alone cannot partition these sources. [The 2007 Beaufort Sea heat-budget analysis](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2008GL034007) found that locally absorbed solar heat was sufficient to account for the enhanced basal melt. **The latent-heat equivalent is about $60\ \mathrm{W\,m^{-2}}$; increased solar absorption by exposed ocean is a well-supported principal explanation.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 89](../../paper-89-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
