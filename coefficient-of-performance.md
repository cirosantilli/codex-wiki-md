# Coefficient of performance

↑ **Parent:** [Heat pump](heat-pump.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coefficient_of_performance)

For the cyclic two-side [energy](energy.md) balance in [refrigerator](refrigerator.md), define the dimensionless cooling and heating coefficients by

$$
\mathrm{COP}_{\rm r}=\frac{Q_c}{W},\qquad
\mathrm{COP}_{\rm heat}=\frac{Q_h}{W}
=\frac{Q_c+W}{W}=\mathrm{COP}_{\rm r}+1.
$$

This identity applies even to irreversible machines, provided both coefficients refer to the same operating point, [work](work.md) input and boundary with no additional [energy](energy.md) transfer or storage. It does not compare two separately operated appliances. Unlike [thermal efficiency](thermal-efficiency.md) of a [heat engine](heat-engine.md), a [COP](coefficient-of-performance.md) can exceed one: its numerator counts [heat](heat.md) moved, including [energy](energy.md) taken from another region. [University of Tennessee, Refrigerators, air conditioners, and heat pumps: the two performance ratios](https://labs.phys.utk.edu/mbreinig/phys136core/modules/m3/refrigerators.html)

To obtain temperature-only bounds, impose stronger assumptions: a cyclic machine exchanges [heat](heat.md) only with two ideal [thermal reservoirs](heat-bath.md) maintained at uniform, fixed absolute [thermodynamic temperatures](thermodynamic-temperature.md) $0<T_c<T_h$, and receives [work](work.md) through an ideal input carrying no [entropy](entropy.md). Include the machine and the [heat transfer](heat-transfer.md) interfaces in the [entropy production](entropy-production.md) accounting. Because its own [entropy](entropy.md) returns to its initial value each cycle, the [Second law of thermodynamics](second-law-of-thermodynamics.md) gives

$$
S_{\rm gen}=\frac{Q_h}{T_h}-\frac{Q_c}{T_c}\geq0.
$$

Combining this inequality with $Q_h=Q_c+W$ gives

$$
\boxed{\mathrm{COP}_{\rm r}\leq\frac{T_c}{T_h-T_c}},\qquad
\boxed{\mathrm{COP}_{\rm heat}\leq\frac{T_h}{T_h-T_c}}.
$$

Equality requires a [reversible thermodynamic process](reversible-thermodynamic-process.md) for the entire cycle and its contacts, as in a reversed [Carnot cycle](carnot-cycle.md). These are [Carnot's theorem](carnot-s-theorem.md) bounds independent of the working substance. Use [kelvin](kelvin.md) values, not [degree Celsius](degree-celsius.md) readings, in the numerators; the [temperature](temperature.md) difference can be expressed in either unit. [MIT, Refrigerators and heat pumps: reversed Carnot cycle and absolute-temperature cooling bound](https://web.mit.edu/16.unified/www/FALL/thermodynamics/notes/node25.html) [Ling, Moebs and Sanny, University Physics Volume 2, §4.5: reversible reservoir entropy balance](https://openstax.org/books/university-physics-volume-2/pages/4-5-the-carnot-cycle)

The diagram fixes $T_c=280\,\mathrm K$ and sets $T_h=320\,\mathrm K$, so the reversible bounds are $280/40=7$ and $320/40=8$. The stipulated machine with $\mathrm{COP}_{\rm r}=3$ and $\mathrm{COP}_{\rm heat}=4$ satisfies both. Its reservoir [entropy production](entropy-production.md) per cycle is $4000/320-3000/280=25/14\,\mathrm{J\,K^{-1}}>0$. Increasing the [temperature](temperature.md) lift $\Delta T=T_h-T_c$ at fixed $T_c$ lowers both bounds. Equivalently, delivering fixed $Q_h$ needs at least

$$
W_{\min}=Q_h\left(1-\frac{T_c}{T_h}\right).
$$

These expressions reveal why a small [temperature](temperature.md) lift is attractive. Their divergence as $T_h-T_c\to0^+$ is an ideal reversible limit, not a promise of infinite heating or cooling [power](power.md). For finite [heat transfer](heat-transfer.md) rates, the working [fluid](fluid.md) must be colder than the cold bath and hotter than the hot bath; these contact differences produce [entropy](entropy.md) and increase the internal [temperature](temperature.md) lift. Dissipative compression and the pressure-reducing restriction of [vapor-compression refrigeration](vapor-compression-refrigeration.md) supply further departures from reversibility. Thus bath [temperatures](temperature.md) set an outer bound, not a prediction of real [COP](coefficient-of-performance.md). [MIT, Refrigerator hardware: working-fluid temperatures on either side of the baths](https://web.mit.edu/16.unified/www/FALL/thermodynamics/notes/node25.html)

## ↑ Ancestors (6)

1. [Heat pump](heat-pump.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Heat engine](heat-engine.md)
- [Heat pump](heat-pump.md)
- [Refrigerator](refrigerator.md)
