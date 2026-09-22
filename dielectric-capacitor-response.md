# Dielectric capacitor response

↑ **Parent:** [Dielectric](dielectric.md)

Compare two initially identical [parallel-plate capacitors](parallel-plate-capacitor.md) with plate [area](surface-area.md) $A$, fixed gap $d$, [vacuum](vacuum.md) [capacitance](capacitance.md) $C_0=\epsilon_0A/d$, and initial [electric potential difference](electric-potential-difference.md) $V_0$. Completely fill both gaps with the same uniform linear [dielectric](dielectric.md) of static [relative permittivity](relative-permittivity.md) $\epsilon_r>1$, neglecting the [fringing field of a capacitor](fringing-field-of-a-capacitor.md). Keep one connected to an ideal voltage source and isolate the other. The geometric [capacitance](capacitance.md) becomes $C=\epsilon_r C_0$ in both cases; the electrical constraint determines what else changes.[§8.4, Figure 8.17 and equation (8.11): isolated capacitor, unchanged free plate charge and increased capacitance](university-physics-volume-2-by-samuel-j-ling-and-others/8-4-capacitor-with-a-dielectric.md)

Write $Q_0=C_0V_0$, $E_0=V_0/d$ and $U_0=C_0V_0^2/2$. Applying $Q=CV$, $E=V/d$ and the [capacitor energy](capacitor-energy.md) formula gives the complete comparison:

$$
\begin{array}{c|cc}
&\text{fixed voltage}&\text{isolated, fixed charge}\\ \hline
C/C_0&\epsilon_r&\epsilon_r\\
Q/Q_0&\epsilon_r&1\\
V/V_0&1&1/\epsilon_r\\
E/E_0&1&1/\epsilon_r\\
U/U_0&\epsilon_r&1/\epsilon_r
\end{array}
$$

Thus the statement that a [dielectric](dielectric.md) reduces the [electric field](electric-field-split.md) needs the fixed-free-charge condition. With fixed [electric potential difference](electric-potential-difference.md), the voltage source supplies additional free plate [electric charge](electric-charge-split.md), maintaining $E=V_0/d$ despite the new bound [electric charges](electric-charge-split.md).

<a id="image-dielectric-capacitor-response-at-fixed-voltage-and-fixed-charge"></a>
![](dielectric-capacitor-voltage-and-charge-constraints.png)

**[Figure 3](#image-dielectric-capacitor-response-at-fixed-voltage-and-fixed-charge). Dielectric capacitor response at fixed voltage and fixed charge**. Original normalized comparison for the stipulated model $\epsilon_r=3$: every ratio is relative to the same initially charged [vacuum](vacuum.md) [capacitor](capacitor.md). The dashed line marks the initial value. The bars show final values, not a time history or measured data. Plate geometry is unchanged and the [dielectric](dielectric.md) completely fills the gap.

For the stipulated $\epsilon_r=3$ example, the voltage source supplies $\Delta Q=2Q_0$. At constant $V_0$, its delivered electrical [work](work.md) is $V_0\Delta Q=4U_0$, whereas the increase in [capacitor energy](capacitor-energy.md) is $2U_0$. In an ideal reversible quasistatic insertion, the remaining $2U_0$ is mechanical [work](work.md) delivered by the assembly, as accounted for in [fixed-voltage capacitor energy balance](fixed-voltage-capacitor-energy-balance.md). For the isolated assembly, [capacitor energy](capacitor-energy.md) falls from $U_0$ to $U_0/3$, allowing $2U_0/3$ of mechanical [work](work.md) in the same ideal limit. Actual losses reduce recoverable [work](work.md); energy increases in the connected case do not arise from the [dielectric](dielectric.md) supplying free [energy](energy-split.md).

## ↑ Ancestors (6)

1. [Dielectric](dielectric.md)
2. [Permittivity](permittivity-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Dielectric](dielectric.md)
- [Dielectric capacitor response](dielectric-capacitor-response.md)
- [Electrical insulator](electrical-insulator.md)
