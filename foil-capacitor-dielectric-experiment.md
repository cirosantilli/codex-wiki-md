# Foil capacitor dielectric experiment

↑ **Parent:** [Dielectric capacitance measurement](dielectric-capacitance-measurement.md)

Southern Methodist University's teaching lab, Introduction to the Parallel Plate Capacitor Lab, makes the response tangible with a [capacitor](capacitor.md) assembled from aluminium foil, paper and taped wire contacts. Its instructions specify approximately $10\,\mathrm{cm}\times10\,\mathrm{cm}$ foil rectangles, aligned with the paper completely separating them. A [multimeter](multimeter.md) in [capacitance](capacitance.md) mode supplies the readout; a ruler measures plate dimensions and a micrometer measures specimen thickness. The lab replaces the paper with other sheets, including cardstock, plastic wrap and wax paper. It asks students to keep foil [area](surface-area.md) and alignment consistent, measure thickness at several positions, estimate thickness uncertainty, and wait for the [capacitance](capacitance.md) reading to stabilize. These are published preparation and measurement instructions, not measured results reported here.[Experiments 1–2, Equipment You Will Be Using, and final construction and dielectric-study instructions](smu-physics-110x-labs/introduction-to-the-parallel-plate-capacitor-lab.md)

The inference uses each specimen's own thickness $t$, not just a comparison of raw meter readings. With corrected [capacitance](capacitance.md) $C_s$ and overlapping [area](surface-area.md) $A$, the ideal estimate is $\epsilon_r=C_s t/(\epsilon_0A)$. A thicker sheet can give a smaller [capacitance](capacitance.md) despite larger [relative permittivity](relative-permittivity.md). This is why changing material while letting the plate gap change does not isolate [electric susceptibility](electric-susceptibility.md) by itself.

Useful additional controls are to keep leads in the same positions, use [capacitance measurement calibration](capacitance-measurement-calibration.md), repeat one sheet after the others to check drift, and repeat the assembly to assess contact reproducibility. An air-gap reference must have known spacers maintaining the same separation; removing a supporting sheet and letting the foil touch is not such a reference. Record the instrument's test [frequency](frequency.md) and measurement mode when available. A [capacitance](capacitance.md) display alone does not establish negligible [dielectric loss](dielectric-loss.md) or a strictly static [permittivity](permittivity-split.md). These are proposed controls extending the published teaching instructions.

Air gaps produce a particularly revealing systematic error. Suppose a uniform sheet of thickness $t$ and [relative permittivity](relative-permittivity.md) $\epsilon_r$ is separated from the [electrodes](electrode.md) by air layers of total thickness $g$. Approximate air [permittivity](permittivity-split.md) by [vacuum permittivity](vacuum-permittivity.md), neglect the [fringing field of a capacitor](fringing-field-of-a-capacitor.md) and use the same [area](surface-area.md) in each layer. The common normal [electric displacement field](electric-displacement-field.md) has magnitude $D=Q/A$, so integrating the [electric field](electric-field-split.md) through the layers gives

$$
V=\frac{Q}{\epsilon_0A}\left(g+\frac{t}{\epsilon_r}\right),\qquad
C_s=\frac{\epsilon_0A}{g+t/\epsilon_r}.
$$

If the analyst inserts the sheet thickness alone into the ideal filled-gap formula, the inferred value is

$$
\widehat\epsilon_r=\frac{C_s t}{\epsilon_0A}
=\frac{\epsilon_r}{1+\epsilon_r g/t}.
$$

For the stipulated model $\epsilon_r=3$ and $g=t/10$, this gives $\widehat\epsilon_r=30/13\simeq2.308$, not three. These values are calculated examples, not measured sheet properties. If total plate separation $d=t+g$ is used instead, the effective estimate is $(t+g)/(g+t/\epsilon_r)$; it still mixes the sheet and the air. Thus measuring a thickness accurately cannot compensate for an unrecognized layer.

The [fringing field of a capacitor](fringing-field-of-a-capacitor.md) and additive lead [capacitance](capacitance.md) further limit a foil measurement. Keep lateral plate dimensions large relative to separation, and use a [guard electrode of a capacitor](guard-electrode-of-a-capacitor.md) in a suitable fixture for more demanding work.[Solution: guarded three-electrode fixture, fringe capacitance, specimen flatness and air gaps](materials-measurement-dielectric-materials.md) A family of thickness measurements can help distinguish material response from an additive offset, but air gaps can vary with the assembly. A large, repeatable reading supports a [capacitance](capacitance.md) change; extracting a material [electric susceptibility](electric-susceptibility.md) requires the geometry, gaps, instrument response and [dielectric loss](dielectric-loss.md) assumptions to survive these checks. No measured [relative permittivity](relative-permittivity.md) is claimed for any of the lab's sheets.

## ↑ Ancestors (6)

1. [Dielectric capacitance measurement](dielectric-capacitance-measurement.md)
2. [Permittivity](permittivity-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
