<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the supplied $-50\,\mathrm{kJ\,mol^{-1}}$ as a standard transformed [Gibbs free energy](../../../../gibbs-free-energy.md) of [ATP hydrolysis](../../../../atp-hydrolysis.md), rather than replacing it with a different commonly quoted standard value. Approximate [thermodynamic activities](../../../../thermodynamic-activity.md) by [concentrations](../../../../concentration.md) divided by $c^\circ=1\,\mathrm M$, at an explicitly assumed $T=300\,\mathrm K$. The dimensionless reaction quotient is

$$
Q_h=\frac{([\mathrm{ADP}]/c^\circ)([P_i]/c^\circ)}{[\mathrm{ATP}]/c^\circ}
=\frac{(0.0008)(0.010)}{0.0016}=0.005.
$$

Consequently

$$
\Delta G_h=\Delta G_h^\circ+RT\ln Q_h
=-50.0-13.22=-63.22\,\mathrm{kJ\,mol^{-1}},
$$

and the reverse synthesis cost is $g_{\rm ATP}=63.22\,\mathrm{kJ\,mol^{-1}}$. Substituting bare millimolar numbers in this quotient without the [standard state](../../../../standard-state.md) would give the wrong logarithm.

For outside-to-inside [proton](../../../../proton.md) movement, the [membrane potential](../../../../membrane-potential-split.md) is $\Delta\psi=-0.125\,\mathrm V$ and $\mathrm{pH}_{\rm in}-\mathrm{pH}_{\rm out}=0.5$, so $[H^+]_{\rm in}/[H^+]_{\rm out}=10^{-0.5}$. The molar [electrochemical potential](../../../../electrochemical-potential.md) change is

$$
\Delta\widetilde\mu_H=F\Delta\psi+RT\ln(10^{-0.5})
=-F\left(0.125+\frac{2.303RT}{F}0.5\right).
$$

Thus the available [proton-motive force](../../../../proton-motive-force.md) magnitude is $0.15476\,\mathrm V$, supplying $14.93\,\mathrm{kJ\,mol^{-1}}$ per transported [proton](../../../../proton.md). Assuming one [proton](../../../../proton.md) per c-subunit per revolution, three [ATP](../../../../adenosine-triphosphate.md) per revolution and no leakage, slippage or transport overhead,

$$
\Delta G_{\rm turn}=3g_{\rm ATP}-n_cF\Delta p,\qquad
\boxed{n_c\geq\frac{3g_{\rm ATP}}{F\Delta p}=12.70.}
$$

The smallest integer permitting synthesis is therefore $\boxed{n_c=13}$ in this ideal budget. A ring of thirteen gives only a small driving margin; inefficiency or sustained finite output could require a larger ring. The result is an energetic lower bound and near-reversible estimate, not a unique structural determination from these data. Reasonable temperatures near $300$–$310\,\mathrm K$ leave the minimum integer thirteen. Additional [membrane transport](../../../../membrane-transport.md) costs have been excluded explicitly.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
