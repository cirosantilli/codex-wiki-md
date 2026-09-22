<h1 id="section-b/b4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [field-effect transistor](../../../../../field-effect-transistor.md) uses a gate voltage to control the conducting channel between source and drain. In a [MOSFET](../../../../../mosfet.md), the gate is insulated from the semiconductor: an electric field changes the channel carrier population with little steady gate current. An n-channel device creates an [semiconductor inversion layer](../../../../../semiconductor-inversion-layer.md) when the gate sufficiently attracts electrons to a p-type surface. The drain supply provides the output power; the gate controls that flow.

The [long-channel MOSFET current law](../../../../../long-channel-mosfet-current-law.md) follows from the gradual-channel approximation. With gate capacitance per area $C_{\rm ox}$, threshold voltage $V_T$, channel width $W$, length $L$, constant [charge carrier mobility](../../../../../charge-carrier-mobility.md) $\mu$ and $V_{
m ov}=V_{GS}-V_T>0$, the local sheet charge magnitude is $C_{\rm ox}(V_{
m ov}-V(x))$. Integrating the drift current along the channel gives

$$
\boxed{I_D=\mu C_{\rm ox}\frac WL\left(V_{
m ov}V_{DS}-\frac{V_{DS}^2}{2}\right),\quad0\leq V_{DS}\leq V_{
m ov}.}
$$

At $V_{DS}=V_{
m ov}$, the drain end reaches pinch-off. The ideal long-channel saturation current is $I_D=\mu C_{\rm ox}WV_{
m ov}^2/(2L)$; this assumes negligible channel-length modulation. A [junction field-effect transistor](../../../../../junction-field-effect-transistor.md) instead changes the channel width through a reverse-biased depletion region.

Experimentally, measure $I_D$ against $V_{GS}$ at fixed drain bias to see gate control, and against $V_{DS}$ at several fixed gate biases to distinguish the approximately linear and saturation regimes. Simultaneously checking gate leakage tests the insulated-gate assumption.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [B4](../../b4.md)
3. [Section B](../../../section-b.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter course of the University of Cambridge](../../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
