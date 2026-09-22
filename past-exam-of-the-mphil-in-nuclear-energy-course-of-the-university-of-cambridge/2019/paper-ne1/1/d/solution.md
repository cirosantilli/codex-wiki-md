<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**In the stated model, the limiting thicknesses are about $0.163\ \mathrm m$ of lead or $0.780\ \mathrm m$ of concrete.** Use the unshielded [equivalent dose](../../../../../equivalent-dose.md) rate from part (c), $\dot H_0=556.815\ \mathrm{\mu Sv\,h^{-1}}$. Let $x=\mu t$, where $\mu$ is the supplied total [linear attenuation coefficient](../../../../../linear-attenuation-coefficient.md). The stipulated [radiation buildup factor](../../../../../radiation-buildup-factor.md) gives the requirement

$$
\dot H_0(1+x)e^{-x}<3\ \mathrm{\mu Sv\,h^{-1}},
\qquad
(1+x)e^{-x}<\frac{3}{556.815}=0.00538778.
$$

The left side decreases for $x>0$ because its derivative is $-xe^{-x}$. Solving the equality gives a unique threshold,

$$
x_*=7.34532.
$$

Thus, with the source-to-observation distance kept at one metre,

$$
\boxed{t_{\rm Pb}>\frac{x_*}{45.2}=0.162507\ \mathrm m,
\qquad
t_{\rm concrete}>\frac{x_*}{9.42}=0.779758\ \mathrm m.}
$$

For example, rounding upward to $0.17\ \mathrm m$ of [lead](../../../../../lead.md) or $0.80\ \mathrm m$ of concrete satisfies the stipulated inequality. Equality at the threshold is not sufficient for the strictly smaller target.

A compact surrounding shield favours [lead](../../../../../lead.md); concrete trades much greater thickness for a common structural material. The densities permit a useful planar comparison: the threshold areal masses $\rho t$ are about $1.84\times10^3$ and $1.87\times10^3\ \mathrm{kg\,m^{-2}}$, respectively. **The thinner shield is not proportionately lighter per equal projected area.** Total enclosure [mass](../../../../../mass.md) also depends on geometry.

The idealized outline is continuous coverage around the source with the required material path length, including the closure; a direct unshielded line through a gap would invalidate this attenuation estimate. The calculation assumes the quoted observation distance, the fixed effective photon coefficients and the prescribed [radiation buildup factor](../../../../../radiation-buildup-factor.md). It is not based on the more optimistic uncollided [exponential attenuation](../../../../../exponential-attenuation.md) alone.

## ↑ Ancestors (10)

1. [D](../d.md)
2. [1](../../1.md)
3. [Module NE1](../../../paper-ne1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
