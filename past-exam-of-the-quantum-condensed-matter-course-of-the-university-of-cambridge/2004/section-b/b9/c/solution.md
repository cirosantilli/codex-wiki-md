<h1 id="section-b/b9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An n-channel [MOSFET](../../../../../mosfet.md) has two heavily n-doped source and drain regions in a p-type body, with an insulated gate above the intervening surface. A positive gate voltage first depletes surface [electron holes](../../../../../electron-hole.md) and then induces an [electron](../../../../../electron.md) [semiconductor inversion layer](../../../../../semiconductor-inversion-layer.md). Above threshold $V_T$ this layer connects source to drain. Gate voltage controls the channel charge through the oxide capacitance, while the insulating gate permits a very small steady gate current.

<a id="section-b/b9/c/image-an-induced-electron-channel-connects-the-source-and-drain-of-an-n-channel-mosfet"></a>
![](../../../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004-mosfet-cross-section.png)

**[Figure 2](#section-b/b9/c/image-an-induced-electron-channel-connects-the-source-and-drain-of-an-n-channel-mosfet). An induced electron channel connects the source and drain of an n-channel MOSFET**. Original schematic cross-section in the on state. The oxide separates the gate electrically from the body; the thin surface channel is an inversion layer rather than a permanently n-doped bridge.

For the [long-channel MOSFET current law](../../../../../long-channel-mosfet-current-law.md), let $C_{\rm ox}$ be oxide capacitance per area, $W,L$ channel width and length, and use constant mobility $\mu_n$. In the gradual-channel approximation,

$$
I_D=\mu_nC_{\rm ox}\frac WL\left[(V_{GS}-V_T)V_{DS}-\frac{V_{DS}^2}{2}\right],\qquad0<V_{DS}<V_{GS}-V_T.
$$

At larger drain voltage the ideal channel pinches off near the drain and the current saturates at

$$
\boxed{I_{D,\rm sat}=\frac12\mu_nC_{\rm ox}\frac WL(V_{GS}-V_T)^2.}
$$

Carriers still flow through the pinch-off region; pinch-off does not mean zero drain current. These formulas neglect channel-length modulation, short-channel effects and velocity saturation. A p-channel device reverses the carrier type and operating polarities. Gate control makes MOSFETs useful as electronic switches and amplifiers.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [B9](../../b9.md)
3. [Section B](../../../section-b.md)
4. [2004](../../../../2004-split.md)
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
