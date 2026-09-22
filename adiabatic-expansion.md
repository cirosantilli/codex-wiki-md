# Adiabatic expansion

↑ **Parent:** [Adiabatic process](adiabatic-process.md)

[Adiabatic expansion](adiabatic-expansion.md) increases the accessible [volume](volume-thermodynamics.md) without [heat transfer](heat-transfer.md). In a loaded piston expansion of the fixed-composition [ideal gas](ideal-gas.md) considered in [adiabatic process](adiabatic-process.md), positive outward [work](work.md) comes from [internal energy](internal-energy.md), so the final [temperature](temperature.md) decreases. This provides a cooling mechanism without removing [heat](heat.md) during the stroke. In the [Carnot cycle](carnot-cycle.md), reversible [adiabatic expansion](adiabatic-expansion.md) connects two different [temperatures](temperature.md) between its [isothermal processes](isothermal-process.md).[§4.3.1: adiabatic expansion between the isothermal legs](statistical-physics-by-david-tong/4-classical-thermodynamics.md)

For the same constant-$\gamma$ [reversible ideal-gas adiabat](reversible-ideal-gas-adiabat.md), put $b=V_2/V_1>1$. The scaling and [first law of thermodynamics](first-law-of-thermodynamics.md) give

$$
\frac{T_2}{T_1}=b^{1-\gamma},\qquad
\frac{p_2}{p_1}=b^{-\gamma},\qquad
W_{\rm out}=C_V(T_1-T_2)
=\frac{p_1V_1}{\gamma-1}\left(1-b^{1-\gamma}\right)>0.
$$

With the figure's stipulated $\gamma=1.4$, $p_1V_1=1\,\mathrm{kJ}$ and $b=2$, the final ratios are $T_2/T_1\simeq0.75786$ and $p_2/p_1\simeq0.37893$. Outward [work](work.md) is $0.60535\,\mathrm{kJ}$ and $\Delta U=-0.60535\,\mathrm{kJ}$. Reversing this particular path from its cooled endpoint would require the same [work](work.md) input; the figure's separate compression starts at the original state, so its input is different. Endpoint [entropy](entropy.md) supplies another independent check:

$$
\Delta S=C_V\ln\frac{T_2}{T_1}+nR\ln\frac{V_2}{V_1}=0.
$$

The two [logarithm](logarithm.md) terms cancel using $C_V(\gamma-1)=nR$, confirming the reversible path is an [isentropic process](isentropic-process.md). [MIT Unified Engineering, §5.4: ideal-gas endpoint entropy and constant-entropy scaling](https://web.mit.edu/16.unified/www/FALL/thermodynamics/notes/node40.html)

PASCO's expansion demonstration first compresses trapped air and waits for [thermal equilibrium](thermal-equilibrium.md) before the rapid expansion. Its manual warns that [friction](friction.md)-warmed cylinder regions contact the [gas](gas.md) during expansion, compromising quantitative comparison. [PASCO scientific, guide 012-05110D, p. 3: expansion preparation and frictional wall-heating limitation](https://cdn.pasco.com/product_document/Adiabatic-Gas-Law-Apparatus-TD-8565-Manual.pdf) The hold separates cooling caused by expansion from simply undoing the earlier hot compression. As proposed controls, observe the [temperature](temperature.md) dip and subsequent warming, compare rapid and slow strokes from matched initial states, and assess wall [heat transfer](heat-transfer.md) and probe lag before fitting a reversible model.

Cooling is not a universal consequence of [adiabatic expansion](adiabatic-expansion.md): [free expansion](free-expansion.md) of an [ideal gas](ideal-gas.md) has no outward [work](work.md) and returns to the same equilibrium [temperature](temperature.md). Its [entropy](entropy.md) increases, so the reversible power laws do not describe it. Reuse [free expansion](free-expansion.md), [Joule's free-expansion experiment](joule-s-free-expansion-experiment.md) and [temperature sensitivity of a free-expansion experiment](temperature-sensitivity-of-a-free-expansion-experiment.md) for that apparatus, its [energy](energy.md) budget and the real-gas qualifications. The useful distinction is the load: expansion cools this [ideal gas](ideal-gas.md) when it must spend [internal energy](internal-energy.md) doing [work](work.md).

## ↑ Ancestors (7)

1. [Adiabatic process](adiabatic-process.md)
2. [First law of thermodynamics](first-law-of-thermodynamics.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Adiabatic compression](adiabatic-compression.md)
- [Adiabatic expansion](adiabatic-expansion.md)
- [Adiabatic process](adiabatic-process.md)
- [Carnot cycle](carnot-cycle.md)
- [Free expansion](free-expansion.md)
- [Ideal gas](ideal-gas.md)
- [Internal energy of an ideal gas](internal-energy-of-an-ideal-gas.md)
- [Isothermal compressibility](isothermal-compressibility.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/10d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/15d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/10d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/34d/a/solution.md)
