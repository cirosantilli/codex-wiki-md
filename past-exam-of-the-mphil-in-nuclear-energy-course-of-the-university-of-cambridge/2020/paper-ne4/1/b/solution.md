<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the thermal power when applying [nuclear fuel burnup](../../../../../nuclear-fuel-burnup.md). No [capacity factor](../../../../../capacity-factor.md) is supplied, so take a full-power year of $365$ days; if the operating fraction were $u$, the annual quantities in this part would be multiplied by $u$.

$$
P_{\rm th}=\frac{1650}{0.37}=4459.459\ \mathrm{MW},\qquad
E_{\rm th}=4459.459(365)=1.627703\times10^6\ \mathrm{MW\,d\,yr^{-1}}.
$$

The corresponding initial heavy-metal [nuclear fuel](../../../../../nuclear-fuel.md) requirement is

$$
M=\frac{E_{\rm th}}{55000}=\boxed{29.5946\ \mathrm{t\,U\,yr^{-1}}}.
$$

All [nuclear fuel](../../../../../nuclear-fuel.md) and concentrate masses below are [uranium](../../../../../uranium.md) masses, excluding oxygen. Let $F,P,W$ denote [uranium](../../../../../uranium.md) feed, product and [enrichment tails](../../../../../enrichment-tails.md), and $x_f,x_p,x_w$ the [uranium-235](../../../../../uranium-235.md) [mass fractions](../../../../../mass-fraction.md). Conservation of total [uranium](../../../../../uranium.md) and [uranium-235](../../../../../uranium-235.md) gives

$$
F=P+W,\qquad Fx_f=Px_p+Wx_w,
$$

so

$$
\frac FP=\frac{x_p-x_w}{x_f-x_w}
=\frac{0.050-0.003}{0.007-0.003}=11.75.
$$

With $P=M$, the [uranium oxide concentrate](../../../../../uranium-oxide-concentrate.md) requirement is therefore

$$
F=11.75M=\boxed{347.7365\ \mathrm{t\,U\,yr^{-1}}},\qquad
W=318.1419\ \mathrm{t\,U\,yr^{-1}}.
$$

This is not the gross mass of oxide concentrate. Both $F-P-W=0$ and $0.007F-0.050P-0.003W=0$ provide independent balance checks.

## ↑ Ancestors (10)

1. [B](../b.md)
2. [1](../../1.md)
3. [Module NE4](../../../paper-ne4-split.md)
4. [2020](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
