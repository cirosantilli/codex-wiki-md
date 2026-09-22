<h1 id="36a/solution">Solution</h1>

↑ **Parent:** [36A](../36a.md)

For a simple system of fixed composition, the [first law of thermodynamics](../../../../../first-law-of-thermodynamics.md) and

$$
G=E-TS+PV
$$

give

$$
dG=-S\,dT+V\,dP.
$$

Thus

$$
S=-\left(\frac{\partial G}{\partial T}\right)_P,
\qquad
V=\left(\frac{\partial G}{\partial P}\right)_T.
$$

Equality of mixed derivatives gives the [Gibbs free-energy Maxwell relation](../../../../../gibbs-free-energy-maxwell-relation.md)

$$
\boxed{
\left(\frac{\partial S}{\partial P}\right)_T
=-\left(\frac{\partial V}{\partial T}\right)_P
}.
$$

The [heat capacity at constant volume](../../../../../heat-capacity-at-constant-volume.md) and [heat capacity at constant pressure](../../../../../heat-capacity-at-constant-pressure.md) are

$$
C_V=\left(\frac{\partial E}{\partial T}\right)_V
=T\left(\frac{\partial S}{\partial T}\right)_V,
$$



$$
C_P=\left(\frac{\partial H}{\partial T}\right)_P
=T\left(\frac{\partial S}{\partial T}\right)_P,
\qquad H=E+PV.
$$

Regarding $S$ as a function of $T,V$ and differentiating along a constant-pressure curve gives

$$
\left(\frac{\partial S}{\partial T}\right)_P
=\left(\frac{\partial S}{\partial T}\right)_V
+\left(\frac{\partial S}{\partial V}\right)_T
\left(\frac{\partial V}{\partial T}\right)_P.
$$

The Maxwell relation from the Helmholtz free energy is

$$
\left(\frac{\partial S}{\partial V}\right)_T
=\left(\frac{\partial P}{\partial T}\right)_V.
$$

Therefore the [difference between constant-pressure and constant-volume heat capacities](../../../../../difference-between-constant-pressure-and-constant-volume-heat-capacities.md) is

$$
\boxed{
C_P-C_V
=T\left(\frac{\partial V}{\partial T}\right)_P
\left(\frac{\partial P}{\partial T}\right)_V
}.
$$

Along the liquid-gas [phase coexistence curve](../../../../../phase-coexistence-curve.md), the molar Gibbs free energies agree. Differentiating $G_{\rm l}=G_{\rm g}$ along the curve gives

$$
-S_{\rm l}\,dT+V_{\rm l}\,dP
=-S_{\rm g}\,dT+V_{\rm g}\,dP.
$$

Hence the [Clausius-Clapeyron relation](../../../../../clausius-clapeyron-relation.md) is

$$
\boxed{
\frac{dP}{dT}
=\frac{S_{\rm g}-S_{\rm l}}{V_{\rm g}-V_{\rm l}}
=\frac{L}{T(V_{\rm g}-V_{\rm l})}
},
$$

where $L=T(S_{\rm g}-S_{\rm l})$ is the molar [latent heat](../../../../../latent-heat.md).

If $V_{\rm g}\gg V_{\rm l}$ and the gas is ideal, then $V_{\rm g}=RT/P$, so

$$
\frac{dP}{dT}\simeq\frac{LP}{RT^2}.
$$

For constant $L$, integration yields

$$
\boxed{
\log P=C-\frac{L}{RT},
\qquad
P(T)=P_0e^{-L/(RT)}
},
$$

where $P_0$ is constant over the range in which the approximations apply.

## ↑ Ancestors (10)

1. [36A](../36a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
