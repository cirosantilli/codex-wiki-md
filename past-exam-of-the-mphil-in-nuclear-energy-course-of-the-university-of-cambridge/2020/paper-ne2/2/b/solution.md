<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Continue the same-rod-number and same-height comparison from part(a), and assume unchanged pump speed, similar inlet conditions and single-phase forced flow for the normal-operation hydraulic argument.

**[Core power density](../../../../../core-power-density.md) increases.** The active core volume decreases while total thermal power stays fixed. The fuel's own average volumetric power and the mean [fuel linear heat rate](../../../../../fuel-linear-heat-rate.md) do not increase merely from bringing the same rods closer together: fuel volume and rod count are unchanged.

**[Coolant](../../../../../coolant.md) [mass flow rate](../../../../../mass-flow-rate.md) normally decreases.** Tighter passages reduce flow area and [hydraulic diameter](../../../../../hydraulic-diameter.md), increasing the core's hydraulic resistance. The unchanged [centrifugal pumps](../../../../../centrifugal-pump.md) do not enforce constant flow. The [pump operating point](../../../../../pump-operating-point.md) moves to the intersection of the same pump curve with the steeper system-resistance curve, normally giving smaller flow at greater pump head.[Module HT-03, pp.51–53, System Characteristic Curve and System Operating Point, Figure10](../../../../../thermodynamics-heat-transfer-and-fluid-flow-volume-3-by-the-united-states-department-of-energy.md)

**The core [pressure](../../../../../pressure-split.md) drop normally increases for the usual pump curve.** Its resistance at any given flow is higher. At the new, smaller flow, unchanged external piping and component losses are smaller, whereas a conventional falling pump head-versus-flow curve gives greater available head. The core takes the difference. This conclusion uses the stated pump-curve assumptions; holding flow fixed or holding pump head fixed would be different models. The exact new flow and pressure drop need both system and pump characteristics.

**Fuel [temperature](../../../../../temperature-split.md) would normally tend to rise, especially downstream, if the loss of flow increases coolant heating without a compensating improvement in film heat transfer.** At fixed inlet state,

$$
P\simeq\dot m c_p(T_{\rm out}-T_{\rm in})
$$

shows that smaller total [mass flow rate](../../../../../mass-flow-rate.md) raises the bulk coolant temperature rise. At unchanged local [fuel linear heat rate](../../../../../fuel-linear-heat-rate.md), the fuel-to-surface conductive contribution is approximately unchanged if material properties and gap conditions are held fixed. Its boundary [temperature](../../../../../temperature-split.md) and the coolant film drop can nevertheless change.

The local [coolant mass flux](../../../../../coolant-mass-flux.md) is $G=\dot m/A_f$. Both total flow and flow area decrease, so the sign of the change in $G$, the [heat transfer coefficient](../../../../../heat-transfer-coefficient.md) and the fuel [temperature](../../../../../temperature-split.md) cannot be deduced from total flow alone. Changes in power peaking and inlet conditions add further qualifications to the usual hotter-fuel tendency.

**The [minimum departure from nucleate boiling ratio](../../../../../minimum-departure-from-nucleate-boiling-ratio.md) would commonly decrease, implying reduced boiling margin, but its sign is conditional.** The defining local ratio is

$$
\mathrm{DNBR}=\frac{q''_{\rm crit}}{q''_{\rm actual}},\qquad
\mathrm{MDNBR}=\min_{\rm core}\mathrm{DNBR}.
$$

The numerator is the [critical heat flux](../../../../../critical-heat-flux.md) for the local conditions, and the denominator is actual rod-surface [heat flux](../../../../../heat-flux-density.md).[Departure from nucleate boiling ratio entry](../../../../../reactor-glossary-by-the-united-states-nuclear-regulatory-commission.md) The mean surface heat loading remains approximately unchanged for the same rods and total power. Greater coolant enthalpy rise tends to reduce margin, while changes in $G$, geometry, pressure and local power determine the actual critical heat flux. A geometry-appropriate correlation or experiment is needed for a definite MDNBR change; unchanged hardware does not supply it.

## ↑ Ancestors (10)

1. [B](../b.md)
2. [2](../../2.md)
3. [Module NE2](../../../paper-ne2-split.md)
4. [2020](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
