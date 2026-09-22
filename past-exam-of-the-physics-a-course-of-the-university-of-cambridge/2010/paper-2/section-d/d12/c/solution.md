<h1 id="section-d/d12/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use an enclosure with [thermal insulation](../../../../../../thermal-insulation.md) and sufficient [heat capacity](../../../../../../heat-capacity.md) to slow the response to ambient changes. Block draughts and direct radiant heating, use low-conductance supports and thermal breaks in wiring, and reduce [thermal radiation](../../../../../../thermal-radiation.md) with low-emissivity shields. Vacuum suppresses gas [thermal conduction](../../../../../../thermal-conduction.md) and [convection](../../../../../../convection-split.md) but leaves [thermal radiation](../../../../../../thermal-radiation.md) and solid [thermal conduction](../../../../../../thermal-conduction.md). A conducting inner shield helps make [temperature](../../../../../../temperature-split.md) uniform; it is not by itself [thermal insulation](../../../../../../thermal-insulation.md).

For a lumped load of [heat capacity](../../../../../../heat-capacity.md) $C_{\rm th}$ coupled to the room by [thermal conductance](../../../../../../thermal-conductance.md) $G$, the [first-order thermal isolation](../../../../../../first-order-thermal-isolation.md) model is

$$
C_{\rm th}\frac{d\delta T}{dt}+G\delta T=G\delta T_a+\delta P,\qquad
\boxed{\frac{\delta T(\omega)}{\delta T_a(\omega)}=\frac1{1+i\omega\tau},\quad\tau=\frac{C_{\rm th}}G}.
$$

Large [thermal resistance](../../../../../../thermal-resistance.md) and [heat capacity](../../../../../../heat-capacity.md) attenuate fast fluctuations; nested shields can provide several filtering stages. **Passive [thermal insulation](../../../../../../thermal-insulation.md) does not reject arbitrarily slow ambient drift**, since this transfer approaches one at zero [frequency](../../../../../../frequency.md). It also increases the [temperature](../../../../../../temperature-split.md) rise $\delta P/G$ caused by internal dissipation.

For long-term stability use a regulated bath or [thermostat](../../../../../../thermostat.md), placing a calibrated sensor near the sensitive component. Heater feedback rejects slow disturbances, provided sensor lag, loop stability, actuator range and electrical pickup are controlled. Maintain stable internal power, allow equilibration, record both room and load [temperatures](../../../../../../temperature-split.md), and test rejection by a deliberate ambient-temperature step or sinusoidal modulation. These measurements reveal gradients and thermal bypasses that an [thermal insulation](../../../../../../thermal-insulation.md) label alone cannot establish.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2010](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
