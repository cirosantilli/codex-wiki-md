<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $H$ denote a ridge's peak [sea-ice draft](../../../../../../sea-ice-draft.md), reserving $h$ for the draft at a randomly sampled position. In the [exponential ridge-draft model](../../../../../../exponential-ridge-draft-model.md), normalization by the line density $\mu$ gives

$$
\mu=\int_{h_0}^\infty Be^{-bH}\,dH
=\frac{B}{b}e^{-bh_0}.
$$

The mean peak [sea-ice draft](../../../../../../sea-ice-draft.md) is

$$
h_m=\frac1\mu\int_{h_0}^\infty HBe^{-bH}\,dH
=h_0+\frac1b.
$$

Consequently

$$
\boxed{b=\frac1{h_m-h_0},\qquad
B=\frac{\mu}{h_m-h_0}\exp\left(\frac{h_0}{h_m-h_0}\right),}
$$

with $h_m>h_0$, $b$ having dimensions inverse length and $B$ inverse length squared. The normalized peak [probability density function](../../../../../../probability-density-function.md) is a shifted [exponential distribution](../../../../../../exponential-distribution.md).

For the triangular argument, interpret the common ridge shape as geometrically similar triangles with common along-track slope $\tan\delta$ and variable peak height. Literal congruence would require identical sizes and could not coexist with an exponential peak-draft distribution. Each side of a triangle has $dx=|dh|/\tan\delta$. A ridge reaching draft $H\ge h$ therefore contributes $2\cot\delta\,dh$ of horizontal track in the interval $[h,h+dh]$. Summing this occupation length over all qualifying peaks proves the [triangular ridge occupation identity](../../../../../../triangular-ridge-occupation-identity.md):

$$
g(h)=2\cot\delta\int_h^\infty n(H)\,dH
=\frac{2B}{b\tan\delta}e^{-bh},
\qquad h\ge h_0.
$$

Thus

$$
\boxed{A=\frac{2B}{b\tan\delta}.}
$$

This is a tail relation for sampled draft occupation, not an instruction to normalize $n$ and $g$ identically. Below $h_0$, the ideal triangles contribute $2\mu\cot\delta$ rather than the same exponential; level ice and gaps contribute their own draft distributions. If triangular keels are referenced to a level-ice base, the vertical coordinate must be shifted consistently. We also require nonoverlapping occupation: arbitrary choices of $\mu$, mean draft and slope can otherwise demand more than the available track length.

Observed mean keel slopes are typically of order $20^\circ$–$30^\circ$, with broad individual variation rather than a single universal angle. Orientation matters: if a track crosses a straight ridge at angle $\psi$ to the crest, $\tan\delta_{\rm track}=\tan\delta_\perp|\sin\psi|$. The track slope can therefore approach zero at a grazing crossing. [A sonar morphology study](https://doi.org/10.1029/95JC00007) found location-dependent mean slopes about $22^\circ$–$27^\circ$ after correcting for ridge orientation.

Young [sea-ice pressure ridges](../../../../../../sea-ice-pressure-ridge.md) often have recognizably triangular sections with angular, porous rubble and comparatively continuous crests. Melting, refreezing and repeated cracking modify older ridges: their blocks can become rounded and consolidated, and their keel or crest can fragment into separated hummocks rather than retain one triangular shape. [A pre-exam multibeam study](https://doi.org/10.1016/j.polar.2012.03.002) found [first-year sea ice](../../../../../../first-year-sea-ice.md) ridge slopes averaging roughly $27^\circ$, while [multi-year sea ice](../../../../../../multi-year-sea-ice.md) ridges often consisted of irregular separated smooth blocks. Multi-year sections can be broader or locally shallower, but age alone does not determine one slope angle. **The constant-slope triangle is a useful statistical idealization, not a faithful shape for every old ridge.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
