<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[burnup](../../../../../nuclear-fuel-burnup.md) refers to thermal energy per initial heavy-metal mass. Correct the electrical rating for [thermal efficiency](../../../../../thermal-efficiency.md) before using it, and apply the [capacity factor](../../../../../capacity-factor.md) once:

$$
P_{\rm th}=\frac{1600}{0.33}=4848.48 \mathrm{MW},\qquad
E_{\rm th}=P_{\rm th}(365)(0.9)=1.592727\times10^6 \mathrm{MW\,d\,yr^{-1}}.
$$

Consequently the annual initial heavy-metal fuel requirement is

$$
M=\frac{E_{\rm th}}{45000}=\boxed{35.394 \mathrm{t\,HM\,yr^{-1}}}.
$$

Let $F,P,W$ be feed, enriched product and [enrichment tails](../../../../../enrichment-tails.md) masses, all measured as [uranium](../../../../../uranium.md), and $x_f,x_p,x_w$ the corresponding [uranium-235](../../../../../uranium-235.md) [mass fractions](../../../../../mass-fraction.md). The [isotopic mass balance](../../../../../isotopic-mass-balance.md) gives

$$
F=P+W,\qquad Fx_f=Px_p+Wx_w,\qquad
\frac FP=\frac{x_p-x_w}{x_f-x_w}=\frac{0.040-0.003}{0.007-0.003}=9.25.
$$

With $P=M$, the [uranium oxide concentrate](../../../../../uranium-oxide-concentrate.md) requirement is therefore

$$
F=9.25M=\boxed{327.394 \mathrm{t\,U\,yr^{-1}}},\qquad W=292.000 \mathrm{t\,U\,yr^{-1}}.
$$

These are [uranium](../../../../../uranium.md) or heavy-metal masses, **not tonnes of [uranium](../../../../../uranium.md) oxide**. The check $327.394(0.007)=35.394(0.040)+292.000(0.003)$ closes the [uranium-235](../../../../../uranium-235.md) balance as well as the total mass balance.

## ↑ Ancestors (10)

1. [B](../b.md)
2. [1](../../1.md)
3. [Module NE4](../../../paper-ne4-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
