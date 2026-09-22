<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [GaAs](../../../../gallium-arsenide.md)–AlGaAs [semiconductor heterostructure](../../../../semiconductor-heterostructure.md) confines electrons normal to the interface in a [semiconductor quantum well](../../../../quantum-well.md). Remote [modulation doping](../../../../modulation-doping.md) supplies a high-mobility [two-dimensional electron gas](../../../../two-dimensional-electron-gas.md). Negative split gates deplete it laterally, leaving a narrow [quantum point contact](../../../../quantum-point-contact.md) with discrete transverse subbands and continuous longitudinal momentum. A single occupied subband requires transverse excitation gaps larger than thermal and applied-bias energies.

Take $e>0$ and count **one spin-resolved channel**. In a length $L$, right-moving states have density $L\,dk/(2\pi)$; each contributes charge current $-ev_k/L$. Thus

$$
I^+=-\frac e{2\pi}\int_0^\infty v_k f_L\,dk,\qquad I^-_{\rm signed}=+\frac e{2\pi}\int_0^\infty v_k f_R\,dk.
$$

The second expression is the right reservoir's left-moving contribution expressed in the same left-to-right conventional-current sign. Since $v_k\,dk=dE/\hbar$,

$$
I=\frac eh\int_{E_0}^\infty[f(E;\mu,T)-f(E;\mu-eV,T)]\,dE,
\qquad\boxed{G=\frac{e^2}{h}f(E_0;\mu,T)\longrightarrow\frac{e^2}{h}.}
$$

The limit needs $k_BT,|eV|\ll\mu-E_0$ and [ballistic transport](../../../../ballistic-transport.md). Velocity cancels the one-dimensional state density. Two degenerate spin channels give $2e^2/h$, not an extra factor hidden in the quoted single-channel result.

For elastic phase-coherent scattering, expand each incident flux-normalized mode in outgoing lead modes. Its transmitted fraction is $|(t_E)_{nm}|^2$; sum over all open outgoing $n$ and occupied incident $m$. Linearizing the reservoir occupations gives the [Landauer formula](../../../../landauer-formula.md)

$$
\boxed{G=\frac{e^2}{h}\int dE\,[-f'(E)]\operatorname{tr}(t_E^\dagger t_E).}
$$

The source's $T_E^+$ denotes this amplitude matrix, not temperature or a probability matrix. Flux normalization is essential: ordinary wave-amplitude ratios need a velocity factor. Reservoirs equilibrate, contacts supply incoming Fermi distributions, and inelastic processes within the channel are neglected. Spin is included among channel labels. At $T\to0$, only transmissions at $\mu$ contribute; perfect channels each add one quantum. This is a two-terminal conductance including contact resistance, even with no internal backscattering.

Trace I has steps near integer $2e^2/h$ as less-negative gate voltage opens successive spin-degenerate subbands. At the printed parallel field $11\,\mathrm T$, [Zeeman splitting](../../../../zeeman-splitting.md) separates the two spin thresholds, allowing approximately half-sized steps in the plotted units; the onset also shifts. Thermal broadening, imperfect transmission and unresolved thresholds round the plateaux. A parallel field primarily resolves spin in the ideal thin-interface model; finite layer thickness can also shift subband energies. The plot alone does not determine a unique effective $g$ factor or microscopic disorder model.

<a id="2/image-illustrative-spin-resolved-channel-thresholds-produce-full-or-half-sized-conductance-steps"></a>
![](../../../../past-exam-of-the-advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge/2014/paper-1-aqc2014-channel-steps.png)

**[Figure 1](#2/image-illustrative-spin-resolved-channel-thresholds-produce-full-or-half-sized-conductance-steps). Illustrative spin-resolved channel thresholds produce full or half-sized conductance steps**. [Source](paper-1-aqc2014-channel-steps.py).

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
