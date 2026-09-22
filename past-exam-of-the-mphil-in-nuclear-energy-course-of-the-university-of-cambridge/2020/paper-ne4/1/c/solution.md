<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The recycle feed is the recovered [uranium](../../../../../uranium.md), not the whole initial [nuclear fuel](../../../../../nuclear-fuel.md) charge. After the stated loss it is

$$
F_r=27(1-0.015)=26.595\ \mathrm{t\,U\,yr^{-1}}.
$$

Using the same [enrichment tails](../../../../../enrichment-tails.md) assay and the stipulated higher recycle-product assay, the [isotopic mass balance](../../../../../isotopic-mass-balance.md) gives

$$
P_r=F_r\frac{0.0085-0.003}{0.053-0.003}
=2.925450\ \mathrm{t\,U\,yr^{-1}},\qquad
W_r=F_r-P_r=23.669550\ \mathrm{t\,U\,yr^{-1}}.
$$

Treat the $5.3\%$ recycled product as replacing the same [uranium](../../../../../uranium.md) mass of ordinary $5.0\%$ [nuclear fuel](../../../../../nuclear-fuel.md): the additional [uranium-235](../../../../../uranium-235.md) compensates for the supplied [uranium-236](../../../../../uranium-236.md) penalty. It displaces fresh natural-uranium feed in the ratio calculated in part (b), hence

$$
\Delta F=11.75P_r=\boxed{34.37404\ \mathrm{t\,U\,yr^{-1}}}.
$$

The remaining natural feed is $313.36245\ \mathrm{t\,U\,yr^{-1}}$, a **9.885% resource saving** relative to the full-power once-through requirement. This credits one [uranium](../../../../../uranium.md) recycle only; it adds no second-pass recycling or [plutonium](../../../../../plutonium.md) credit.

Separative work must be charged for producing the recycled [nuclear fuel](../../../../../nuclear-fuel.md) as well as credited for displaced fresh [nuclear fuel](../../../../../nuclear-fuel.md). With [uranium-235](../../../../../uranium-235.md) [mass fraction](../../../../../mass-fraction.md) $x$, use the [separative value function](../../../../../separative-value-function.md)

$$
V(x)=(1-2x)\ln\frac{1-x}{x},\qquad
S=PV(x_p)+WV(x_w)-FV(x_f).
$$

Masses in kilograms give work in kg-SWU. For ordinary fresh product the work per product kilogram is

$$
s_f=V(0.050)+10.75V(0.003)-11.75V(0.007)
=7.28741475\ \mathrm{kg\!\text{-}\!SWU\,kg^{-1}}.
$$

Thus the fresh work avoided is

$$
S_{\rm avoided}=1000P_rs_f=21318.9675\ \mathrm{kg\!\text{-}\!SWU\,yr^{-1}}.
$$

The recycled product still requires

$$
S_r=1000\big[P_rV(0.053)+W_rV(0.003)-F_rV(0.0085)\big]
=19726.2085\ \mathrm{kg\!\text{-}\!SWU\,yr^{-1}}.
$$

The **net separative-work saving** is consequently

$$
\Delta S=S_{\rm avoided}-S_r
=\boxed{1592.7590\ \mathrm{kg\!\text{-}\!SWU\,yr^{-1}}}.
$$

As a whole-cycle check, the fresh route requires $215668.0851$ kg-SWU per year, while the mixed fresh-plus-recycled supply requires $214075.3261$ kg-SWU. The net saving is only **0.7385%** of the original work. The recovered stream has a higher [uranium-235](../../../../../uranium-235.md) assay than natural feed, but the higher required product assay uses most of the work credit. These equations are resource accounting and do not specify an [uranium enrichment](../../../../../uranium-enrichment.md) plant or its operation.

## ↑ Ancestors (10)

1. [C](../c.md)
2. [1](../../1.md)
3. [Module NE4](../../../paper-ne4-split.md)
4. [2020](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
