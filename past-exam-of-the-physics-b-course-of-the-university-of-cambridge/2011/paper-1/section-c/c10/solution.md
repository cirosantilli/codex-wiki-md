<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

Use $c_p,c_V$ for the [heat capacities](../../../../../heat-capacity.md) of the entire $n$-mole sample. For a stable simple compressible gas, a [Maxwell relation](../../../../../maxwell-relations.md) gives

$$
c_p-c_V=T\left(\frac{\partial p}{\partial T}\right)_V\left(\frac{\partial V}{\partial T}\right)_p
=\frac{TV\alpha_V^2}{\kappa_T}\geq0,
$$

where $\alpha_V=V^{-1}(\partial V/\partial T)_p$ and $\kappa_T=-V^{-1}(\partial V/\partial p)_T>0$. This [heat-capacity difference and mechanical stability](../../../../../heat-capacity-difference-and-mechanical-stability.md) explains the sign without assuming the [internal energy](../../../../../internal-energy-split.md) depends only on [temperature](../../../../../temperature-split.md). It is strictly positive for an ordinary expanding gas; the unrestricted word “always” needs the qualification that equality is possible when [thermal expansion](../../../../../thermal-expansion.md) vanishes.

For an [ideal gas](../../../../../ideal-gas-split.md), thermodynamic consistency gives

$$
\left(\frac{\partial U}{\partial V}\right)_T
=T\left(\frac{\partial p}{\partial T}\right)_V-p=0.
$$

Consequently $U=U(T)$, while $H=U+pV=U+nRT$. Differentiating gives **$c_p-c_V=nR$**: at fixed [pressure](../../../../../pressure-split.md) extra supplied [heat](../../../../../heat-split.md) permits expansion work in addition to the internal-energy increase.

Differentiate the supplied [entropy](../../../../../entropy-split.md) at fixed $n$:

$$
\frac1T=\left(\frac{\partial S}{\partial U}\right)_{V,n}=\frac{5nR}{2U},\qquad
\frac pT=\left(\frac{\partial S}{\partial V}\right)_{U,n}=\frac{nR}{V}.
$$

Thus $U=5nRT/2$, consistently recovering $pV=nRT$, and

$$
\boxed{c_V=\frac52nR,\qquad c_p=\frac72nR.}
$$

The coefficient in this [entropy](../../../../../entropy-split.md) corresponds to five active quadratic thermal degrees of freedom per molecule. It should not be replaced by the monatomic value. Reference scales needed to make logarithms dimensionless are absorbed into the [entropy](../../../../../entropy-split.md) constant and do not affect these [derivatives](../../../../../derivative.md).

With open windows the house equilibrates mechanically at approximately the same atmospheric [pressure](../../../../../pressure-split.md) before and after heating. It is an open system: its mole number is not fixed. The [isobaric ideal-gas internal-energy density](../../../../../isobaric-ideal-gas-internal-energy-density.md) is

$$
\boxed{\frac UV=\frac52\frac{nRT}{V}=\frac52p,\qquad
\frac{(U/V)_{300}}{(U/V)_{273}}=1.}
$$

At a fixed house [volume](../../../../../volume.md), $n_{300}/n_{273}=273/300=0.91$: fewer molecules occupy the house, each with greater mean [energy](../../../../../energy-split.md). Heating [energy](../../../../../energy-split.md) can enter while [enthalpy](../../../../../enthalpy-split.md) leaves with escaping air. Treating the room as a sealed fixed-$n$ gas would give the wrong energy-density comparison.

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
