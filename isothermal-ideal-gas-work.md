# Isothermal ideal-gas work

↑ **Parent:** [Isothermal process](isothermal-process.md)

For a [reversible thermodynamic process](reversible-thermodynamic-process.md) that changes the [volume](volume-thermodynamics.md) of a fixed amount of [ideal gas](ideal-gas-split.md) at absolute [temperature](temperature-split.md) $T$, the [work](work.md) done by the [gas](gas.md) is

$$
W_{\rm by,rev}=\int_{V_i}^{V_f}p\,dV
=nRT\int_{V_i}^{V_f}\frac{dV}{V}
=nRT\ln\frac{V_f}{V_i}
=nRT\ln\frac{p_i}{p_f}.
$$

Here $n$ is the [amount of substance](amount-of-substance.md), $R$ the [molar gas constant](molar-gas-constant.md), $p$ the [pressure](pressure-split.md), and $\ln$ the [natural logarithm](natural-logarithm.md). The [ideal gas law](ideal-gas-law.md) supplies $p=nRT/V$; the [integral](integral-split.md) is the signed [area](surface-area.md) under the [pressure](pressure-split.md)-[volume](volume-thermodynamics.md) curve. [Isothermal expansion](isothermal-expansion.md) gives positive [work](work.md); [isothermal compression](isothermal-compression.md) gives negative [work](work.md). A convention counting [work](work.md) done on the [gas](gas.md) instead has $W_{\rm on}=-W_{\rm by}$.[§3.2, equations 3.3–3.4, Figure 3.5 and the isothermal integral following Figure 3.6](university-physics-volume-2-by-samuel-j-ling-and-others/3-2-work-heat-and-internal-energy.md)

For a calculated example, let $n=1\,\mathrm{mol}$, $T=300\,\mathrm K$ and $V_i=10\,\mathrm L$, $V_f=20\,\mathrm L$. The [pressure](pressure-split.md) falls from approximately $249.4$ to $124.7\,\mathrm{kPa}$, and

$$
W_{\rm by,rev}=Q=nRT\ln2\approx1.729\,\mathrm{kJ},\qquad \Delta U=0.
$$

Traversing the same [isothermal process](isothermal-process.md) backward changes both transfer signs: $W_{\rm by,rev}=Q\approx-1.729\,\mathrm{kJ}$. Neither direction changes [internal energy of an ideal gas](internal-energy-of-an-ideal-gas.md). These stipulated values illustrate the [energy](energy-split.md) balance; they are not experimental measurements.

<a id="image-signed-work-along-an-ideal-gas-isotherm-expansion-and-compression"></a>
![](isothermal-ideal-gas-signed-work-area.png)

**[Figure 2](#image-signed-work-along-an-ideal-gas-isotherm-expansion-and-compression). Signed work along an ideal-gas isotherm: expansion and compression**.

The shaded geometric [area](surface-area.md) is positive in both panels; the direction of the [integral](integral-split.md) supplies the sign of [work](work.md). Knowing only the two equilibrium endpoints does not justify shading this curve for an irreversible process. For an idealized piston moving against a specified external resisting [pressure](pressure-split.md), boundary [work](work.md) is $W_{\rm by}=\int p_{\rm ext}\,dV$. Substitution of the equilibrium [gas](gas.md) [pressure](pressure-split.md) requires the appropriate reversible limit. In [free expansion](free-expansion.md) into [vacuum](vacuum.md), $p_{\rm ext}=0$ and this boundary [work](work.md) is zero.

## ↑ Ancestors (9)

1. [Isothermal process](isothermal-process.md)
2. [Carnot cycle](carnot-cycle.md)
3. [Carnot's theorem](carnot-s-theorem.md)
4. [Second law of thermodynamics](second-law-of-thermodynamics-split.md)
5. [Thermodynamics](thermodynamics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Boyle's law](boyle-s-law.md)
- [Isothermal compression](isothermal-compression.md)
- [Isothermal expansion](isothermal-expansion.md)
- [Isothermal process](isothermal-process.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2b/section-a/1/solution.md)
