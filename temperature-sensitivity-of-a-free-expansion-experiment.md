# Temperature sensitivity of a free-expansion experiment

↑ **Parent:** [Joule's free-expansion experiment](joule-s-free-expansion-experiment.md)

The [gas](gas.md)-only condition $\Delta U=0$ requires negligible [heat](heat-split.md) exchange with the apparatus. If the insulated [isolated system](isolated-system.md) instead includes the walls, sensors and water, the [first law of thermodynamics](first-law-of-thermodynamics-split.md) fixes their combined [energy](energy-split.md). Once everything returns to a common final [temperature](temperature-split.md), a constant apparatus [heat capacity](heat-capacity.md) $C_a$ gives

$$
U_g(T_2,V_2)-U_g(T_1,V_1)+C_a(T_2-T_1)=0.
$$

Define $A=U_g(T_1,V_2)-U_g(T_1,V_1)$, the gas's [internal energy](internal-energy-split.md) increase for the same expansion evaluated at the initial [temperature](temperature-split.md). For a small [temperature](temperature-split.md) change, linearizing at the final [volume](volume-thermodynamics.md) gives

$$
\Delta T\simeq-\frac{A}{C_{V,g}+C_a}.
$$

Here $C_{V,g}$ is the whole gas sample's [heat capacity at constant volume](heat-capacity-at-constant-volume.md) at the reference state. Compared with an isolated gas sample's $-A/C_{V,g}$, the common final signal is reduced by $C_{V,g}/(C_{V,g}+C_a)$. This [energy](energy-split.md) accounting explains why a massive bath can conceal a real-gas effect. Fitzpatrick gives the corresponding apparatus correction for the [Van der Waals equation](van-der-waals-equation.md). [Van der Waals Gas](thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/van-der-waals-gas.md)

For a toy calculation, stipulate $A=5\,\mathrm J$, $C_{V,g}=10\,\mathrm{J\,K^{-1}}$ and $C_a=990\,\mathrm{J\,K^{-1}}$, all constant in this example. The predicted cooling magnitude changes from $0.5\,\mathrm K$ for the gas alone to $0.005\,\mathrm K$ for the combined apparatus. An illustrative effective detection threshold of $0.01\,\mathrm K$ would miss the latter. These are chosen numbers, not Joule's measurements. In this approximation a null observation only bounds $|A|\lesssim(C_{V,g}+C_a)\epsilon_T$, where $\epsilon_T$ is the detectable [temperature](temperature-split.md) change after allowing for drift and other experimental uncertainties; a display's smallest digit is not automatically this threshold.

The historical limitation was recognized explicitly: Joule and Thomson later estimated that the common apparatus in Joule's experiment would cool by only about $0.003\,\mathrm K$, explaining why the earlier external thermal effect was undetectable. This was a later calculation about the apparatus, not a measured cooling trace. [Joule and Thomson, On the Thermal Effects of Elastic Fluids, Part II, reprint p. 63: estimated temperature change of the copper-and-water apparatus](https://upload.wikimedia.org/wikipedia/commons/4/47/The_free_expansion_of_gases-_memoirs_by_Gay-Lussac%2C_Joule%2C_and_Joule_and_Thomson%3B_%28IA_cu31924012329300%29.pdf#page=75)

## ↑ Ancestors (7)

1. [Joule's free-expansion experiment](joule-s-free-expansion-experiment.md)
2. [Free expansion](free-expansion.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Adiabatic expansion](adiabatic-expansion.md)
- [Free expansion](free-expansion.md)
- [Internal energy of an ideal gas](internal-energy-of-an-ideal-gas.md)
