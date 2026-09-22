<h1 id="section-a-ii/15/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume the usual one-lead-biased measurement, $V_s=V_{sd}$ with drain grounded and the gate referred to that ground; the printed map does not separately specify the wiring. This assumption is needed to assign individual source/drain capacitances. In this [Coulomb diamond capacitance extraction](../../../../../../coulomb-diamond-capacitance-extraction.md), the smaller zero-bias gate intervals are 5 mV wide. In the [constant interaction model](../../../../../../constant-interaction-model.md) with no orbital gap between those additions,

$$
C_g=\frac e{\Delta V_g}=\frac{1.602\times10^{-19}}{5\times10^{-3}}
=32.04\ \mathrm{aF}.
$$

An upper diamond tip lies at gate 123.75 mV between the zero-bias vertices 120 and 125 mV and at bias 2.50 mV. Its positive and negative edge slopes are therefore $s_+=2.50/3.75=2/3$ and $s_-=-2.50/1.25=-2$. Reservoir alignment gives

$$
s_-=-\frac{C_g}{C_s},\qquad
s_+=\frac{C_g}{C_\Sigma-C_s}=\frac{C_g}{C_g+C_d}.
$$

The [gate capacitance](../../../../../../gate-capacitance.md) is not negligible in the second denominator. Consequently

$$
\boxed{C_s\simeq16.0\ \mathrm{aF},\quad C_d\simeq16.0\ \mathrm{aF},\quad
C_g\simeq32.0\ \mathrm{aF},\quad C_\Sigma\simeq64.1\ \mathrm{aF}.}
$$

The consistency check is $e^2/C_\Sigma=2.50\ \mathrm{meV}$, matching the smaller tip's bias energy. The conventional electrostatic [charging energy](../../../../../../charging-energy.md) $E_C=e^2/(2C_\Sigma)$ is 1.25 meV; it is half the [charging energy](../../../../../../charging-energy.md) contribution to the [addition energy](../../../../../../addition-energy.md). A different applied-bias convention changes the slope formulas, so the convention must accompany the extraction.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [15](../../15.md)
3. [Section A(ii)](../../../section-a-ii.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
