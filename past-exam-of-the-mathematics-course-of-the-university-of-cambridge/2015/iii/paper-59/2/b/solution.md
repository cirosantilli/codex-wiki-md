<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a dry [ideal gas](../../../../../../ideal-gas.md) of fixed composition with specific gas constant $\mathcal R=C_p-C_v$ and constant [specific heat capacity at constant pressure](../../../../../../specific-heat-capacity-at-constant-pressure.md) $C_p$. For a fixed-mass parcel, $PV^\gamma=$ constant and $PV=m_{\rm parcel}\mathcal RT_g$ imply

$$
T_gP^{-(\gamma-1)/\gamma}=\mathrm{constant},\qquad \frac{dT_g}{dP}=\frac{\mathcal R}{C_p}\frac{T_g}{P}=\frac1{\rho_gC_p}.
$$

Along a hydrostatic adiabat, $dP/dz=-\rho_gg$; hence the [dry adiabatic lapse rate](../../../../../../dry-adiabatic-lapse-rate.md) is

$$
\boxed{\left(\frac{dT_g}{dz}\right)_{\rm ad}=-\frac g{C_p}.}
$$

For an actual pressure-balanced parcel rising in an ambient atmosphere, $dP/dz=-\rho_{\rm env}g$ instead gives $dT_g/dz=-(g/C_p)(T_g/T_{\rm env})$. The usual lapse-rate expression is exact for a hydrostatic adiabatic column and is the local first-order result at the launch point where $T_g=T_{\rm env}$, as needed in a linear stability test. Treating an already much hotter parcel as an exact copy of the ambient hydrostatic column would be an extra approximation.

After a small upward displacement $\delta z$ from temperature equilibrium, its temperature excess is

$$
T_g-T_{\rm env}\simeq\left[-\frac g{C_p}-\frac{dT_{\rm env}}{dz}\right]\delta z.
$$

At equal pressure, warmer gas is less dense and continues to rise. Thus the [Schwarzschild criterion](../../../../../../schwarzschild-criterion.md) in altitude form is

$$
\boxed{\frac{dT_{\rm env}}{dz}<-\frac g{C_p}\quad\text{unstable},\qquad \frac{dT_{\rm env}}{dz}=-\frac g{C_p}\quad\text{neutral}.}
$$

The supplied non-strict inequality includes the marginal case; strict growth requires the strict inequality. A downward displacement gives the same stability conclusion. Efficient [convection](../../../../../../convection.md) normally adjusts an initially superadiabatic gradient to a nearly adiabatic one.

Deep envelopes of [gas giants](../../../../../../gas-giant.md) and [ice giants](../../../../../../ice-giant.md) commonly transport intrinsic heat by [convection](../../../../../../convection.md), as do the [planetary tropospheres](../../../../../../planetary-troposphere.md) of many weakly irradiated atmospheres. [Earth](../../../../../../earth.md)'s dry [troposphere](../../../../../../troposphere.md) provides another approximate example, with moisture changing the lapse rate. Strongly irradiated [hot Jupiters](../../../../../../hot-jupiter.md) can still have deep convective interiors, while their upper radiative regions need not be convective. Composition gradients can modify the homogeneous-gas criterion and inhibit overturning even in an interior.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
